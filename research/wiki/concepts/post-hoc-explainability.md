---
title: Post-Hoc Explainability
type: concept
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]
aliases: [Post-Hoc XAI, Post-Hoc Interpretation, Model-Agnostic Explainability]
---

# Post-Hoc Explainability

**A family of XAI techniques applied after a model has been trained, providing explanations for the predictions of otherwise opaque (black-box) models without modifying the underlying model architecture.**

## Summary

Post-hoc explainability is one of the two main branches of the XAI taxonomy (the other being transparent-by-design models). It targets models that are not interpretable on their own — such as Deep Neural Networks, tree ensembles (Random Forests, LightGBM, XGBoost), and Support Vector Machines — and applies external tools to produce explanations of their outputs. The key property is that the model itself remains unchanged; only the explanation layer is added. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

The practical importance of post-hoc methods is that they allow practitioners to retain the performance benefits of state-of-the-art black-box models while adding a layer of explanatory accountability. This is the standard approach when a high-performing model must be deployed in a context (finance, medicine, law) where decisions must be justifiable to regulators, users, or boards. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

Post-hoc techniques differ along several dimensions: they can be model-agnostic (applicable to any model) or model-specific (designed for a particular architecture); they can be global (explaining the overall model behaviour) or local (explaining individual predictions); and they can target different output formats (text rules, visualizations, importance scores). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

## Variations / sub-concepts

The Arrieta et al. (2020) taxonomy identifies six post-hoc explanation technique types:

- **Text explanations** — generate symbolic or rule-based representations of what the model learned; includes rule-extraction methods that produce readable IF-THEN logic from trained neural networks or tree ensembles.
- **Visual explanations** — visualize model decisions; particularly developed for image-processing DNNs (saliency maps, heat maps, Grad-CAM); can also include dimensionality-reduction visualizations of model decision boundaries.
- **Local explanations** — explain individual predictions by identifying the features most responsible for a specific output; LIME (Local Interpretable Model-agnostic Explanations) is the primary example, fitting a simple interpretable model in the local neighbourhood of the prediction.
- **Explanations by example** — identify representative training examples that best characterise a model's behaviour or a given prediction; prototype and criticisms methods; counterfactual examples.
- **Explanations by simplification** — build a globally simpler surrogate model that approximates the black-box model's behaviour while being interpretable; includes model distillation and knowledge distillation approaches.
- **Feature relevance** — quantify the contribution of each input variable to the model's output; SHAP (SHapley Additive exPlanations), LIME feature importance, and sensitivity analysis are the primary methods; these scores allow ranking of input variables by importance.

## Key claims across sources

- Post-hoc explainability is a broader concept than interpretability by design: a model can be explained post-hoc even if it is not interpretable on its own, but a model that is interpretable by design also meets the requirements of explainability if its audience can understand it directly. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- LIME and SHAP are the two most widely deployed post-hoc model-agnostic techniques; both are directly applicable to gradient boosting models (LightGBM, XGBoost) of the type used in M&A synergy prediction by Zhang et al. (2024). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Feature relevance methods (SHAP) are particularly valuable for managers and board members who need to understand which variables drive a model's recommendation — they produce a ranked importance list without requiring mathematical training. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- In Deep Learning specifically, attention mechanisms in Transformer architectures can serve as a form of built-in post-hoc visualization — though the paper notes debate about whether attention truly equals explanation. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- The availability of post-hoc explainability tools does not automatically solve the adoption problem: the quality of an explanation is always relative to the audience, and the same SHAP plot may satisfy a data scientist but not a regulator or an M&A practitioner. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

## Related

- [[xai-explainable-ai]] — the parent field; post-hoc explainability is one of its two main branches
- [[black-box-problem]] — the problem post-hoc techniques are designed to address
- [[deep-learning]] — the model family most commonly targeted by post-hoc XAI
- [[gradient-boosting]] — tree ensembles (LightGBM, XGBoost) commonly explained via SHAP/LIME
- [[ml-target-selection]] — M&A synergy prediction models (LightGBM) are candidates for post-hoc SHAP explanation
- [[responsible-ai]] — post-hoc explainability is the practical implementation layer for Responsible AI

## Open questions

- Is post-hoc explainability sufficient for regulatory compliance (EU AI Act, GDPR), or do high-risk contexts require transparent-by-design models?
- In the M&A context, which post-hoc technique best serves each of the five XAI audience profiles (domain expert, affected user, regulator, developer, manager)?
- Does adding post-hoc explanation to a high-performing M&A ML model change practitioner decision-making, or do practitioners override model recommendations regardless of explanation quality?
