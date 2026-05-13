---
title: Feature Engineering
type: concept
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-zhang-et-al-2024-ai-ma-target-selection]
aliases: [Feature Selection, Feature Construction]
---

# Feature Engineering

**The process of transforming raw data into informative input variables (features) that improve the predictive performance of machine learning models.**

## Summary

Feature engineering encompasses feature construction (deriving new variables from raw data), feature selection (identifying the most predictive subset), and feature transformation (normalizing, encoding, or otherwise preprocessing variables). It is widely considered the most impactful step in tabular ML pipelines.

In the Zhang et al. (2024) M&A target selection study, feature engineering was applied in two stages: (1) construction of 25 additional features (financial ratios, growth rates, market sentiment indicators) from the 61 raw CrunchBase features; (2) selection via correlation analysis, mutual information, and Recursive Feature Elimination with Cross-Validation (RFECV), reducing the final feature set to 43. Text-based features were extracted using TF-IDF vectorization from company descriptions and press releases. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

The top 10 features by importance in the resulting model are: Revenue Growth Rate (0.182), Market Cap/EBITDA (0.159), Debt-to-Equity Ratio (0.143), R&D Intensity (0.128), Industry Concentration (0.115), Geographic Overlap (0.103), Patent Portfolio Strength (0.097), Employee Productivity (0.089), Customer Base Overlap (0.082), and Market Sentiment Score (0.076). [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Variations / sub-concepts

- Recursive Feature Elimination with Cross-Validation (RFECV)
- TF-IDF text feature extraction
- Financial ratio derivation
- Missing value imputation (RANSAC Regressor, Categorical Imputer)
- Outlier treatment (IQR-based winsorization)
- Normalization (Min-Max scaling)

## Key claims across sources

- Zhang et al. (2024) derive 25 additional features from 61 raw variables, then select 43 final features using RFECV. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- TF-IDF vectorization of company descriptions and press releases is used to capture qualitative compatibility signals in a hybrid ML/NLP pipeline. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Revenue Growth Rate is the top-ranked feature (importance 0.182); R&D Intensity (0.128) and Industry Concentration (0.115) are identified as underweighted by traditional analysts. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Related

- [[ml-target-selection]] — the application where feature engineering is applied
- [[gradient-boosting]] — ML algorithm that heavily benefits from good features
- [[synergy-prediction]] — the outcome predicted using these engineered features
- [[crunchbase]] — the raw data source from which features are constructed

## Open questions

- Are the top-ranked features stable across different industries, or is feature importance sector-specific?
- How transferable are the derived financial ratio features to non-US or private-company M&A datasets?
