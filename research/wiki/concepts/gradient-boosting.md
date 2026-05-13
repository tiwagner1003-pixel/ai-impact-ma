---
title: Gradient Boosting
type: concept
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-zhang-et-al-2024-ai-ma-target-selection, 2026-05-04-bozman-et-al-2026-ai-deal-screening]
aliases: [Gradient Boosted Trees, GBT, GBDT, Gradient Boosted Decision Trees]
---

# Gradient Boosting

**An ensemble machine learning technique that builds a strong predictive model by sequentially adding weak learners (typically decision trees) where each new learner corrects the errors of the previous ones.**

## Summary

Gradient boosting is one of the most effective algorithms for supervised learning on tabular (structured) data. It minimizes a differentiable loss function by iteratively fitting new trees to the residual errors of the current ensemble. Major implementations include XGBoost, LightGBM, and CatBoost — all competing on speed, memory efficiency, and categorical data handling.

In the M&A domain, Zhang et al. (2024) use [[lightgbm]] as the gradient boosting component of a hybrid M&A synergy prediction model, combined with SVM and MLP neural networks. The ensemble's gradient boosting component is valued for handling large datasets and non-linear feature interactions. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Variations / sub-concepts

- [[lightgbm]] — Microsoft's leaf-wise gradient boosting library
- XGBoost — level-wise gradient boosting (cited as alternative in Zhang et al.)
- CatBoost — gradient boosting with native categorical feature support

## Key claims across sources

- LightGBM (gradient boosting) is used as one of three components in the Zhang et al. (2024) hybrid M&A target selection model, with parameters num_leaves: 31, learning_rate: 0.05, n_estimators: 100. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Gradient boosting models are noted for particular promise in identifying patterns of successful M&A combinations and ranking potential targets; XGBoost and LightGBM are specifically cited. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Gradient Boosting is one of four algorithms in the Bozman et al. (2026) ML ensemble (alongside Ridge, Lasso, Random Forest) for predicting acquirer announcement returns; the ensemble's median prediction is used as the final forecast. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- In the Bozman et al. gradient-boosted model, the three most important features are Public Target status, Relative Size, and Total Assets; interaction terms account for over two-thirds of the impact of Public Target and more than 1.5x the main effect of Relative Size. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]

## Related

- [[lightgbm]] — the specific gradient boosting tool used in Zhang et al.
- [[ml-target-selection]] — the application context
- [[feature-engineering]] — gradient boosting models benefit from careful feature construction

## Open questions

- How does gradient boosting compare to deep learning (MLP, transformers) on M&A tabular data when sample size is increased beyond 10,000 deals?
