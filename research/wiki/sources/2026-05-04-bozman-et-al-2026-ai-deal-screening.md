---
title: "Better Than a Coin Flip? Screening Mergers and Acquisitions With Artificial Intelligence Models"
type: source
created: 2026-05-04
updated: 2026-05-04
sources: []
origin: research/input/inbox/ssrn-5421737.pdf
author: Adam Bozman, Douglas (DJ) Fairhurst, Daniel Greene
date: March 2026 (first draft April 2024)
aliases: [Bozman et al. 2026, SSRN 5421737, AI Deal Screening]
---

# Better Than a Coin Flip? Screening Mergers and Acquisitions With Artificial Intelligence Models

**Bozman, Fairhurst & Greene (2026) provide the first empirical test of whether ML models and LLMs can screen M&A deals to improve acquirer announcement returns out-of-sample, finding that ML models reliably do so while baseline LLMs do not, and that governance quality and deal complexity moderate effectiveness.**

## Key takeaways

- AI models (both classical ML and LLMs) can forecast the direction of acquirer stock-price reactions to M&A announcements; ML models consistently outperform baseline LLMs in this task.
- Out-of-sample testing on 615 deals (October 2021 – December 2024) shows ML deal screening raises mean acquirer returns from 0.39% (unconditional) to 1.05% when acting on positive predictions; optimized ML models raise this further to over 5%.
- Fine-tuning GPT-4o on 500 recent deals substantially improves LLM performance (directional accuracy 61.7%, mean return 3.00%), partially closing the gap with ML.
- AI screening is significantly more effective for firms with weaker governance (staggered boards), suggesting AI can counteract managerial biases such as hubris and empire-building.
- AI screening is much less effective for complex deals (acquirer and target in different two-digit SIC industries), consistent with evidence that AI models struggle as task complexity rises.
- The out-of-sample period begins after GPT-4's knowledge cutoff (September 30, 2021), structurally ruling out the memorization problem identified by Lopez-Lira et al. (2025) for LLM predictions.
- Two distinct channels drive AI-enabled improvement: identifying large-magnitude return deals (both positive and negative) and detecting overpayment relative to fair value.

## Claims

- The average three-day acquirer announcement return in the 615-deal out-of-sample period is 0.39% (not statistically different from zero), and 50.1% of deals have positive returns — odds similar to a coin flip. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- ML models achieve directional accuracy of 53.7% in the standardized testing period, compared to the unconditional positive rate of 50.1%; only ML models have AUC values that statistically differ from 0.50. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- Deals predicted to increase value by ML models show mean observed returns of 1.05%, compared to -2.26% for deals predicted to decrease value; the 3.32% difference is statistically significant. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- Baseline LLMs (GPT-4 prompted with serialized deal data) show mean observed returns of only 0.28% for deals predicted to increase value — economically small and not statistically significant, indicating no predictive ability in the baseline setting. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- The ML ensemble uses the median of Ridge, Lasso, Random Forest, and Gradient Boosting predictions; training period spans January 1988 to September 2021 (6,098 deals). [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- The most important features for the gradient-boosted ML model are Public Target status, Relative Size, and Total Assets of the acquirer; interaction terms account for more than half of each variable's total importance. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- When ML predicts returns above 1%, observed returns average 3.23%; when it predicts returns below -1%, observed returns average -3.43%; the AUC is 0.65, substantially above random selection. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- For ML predicted wealth losses in the bottom decile, the average observed wealth loss is -$2.7 billion, compared to -$0.19 billion for the top nine deciles — confirming ML's ability to flag large-loss deals. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- In an overpayment experiment (varying offer price 0.1x–10x), LLMs show the highest sensitivity: a 10x offer price increase leads to 25.22% fewer deals predicted to increase value (vs. 4.23% for ML), and halving the price increases positive predictions by 14.67% for LLMs. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- For firms with staggered boards (weaker governance), ML screening raises positive-prediction observed returns to 1.60% (vs. 0.39% for all deals); AUC is 0.58 and statistically different from 0.50; for non-staggered board firms the screening effect is not statistically significant. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- For same-industry (less complex) deals, ML positive predictions yield observed returns of 1.90% with AUC 0.59 (statistically significant); for cross-industry (more complex) deals, neither the return difference nor the AUC is statistically significant. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- When the ML testing period is extended to January 2018 – December 2024 (1,554 deals) with an optimized model, mean observed returns for positive predictions reach 1.57%, and further optimizing with large-magnitude predictions produces returns of 4.83–5.17%. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- Fine-tuning GPT-4o on 500 recent deals (500 most recent prior to October 2023) yields directional accuracy of 61.7%, a mean observed return of 3.00% for positive predictions, and AUC of 0.62 — all statistically significant. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- GPT-4o (tested in Section 7) performs no better than random in the baseline (no fine-tuning) setting, underscoring that the improvement from fine-tuning is specific to the domain-adaptation step. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- The GPT-4 variant used (gpt-4-0613, snapshot of GPT-4.0 as of June 13 2023) has a training data cutoff of September 2021, making the October 2021 – December 2024 testing window fully post-cutoff and therefore not subject to the memorization problem. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- Moeller, Schlingemann & Stulz (2005) found that a small number of deals destroyed nearly $400 billion in shareholder wealth in the late 1990s; Bozman et al. show that AI-trained large-loss prediction models can flag such deals, with ML raising the share of identified large-loss deals from a 10% base rate to 45.16% within the predicted-loss decile. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]

## Entities mentioned

- [[adam-bozman]]
- [[douglas-fairhurst]]
- [[daniel-greene]]
- [[washington-state-university]]
- [[clemson-university]]
- [[gpt-4]]

## Concepts mentioned

- [[ml-target-selection]]
- [[ai-in-ma]]
- [[mergers-and-acquisitions]]
- [[gradient-boosting]]
- [[memorization-problem-llms]]
- [[llms-in-ma]]
- [[generative-ai-in-ma]]
- [[ma-success-measurement]]
- [[lookahead-bias]]
- [[prompt-engineering]]

## Notes

**Positioning in the seminar paper:** This paper belongs primarily in Abschnitt 3.1 (KI in der Target-Identifikation und Deal-Sourcing) but also covers elements of Abschnitt 3.3 (KI in der Bewertung / Overpayment-Prävention). It provides the strongest empirical evidence in this wiki that AI deal screening can improve acquirer returns, making it the key quantitative anchor for Section 3.1.

**Relation to Lopez-Lira et al. (2025):** The authors are explicitly aware of the memorization critique (Lopez-Lira, Tang, and Zhu, 2026, as cited in the paper). Their methodological response is to exploit GPT-4's exogenous knowledge cutoff (September 30, 2021) as an out-of-sample divider, ensuring the test set is structurally post-cutoff. This is the most credible design available given current LLMs. However, the paper also tests GPT-4o (cutoff October 2023), which leaves only November 2023 – December 2024 as the test window (short and concentrated in a single macroeconomic episode). The fine-tuning results should be read with this caveat.

**ML vs. LLM comparison:** The paper provides a clean head-to-head under identical training/testing windows and feature sets. The conclusion is clear: in the baseline setting, ML models have statistically significant AUC > 0.50; baseline LLMs do not. Fine-tuning partially closes the gap. This is consistent with and extends the finding in Cao et al. (2024) that human-machine combinations can outperform either alone.

**Key quote (abstract):** "Screening deals with AI models is more effective for firms with weaker governance, suggesting the potential to counteract managerial biases, and is less effective for complex deals."

**Key quote (Section 3.2):** "Our methodology side-steps common problems with predictions made by LLMs, including a look-ahead bias (Sarkar and Vafa, 2024) and a memorization problem (Lopez-Lira, Tang, and Zhu, 2026). [...] An out-of-sample period beginning in October 2021, which is after GPT-4's knowledge cutoff, avoids both problems."

**Data sources used:** Refinitiv SDC (deal data), Compustat (acquirer financials), CRSP/Eventus (announcement returns), Guernsey et al. (2022/2024) staggered board data.

**Sample:** 6,713 deals total (January 1988 – December 2024); 6,098 training deals; 615 out-of-sample test deals. U.S.-based, publicly listed acquirers; deal value ≥ $50 million; U.S.-based public or private targets.

**Publication status:** SSRN Working Paper 5421737 (not yet peer-reviewed). First draft April 2024; this draft March 2026. JEL codes G30, G34.

**Open questions for the seminar paper:**
- Can the governance-moderated finding (AI is more useful for weak-governance firms) inform a policy recommendation about who should adopt AI deal screening tools?
- Does the ML-beats-LLM finding in the baseline persist if LLMs are augmented with retrieval-augmented generation (RAG) to access structured financial databases?
- How does the finding relate to the Jensen (1986) free-cash-flow / empire-building hypothesis — is the governance channel a pure managerial-bias story or does it reflect information quality?
