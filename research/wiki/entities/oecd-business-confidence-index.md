---
title: OECD Business Confidence Index
type: entity
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [OECD BCI, OECD_BCI, Business Confidence Index]
entity_kind: dataset
---

# OECD Business Confidence Index

**An OECD indicator derived from opinion surveys of firms about future production, orders, and inventories in the industrial sector; the strongest single predictor of M&A activity in the Degen et al. (2024) study.**

## Overview

The OECD Business Confidence Index (BCI) is constructed from business opinion surveys and is published monthly. It is designed to capture managerial expectations about near-term economic conditions in the industrial sector. In the MASS study, it consistently outperforms all other individual predictors of M&A deal volume, including MASS. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

The BCI's dominance is notable: in out-of-sample forecasting it achieves R²OS of 49.1%, compared to 9.4% for MASS alone. It also has strong forecast encompassing properties — it partially encompasses the information in MASS, Baker-Wurgler, Huang et al., and UM CSI. Combining OECD BCI with MASS (equal weighting) raises out-of-sample R²OS to 50.5%. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

The authors suggest the BCI's strength reflects its capture of macroeconomic cycle conditions, CEO confidence, and regulatory and political uncertainty — the broad set of fundamental M&A activity drivers identified in the merger waves literature (Harford, 2005). The paper notes that future research on BCI as a predictor across different asset classes and business decisions is warranted. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- Out-of-sample R²OS: 49.1% — far larger than all other individual predictors. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Combined EW_MASS_BCI achieves R²OS of 50.5%, confirming MASS adds incremental value. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Negatively correlated with MASS and other investor sentiment indices (cyclicality argument). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Source: OECD (2024). Business confidence index (BCI). doi: 10.1787/3092dc4f-en.

## Related

- [[mass-index]] — the complementary index that adds predictive power on top of OECD BCI
- [[baker-wurgler-sentiment-index]] — a competing benchmark in the same study
- [[merger-waves]] — the aggregate phenomenon both indices predict

## Open questions

- Why does the OECD BCI so strongly predict M&A activity? Is it a leading indicator of credit conditions, deal confidence, or both?
- Does the BCI's predictive power hold equally well in non-OECD markets?
