---
title: Support Vector Machine
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-03-zhang-et-al-2024-ai-ma-target-selection]
aliases: [SVM, Support Vector Classifier]
entity_kind: model
---

# Support Vector Machine

**A supervised learning algorithm that finds the maximum-margin hyperplane separating classes; used as one component in Zhang et al.'s (2024) hybrid M&A target-selection and synergy-prediction model.**

## Overview

Support Vector Machines (SVMs) are a family of supervised classification and regression algorithms that identify the decision boundary (hyperplane) maximising the margin between classes in high-dimensional feature spaces. They are particularly effective with mixed data types and mid-size datasets where interpretability is less critical than accuracy.


Zhang et al. (2024) also include SVM as a component in their hybrid ML model for M&A target selection and synergy prediction (alongside LightGBM and MLP), where the combination achieves AUC-ROC 0.937. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Key facts

- Used as a component in Zhang et al.'s (2024) hybrid model achieving AUC-ROC 0.937. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Related

- [[machine-learning]] — parent algorithm family
- [[ml-target-selection]] — Zhang et al. (2024) use SVM in their hybrid model

## Open questions

- Whether SVM contributes materially to the hybrid model's performance or mainly serves as a complementary classifier alongside LightGBM and MLP.
