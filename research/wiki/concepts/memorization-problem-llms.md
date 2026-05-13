---
title: Memorization Problem (LLMs)
type: concept
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms, 2026-05-04-bozman-et-al-2026-ai-deal-screening]
aliases: [LLM memorization, training data memorization, memorization problem]
---

# Memorization Problem (LLMs)

**The fundamental identification failure that arises when large language models are used to "forecast" economic or financial outcomes for periods covered by their training data: because the model may have memorized realized values during training, genuine forecasting ability and simple recall are observationally equivalent and cannot be distinguished.**

## Summary

LLMs are trained on comprehensive internet-scale datasets up to a knowledge cutoff date. When researchers use LLMs to evaluate historical expectations, backtest investment strategies, or produce "forecasts" of economic variables for dates within the training period, they face a structural identification problem: any correct output is consistent with two mutually incompatible explanations — (1) the model has genuine analytical skill and correctly reasoned from available pre-cutoff information, or (2) the model memorized the realized outcome during training and is recalling it rather than predicting it. These two explanations produce identical observable outputs, making inference logically impossible. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

Lopez-Lira, Tang & Zhu (2025) formalize this as a non-identification result (Proposition 1): for any set of constraining prompts designed to restrict the model to information available at time t, the ideal counterfactual estimand cannot be uniquely identified. The identified set for the true counterfactual forecast equals the entire label space — observing constrained outputs provides zero information about the ideal estimand (Corollary 1). This is not a statistical limitation addressable with larger samples; it is a logical impossibility. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

Empirically, Lopez-Lira et al. (2025) demonstrate pervasive memorization: GPT-4o recalls daily S&P 500 closing values with MAPE 0.61%, unemployment rates with MAE 0.03 percentage points, and GDP growth with 96.27% threshold accuracy for pre-cutoff data (January 1990 to September 2023). The same model achieves only 29–53% threshold accuracy on post-cutoff macroeconomic data — near or below random. A recency effect is documented: memorization is strongest for recent pre-cutoff data, consistent with denser representation in the training corpus. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

**Partial design response — Bozman et al. (2026):** Bozman, Fairhurst & Greene (2026) exploit GPT-4's exogenous knowledge cutoff (September 30, 2021) to construct a genuinely post-cutoff test period (October 2021 – December 2024, 615 deals). By ensuring no out-of-sample deal falls within GPT-4's training window, the design structurally prevents memorization for LLM predictions on that test set. The authors explicitly acknowledge both the look-ahead bias problem (Sarkar and Vafa, 2024) and the memorization problem (Lopez-Lira, Tang & Zhu, 2026) and describe their design as specifically addressing both. This is the only M&A-focused LLM study in this wiki that satisfies the Lopez-Lira et al. requirement of testing on post-cutoff data. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]

The memorization problem extends beyond text-based outputs to LLM embeddings: Ridge regression on date-and-variable embeddings predicts inflation (r = 0.892) and unemployment (r = 0.927) far above moving-average benchmarks, with placebo tests confirming the signal is driven by temporal information encoded in the embedding geometry. This means embedding-based approaches to financial prediction using pre-cutoff data are also potentially contaminated. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

## Variations / sub-concepts

- [[lookahead-bias]] — the broader family of methodological errors from using future information in historical analysis; the memorization problem is a specific, structural form of lookahead bias embedded in LLM parameters
- Training data leakage — a related concept (Ludwig, Mullainathan & Rambachan 2025) concerning whether specific training texts were in the model's corpus; the memorization problem is more fundamental because it applies even when specific inputs were not in training data, via aggregate functional contamination of the model's decision rule
- Functional lookahead bias — Lopez-Lira et al.'s preferred framing: the model's parameters encode post-t information learned from the training corpus, contaminating the decision rule even when the specific input text was never seen

## Key claims across sources

- Proposition 1 (Non-identification): Given observations from any set of constraining prompts designed to restrict the model to pre-t information, the ideal counterfactual estimand cannot be uniquely identified; any constrained output is consistent with multiple, contradictory values of the true counterfactual forecast. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- Corollary 1 (Sharp non-identification): The identified set for the counterfactual forecast equals the entire label space — constraining outputs provides zero information about the ideal estimand. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- Corollary 2 (Fine-tuning fails): Black-box fine-tuning to "forget" post-t information is subject to the same non-identification: genuine forgetting and behavioral suppression are observationally equivalent without white-box parameter inspection. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- Proposition 2 (Statistical indistinguishability): When post-cutoff sample size is small relative to pre-cutoff sample size, hypothesis tests cannot reliably distinguish skill from undetected memorization due to low statistical power. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- Any memorization test establishes only a lower bound: positive evidence is conclusive, but failure to elicit memorization in one test does not prove its absence — the model may access memorized knowledge through different contextual pathways. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- The memorization problem applies to all "future-variant" tasks — where an analyst's answer would differ knowing future outcomes — including sentiment classification, risk identification, and expectation extraction; purely factual extraction (e.g., entity names, reported numbers) is typically future-invariant and unaffected. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- The only reliable solution is to test exclusively on post-training-cutoff data, where memorization is structurally impossible. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

> ⚠️ Conflict: [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]] reports that ChatGPT (GPT-4.0) applied to 2013–2023 earnings call transcripts produces an M&A Sentiment Score (MASS) with statistically significant predictive power for M&A deal volume (out-of-sample R2 = 9.4%), and interprets this as evidence that LLMs extract genuine managerial private information. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]] demonstrates that such pre-cutoff LLM forecasting tasks are fundamentally non-identified: the MASS study's entire sample (2013–2023) is within GPT-4o's training period, so the measured predictive power is observationally equivalent to memorization of realized M&A outcomes rather than genuine information extraction. Unresolved — the Degen et al. (2024) authors have not (as of this ingest) published a response.

## Related

- [[lookahead-bias]] — the broader methodological family; memorization is a structural sub-type
- [[llms-in-ma]] — the M&A-specific application domain where the problem is most relevant for this wiki
- [[ma-sentiment-analysis]] — the specific method (MASS) most directly challenged by Lopez-Lira et al.
- [[prompt-engineering]] — cannot resolve the memorization problem; constraining prompts are formally shown to be ineffective
- [[generative-ai-in-ma]] — the broader adoption trend whose validity is partially called into question
- [[gpt-4]] — the primary model tested for memorization
- [[earnings-conference-calls]] — the data source used in both MASS and the memorization tests
- [[alejandro-lopez-lira]] — lead author of the 2025 paper
- [[mass-index]] — the specific LLM-based index whose validity is challenged

## Open questions

- ~~Does any published study satisfying the post-cutoff requirement replicate LLM predictive power in M&A?~~ Partially resolved: Bozman et al. (2026) test both ML and LLM on a post-GPT-4-cutoff sample; LLMs do not show predictive ability in the baseline setting, but fine-tuned GPT-4o does (AUC 0.62). This is the first post-cutoff study for M&A announcement return forecasting. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- Are there tasks in M&A AI that are clearly future-invariant and therefore safe for pre-cutoff LLM use?
- Does the memorization problem affect fine-tuned domain-specific FinLLMs that were not trained on general internet corpora containing financial data?
- How does the severity of memorization vary across different LLM families and sizes?
- Does fine-tuning (as used by Bozman et al. for GPT-4o) introduce a new form of the memorization problem — where training-set deal outcomes are embedded in the fine-tuned weights — that is structurally similar to Corollary 2 of Lopez-Lira et al.?
