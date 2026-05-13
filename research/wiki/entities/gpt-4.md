---
title: GPT-4
type: entity
created: 2026-05-03
updated: 2026-05-05
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence, 2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms, 2026-05-04-bozman-et-al-2026-ai-deal-screening, 2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [GPT-4.0, GPT-4o, GPT-4 Turbo, gpt4]
entity_kind: model
---

# GPT-4

**OpenAI's fourth-generation large language model family, including GPT-4.0 and GPT-4o; GPT-4.0 was selected as the primary model for the MASS study after achieving the highest correlation with human M&A expert consensus.**

## Overview

GPT-4 is OpenAI's most capable model family as of the MASS study period (2023–2024). In Degen et al. (2024), three versions were compared: GPT-4.0 (selected for main analysis), GPT-4o, and the earlier GPT-3.5-Turbo. GPT-4.0 was chosen based on the highest phi-coefficient correlation with a four-person human M&A expert panel across a 100-transcript validation sample. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

Key performance difference versus GPT-3.5-Turbo: GPT-4.0 identifies more paragraphs as M&A-relevant (68% vs 53%), which increases coverage and potentially captures more signal. GPT-3.5-Turbo also assigns higher average sentiment scores (0.95 conditional mean vs 0.82 for GPT-4.0), suggesting it may be more prone to positive-sentiment bias. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- GPT-4.0 M&A-related classification rate: 68%; average conditional sentiment: 0.82; forward-reference rate: 45%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- GPT-4o M&A-related classification rate: 66%; average conditional sentiment: 0.95; forward-reference rate: 43%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- GPT-3.5-Turbo M&A-related rate: 53%; average conditional sentiment: 0.64; forward-reference rate: 26%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

In Jang & Stikkel (2024), GPT-4 was evaluated in a few-shot in-context learning setup on the [[kira-dataset]] for M&A due diligence sentence classification. The task was simplified to paragraph-level binary classification (paragraphs of 16 sentences) to stay within context limits. GPT-4 (2–8 shots) achieved F1 of 0.81–0.82 with recall of 0.93–0.96 on topic 1243, outperforming the KIRA CRF baseline on F1 and substantially on recall. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Key facts

- GPT-4.0 M&A-related classification rate: 68%; average conditional sentiment: 0.82; forward-reference rate: 45%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- GPT-4o M&A-related classification rate: 66%; average conditional sentiment: 0.95; forward-reference rate: 43%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- GPT-3.5-Turbo M&A-related rate: 53%; average conditional sentiment: 0.64; forward-reference rate: 26%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- GPT-4 (2–8 shots) on KIRA topic 1243: recall 0.93–0.96, precision 0.70–0.72, F1 0.81–0.82 — outperforming KIRA CRF baseline (F1 0.78) on F1 and substantially on recall. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- GPT-4's context-length constraint required simplifying DD classification from full-document to 16-sentence paragraph-level processing. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Related

- [[chatgpt]] — the product/interface that uses GPT-4
- [[mass-index]] — the index built on GPT-4.0 scoring
- [[sentiment-analysis]] — the task the model performs in the MASS study
- [[prompt-engineering]] — the technique used to steer the model
- [[due-diligence]] — the legal task evaluated in Jang & Stikkel (2024)
- [[kira-dataset]] — the DD benchmark on which GPT-4 was evaluated

## Memorization findings (Lopez-Lira et al. 2025)

GPT-4o (version gpt-4o-2024-08-06, knowledge cutoff October 2023) is the primary model studied in Lopez-Lira, Tang & Zhu (2025). The paper demonstrates that GPT-4o has memorized large amounts of economic and financial data from its training: [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

- Pre-cutoff macroeconomic recall: Threshold Accuracy >96% for GDP Growth, Inflation, Unemployment Rate, 10-Year Treasury Yield (Jan 1990 – Sep 2023); post-cutoff accuracy collapses to 29–53%.
- Pre-cutoff stock market recall: MAPE 0.61% for S&P 500 daily closing values; post-cutoff MAPE 16.87%.
- WSJ headline date identification: 98.45% year accuracy pre-cutoff vs. 28.81% post-cutoff.
- Entity reconstruction: 100% firm identification accuracy for anonymized AAPL, META, MSFT earnings call transcripts.
- Fake cutoff compliance: when instructed to use only pre-2010 data, GPT-4o achieves 97.6% threshold accuracy on 2011-onward data (vs. 98.0% unconstrained), demonstrating that prompt-based constraints do not prevent recall.

This body of evidence directly challenges the use of GPT-4o (and by extension GPT-4.0, used in the MASS study) for any pre-cutoff economic forecasting or sentiment scoring task. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

## Usage in Bozman et al. (2026) — M&A deal screening

Bozman et al. (2026) use the `gpt-4-0613` model snapshot (GPT-4.0 as of June 13, 2023, trained on data through September 2021) to predict whether acquirer stock prices will increase or decrease upon a merger announcement. GPT is prompted with serialized deal and firm characteristics (bidder and target names, acquirer financials, deal features) and asked for a directional prediction. Randomness parameters are set to zero for reproducibility (frequency penalty and presence penalty set to 1, following Fairhurst and Greene 2025). [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]

Key findings in this application:
- Baseline GPT-4 achieves directional accuracy of 53% (vs. 50.1% unconditional) but its AUC is not statistically different from 0.50 — indicating no genuine predictive ability in the baseline setting.
- LLMs predict value creation in only 45.6% of deals (closer to 50-50 than ML's 79.8%), but with no statistically significant accuracy advantage.
- GPT-4 shows high sensitivity to offer price manipulation in the overpayment experiment: a 10x price increase reduces positive predictions by 25.22%, the largest sensitivity across all models tested.
- The GPT-4 training cutoff (September 2021) is used as an exogenous divider to construct a genuine out-of-sample period, directly addressing the memorization critique.
- Fine-tuning GPT-4o (cutoff October 2023) on 500 recent deals substantially improves performance: directional accuracy 61.7%, mean observed return 3.00% for positive predictions, AUC 0.62.

## Technical background (Zhao et al. 2023)

GPT-4 was released in March 2023 and represents the second major milestone in LLM development identified by Zhao et al. (2023). It extended GPT-3.5's text-only input to multimodal signals. Performance: surpasses average human performance on AGIEval (86.4% in 5-shot MMLU), which is significantly better than previous state-of-the-art models. GPT-4 "has stronger capacities in solving complex tasks than GPT-3.5, showing a large performance improvement on many evaluation tasks." [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

GPT-4 is part of the LLM generation (Generation 4 in the four-generation taxonomy), distinguished from PLMs by emergent abilities including strong in-context learning, instruction following, and chain-of-thought reasoning. The GPT series evolved from causal decoder architecture (GPT-1 through GPT-4), with training on code data being a critical enhancement: Codex (2021) showed that training on code dramatically improves reasoning ability, and the GPT-3.5 series built on code-davinci-002 inherits this. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

GPT-4 Turbo (September 2023) extended context to 128k tokens, updated knowledge to April 2023, introduced function calls, and improved reproducibility (reproducible outputs). [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Open questions

- Would GPT-4.5 or GPT-5 (post-study models) show materially different MASS properties?
- Do long-context GPT-4 variants (128k context window) change the feasibility of full-document DD classification without hierarchical decomposition?
- Does GPT-4.0 (the specific MASS model) exhibit the same memorization patterns as GPT-4o tested by Lopez-Lira et al.?
- Does fine-tuning GPT-4o on 500 deals (Bozman et al.) introduce a new form of memorization in the fine-tuned weights, as suggested by Lopez-Lira et al. Corollary 2?
