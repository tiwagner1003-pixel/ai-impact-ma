---
title: Baker-Wurgler Investor Sentiment Index
type: entity
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [Baker-Wurgler, BAKER_WURGLER, Baker and Wurgler 2006]
entity_kind: dataset
---

# Baker-Wurgler Investor Sentiment Index

**An investor sentiment index developed by Baker and Wurgler (2006) as the first principal component of six stock market-based proxies; one of the benchmark indices used to validate MASS in Degen et al. (2024).**

## Overview

The Baker-Wurgler index is constructed from six stock market proxies: the closed-end fund discount, NYSE share turnover, number and first-day returns of IPOs, equity share in new issues, and the dividend premium. It is widely used in empirical finance as a measure of equity market investor sentiment. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

In the MASS study, Baker-Wurgler is one of four benchmark sentiment indices. It is positively correlated with MASS (indicating both capture non-consumer managerial/investor sentiment), and it adds incremental forecasting value not already included in MASS — making it one of the benchmarks that MASS does not fully encompass. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- Source: Baker, M., Wurgler, J. (2006). Investor sentiment and the cross-section of stock returns. Journal of Finance, 61(4), 1645–1680.
- Out-of-sample R²OS in MASS study: 4.4% vs MASS's 9.4%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Forecast encompassing test: MASS does not fully encompass Baker-Wurgler (Baker-Wurgler retains some incremental predictive content). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[mass-index]] — the new index tested against this benchmark
- [[oecd-business-confidence-index]] — a stronger benchmark in the same study
- [[ma-sentiment-analysis]] — the application context

## Open questions

- Does Baker-Wurgler's value-add over MASS come from its measurement of retail/market-wide sentiment vs. corporate managerial sentiment?
