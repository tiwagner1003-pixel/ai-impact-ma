---
title: "The Memorization Problem: Can We Trust LLMs' Economic Forecasts?"
type: source
created: 2026-05-04
updated: 2026-05-04
sources: []
origin: research/input/inbox/2504.14765v2.pdf
author: Alejandro Lopez-Lira, Yuehua Tang, Mingyin Zhu
date: "2025-12-16"
aliases: [Lopez-Lira et al. 2025, arXiv 2504.14765, Memorization Problem paper]
---

# The Memorization Problem: Can We Trust LLMs' Economic Forecasts?

**Lopez-Lira, Tang & Zhu (2025) prove that LLM-based economic forecasting on pre-training-cutoff data is fundamentally non-identified — genuine forecasting skill and memorization are observationally equivalent — and demonstrate empirically that GPT-4o has memorized macroeconomic indicators, stock market indices, and individual security prices with near-perfect precision for pre-cutoff periods, while post-cutoff accuracy collapses to near-random levels.**

## Key takeaways

- LLMs cannot be trusted for economic forecasting during periods covered by their training data; this is a formal non-identification problem: any correct forecast is consistent with both genuine skill and memorized recall of the outcome.
- GPT-4o recalls S&P 500 daily closing values (MAPE 0.61%), unemployment rates (MAE 0.03 pp), and GDP growth figures (threshold accuracy 96.27%) for pre-cutoff periods; post-cutoff accuracy collapses to near-random (threshold accuracy 29–53% across indicators).
- Prompt-based constraints ("use only data before 2010") do not prevent recall: GPT-4o achieves 97.6% threshold accuracy when "constrained" to pre-2010 data vs. 98.0% unconstrained, both far above the 40% post-cutoff baseline for truly unseen data.
- Masking (entity neutering — removing company names, dates, numbers) also fails: GPT-4o correctly identifies Apple, Meta, and Microsoft in 100% of anonymized earnings call transcripts, and Alphabet in 91.89%; the model reconstructs entities from minimal contextual clues.
- Fine-tuning to "forget" post-cutoff data fails for the same structural reason: observationally equivalent outcomes (genuine forgetting vs. behavioral suppression of known information) cannot be distinguished without white-box parameter inspection.
- The memorization problem extends to LLM embeddings: Ridge regression on date-and-variable embeddings predicts inflation (r = 0.892) and unemployment (r = 0.927) far above the 5-year SMA benchmark; temporal information appears encoded in embedding geometry.
- The direct implication for studies like Degen et al. (2024) is that apparent predictive power in pre-cutoff LLM forecasting tasks (e.g., MASS, 2013–2023) may entirely reflect memorization of realized outcomes rather than genuine extraction of managerial private information.

## Claims

- The memorization problem is formally non-identified: when a model has seen realized values during training, the counterfactual forecasting ability (what it would have predicted without post-cutoff information) cannot be recovered from the observed output (Proposition 1).
- Corollary 1 proves sharp non-identification: for any constrained LLM output, the identified set for the true counterfactual forecast equals the entire label space — observing constrained outputs provides zero information about the ideal estimand.
- Corollary 2 proves that black-box fine-tuning to "forget" fails: the same non-identification holds for fine-tuned outputs because genuine forgetting and behavioral suppression are observationally equivalent without white-box verification.
- Proposition 2 proves statistical indistinguishability: when post-cutoff sample size is small relative to pre-cutoff sample size, standard hypothesis tests cannot reliably distinguish genuine forecasting skill from undetected memorization due to low statistical power.
- Any memorization test establishes only a lower bound on encoded knowledge: positive evidence of memorization is conclusive, but failure to elicit memorized knowledge in a specific test does not prove its absence (Remark 1).
- GPT-4o (version gpt-4o-2024-08-06, training cutoff October 2023) recalls pre-cutoff macroeconomic rates with Threshold Accuracy exceeding 96% across GDP Growth, Inflation, Unemployment Rate, and 10-Year Treasury Yield (January 1990 to September 2023, Table 1).
- Post-cutoff (October 2023 to February 2025), Threshold Accuracy for the same indicators falls to 29.41%–52.94% — near or below random (50%) — with Mean Absolute Errors increasing by factors of 6–30x.
- Recency effect: GPT-4o's memorization is stronger for recent pre-cutoff data — MAPE for Nonfarm Payrolls falls from 66.30% over the full sample to 0.00% for the most recent 10-year sub-period; Threshold Accuracy rises to 95–100% for level indicators in the recent period.
- GPT-4o recalls daily S&P 500 closing values with MAPE 0.61% (pre-cutoff) vs. 16.87% (post-cutoff); daily DJIA with MAPE 0.53% vs. 13.01%; daily Nasdaq Composite with MAPE 1.80% vs. 20.48% (Table 2).
- GPT-4o identifies WSJ front-page headline dates with 98.45% year accuracy and 90.38% month-and-year accuracy pre-cutoff; post-cutoff year accuracy falls to 28.81% (Table 3).
- Individual stock price recall is selective: META has MAPE 0.37% and Directional Accuracy 99.26% pre-cutoff, while AAPL has MAPE 36.44% without context; providing two months of context sharply reduces errors across all Magnificent 7 stocks (Table 4).
- GPT-4o correctly identifies the company in anonymized earnings call transcripts with 100% accuracy for AAPL, META, MSFT; 93.24% quarter-and-year accuracy for AAPL (Table 7). Masking fails as a safeguard.
- A fundamental trade-off makes masking structurally inadequate: text specific enough to carry forecasting signal is also specific enough to enable entity reconstruction; text generic enough to prevent reconstruction loses its forecasting signal.
- The memorization problem applies to all "future-variant" tasks — tasks where an analyst's answer would differ knowing future outcomes — including sentiment classification, relevance assessment, risk identification, and expectation extraction; only purely factual extraction tasks are likely unaffected.
- M&A sentiment analysis as practiced in Degen et al. (2024) is a future-variant task: classifying whether an earnings call paragraph is "M&A-relevant" and scoring its sentiment is judgment-laden, and the model's parameters encode knowledge of which M&A deals actually occurred after the transcript date.
- Llama-3.1-70b-Instruct (open-source, knowledge cutoff December 2023) exhibits similar memorization patterns: Threshold Accuracy exceeds 91% for macroeconomic rates pre-cutoff; post-cutoff Threshold Accuracy drops to 60–75%. Memorization is not GPT-4o-specific.
- LLM embeddings (text-embedding-3-large) show evidence of memorization: Ridge regression on date-and-variable embeddings achieves correlation 0.892 with inflation and 0.927 with unemployment, compared to SMA benchmarks of 0.333 and 0.385 respectively; placebo tests confirm the signal is driven by temporal information encoded in the embeddings (Table 13).
- Memorization extends internationally: similar recall behavior documented for Euro area, UK, Japan, and China macroeconomic indicators and for Euro Stoxx 50, FTSE 100, Nikkei 225, and SSE Composite Index.
- The only reliable methodological solution is to test LLM forecasting ability exclusively on data after the model's training cutoff, where memorization is structurally impossible.

## Entities mentioned

- [[alejandro-lopez-lira]]
- [[yuehua-tang]]
- [[mingyin-zhu]]
- [[university-of-florida]]
- [[gpt-4]]
- [[chatgpt]]
- [[mass-index]]
- [[dominik-degen]]

## Concepts mentioned

- [[memorization-problem-llms]]
- [[lookahead-bias]]
- [[llms-in-ma]]
- [[ma-sentiment-analysis]]
- [[earnings-conference-calls]]
- [[prompt-engineering]]
- [[generative-ai-in-ma]]
- [[ai-in-ma]]

## Notes

**Publication status:** arXiv working paper (arXiv:2504.14765 [q-fin.GN]). First version: April 15, 2025; this version: December 16, 2025. Presented at the 2025 GSU-MS AI & FinTech Conference and the Applied Machine Learning, Economics, and Data Science (AMLED) Webinar. Submitted to *Journal of Accounting, Auditing and Finance* (JAAF). NOT yet peer-reviewed as of ingest date — cite with explicit working-paper qualifier in the seminar paper. URL: https://arxiv.org/abs/2504.14765

**Institutional affiliation:** All three authors: University of Florida (Warrington College of Business). Contact: alejandro.lopez-lira@warrington.ufl.edu

**Relationship to Degen et al. (2024):** Lopez-Lira et al. explicitly name Degen et al. (2024) in their list of studies warranting caution (p. 9: "Degen et al. 2024"). The MASS study uses GPT-4.0/GPT-4o to score earnings call paragraphs from 2013 to 2023 — a period entirely within GPT-4o's training data. The measured predictive power of MASS may reflect recall of the M&A outcomes rather than genuine extraction of managerial private information. This is the primary methodological concern for the Thema 7 seminar paper's critical reflection section (Abschnitt 4).

**Key quote (abstract):** "LLMs cannot be trusted for economic forecasts during periods covered by their training data. Counterfactual forecasting ability is non-identified when the model has seen the realized values: any observed output is consistent with both genuine skill and memorization."

**Key quote (p. 3):** "When we instruct GPT-4o to ignore any information after 2010 when forecasting quarterly GDP growth direction, the model achieves 97.6% threshold accuracy before the artificial cutoff and 98.0% after, nearly identical performance despite the explicit constraint. In contrast, actual post-knowledge cutoff accuracy is only 40%."

**Key quote (p. 44):** "Achieving both effective anonymization and meaningful forecasting power simultaneously is highly challenging. Combined with Remark 1, which establishes that failed identification does not prove successful anonymization, this trade-off suggests masking cannot reliably solve the memorization problem for forecasting tasks."

**Practical guidance (p. 11):** The paper provides a simple researcher heuristic: "Would an analyst's answer differ if they knew what happened after time t? If the answer is yes, or even plausibly yes, the task is not future-invariant." Tasks classified as NOT future-invariant (and therefore unreliable pre-cutoff): sentiment and tone analysis, risk/uncertainty extraction, forecasting and expectations, similarity and comparison, judgment-based relevance assessments.

**Data:** Tests cover January 1990 – September 2023 (pre-cutoff) and October 2023 – February 2025 (post-cutoff). Variables: S&P 500, DJIA, Nasdaq (Yahoo Finance); 4,200+ individual stocks (CRSP); GDP growth, inflation, unemployment, 10-yr Treasury Yield, VIX, housing starts, nonfarm payrolls (FRED, Philadelphia Fed Real-Time Data Set); 90,123 WSJ front-page headlines (Factiva); earnings call transcripts (Capital IQ); firm headlines (RavenPack).

**Suggested follow-up sources:**
- Engelberg et al. (2025) — "entity neutering" as a proposed (but ultimately insufficient) anonymization method; cited and empirically refuted in Lopez-Lira et al.
- Bozman, Fairhurst & Greene (2025) — "Better Than a Coin Flip? Merger Success and Artificial Intelligence Models" — a post-cutoff LLM study that avoids the memorization problem by design; cited positively in Lopez-Lira et al.
- Ludwig, Mullainathan & Rambachan (2025) — related econometric framework addressing "training leakage" (a related but distinct concept); cited in related literature section.
