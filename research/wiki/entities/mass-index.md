---
title: M&A Sentiment Score (MASS)
type: entity
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [MASS, M&A Sentiment Score, ChatGPT M&A Sentiment Score]
entity_kind: product
---

# M&A Sentiment Score (MASS)

**A novel monthly aggregate index of corporate M&A sentiment constructed by applying ChatGPT (GPT-4.0) to earnings call transcripts of S&P Global 1200 companies, developed by Degen, Kengelbach, Kim, Sievers & Wang (2024).**

## Overview

MASS is constructed in three aggregation steps: (1) ChatGPT scores each M&A-relevant earnings call paragraph on a –2 to +2 integer scale; (2) paragraph scores are averaged to transcript level, then averaged to a monthly series; (3) a 3-month rolling average is applied to smooth quarterly reporting seasonality. The resulting series is called the "raw MASS." For forecasting purposes, the 18-month lagged version of the raw MASS is used as the predictive variable. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

Empirically, an 18-month lag is optimal: it reflects the deal preparation timeline (target identification, due diligence, negotiation, regulatory approval) documented in the M&A literature. The univariate model with 18-month lagged MASS achieves adj. R² of 9.1%. When combined with the OECD Business Confidence Index, the combined model explains 44.1% of monthly deal activity. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

Only extreme quintile positions in MASS (top 20% and bottom 20%) are statistically significant predictors of future deal volume; the middle quintiles have no significant effect. A very high MASS score is associated with fewer deals 18 months later (negative coefficient), consistent with a late-cycle sentiment indicator interpretation analogous to patterns found in equity markets. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- Sample period: July 2013 – December 2023, monthly frequency. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Mean raw score: 0.80 (standard deviation 0.08), indicating persistently mild positive M&A sentiment among S&P 1200 executives. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Out-of-sample R²OS: 9.4%, statistically significant (Clark-West p = 0.024). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Correlation with OECD BCI: negative (cyclicality argument); correlation with Baker-Wurgler and Huang et al.: positive (all capture non-consumer managerial sentiment). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Published as TRR 266 Working Paper No. 150, July 2024. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[chatgpt]] — the model used to score paragraphs
- [[gpt-4]] — the specific model version (GPT-4.0)
- [[s-p-global-1200]] — the company universe from which transcripts are drawn
- [[baker-wurgler-sentiment-index]] — benchmark sentiment index compared against MASS
- [[oecd-business-confidence-index]] — strongest benchmark; combined with MASS for best prediction
- [[ma-sentiment-analysis]] — the underlying methodology
- [[prompt-engineering]] — key technical determinant of score quality
- [[merger-waves]] — the aggregate phenomenon MASS is designed to predict

## Open questions

- Is MASS publicly available for replication or further research?
- Would a real-time or quarterly MASS update be feasible operationally?
- How does MASS behave across different industries or geographies?
