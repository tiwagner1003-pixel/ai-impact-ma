---
title: Explainable Artificial Intelligence (XAI)
type: concept
created: 2026-05-04
updated: 2026-05-07
sources: [2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies, 2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]
aliases: [XAI, Explainable AI, Model Explainability, Explainability]
---

# Explainable Artificial Intelligence (XAI)

**A field of AI research and practice concerned with creating ML models whose decisions can be made understandable, auditable, and justifiable to specific human audiences — defined formally as: given a certain audience, an explainable AI is one that produces details or reasons to make its functioning clear or easy to understand.**

## Summary

XAI emerged as a distinct research area in response to the widespread adoption of high-performance but opaque ML models — particularly Deep Neural Networks — in consequential decision-making contexts. While these models achieve state-of-the-art predictive accuracy, their internal workings are not legible to humans, creating a structural barrier to deployment in domains where decisions must be justified, audited, or legally defended. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

The key conceptual contribution of the field is the distinction between two properties: interpretability (a passive characteristic — the model makes sense by itself) and explainability (an active characteristic — deliberate procedures are applied to clarify a model's functioning for a target audience). This distinction is practically important because it separates model design choices from post-deployment explanation tooling. The cornerstone concept is **audience**: what counts as a sufficient explanation depends entirely on who needs to understand the model and why. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

The literature recognises five main target audience profiles for XAI: (1) domain experts and users of the model (need to trust the model and gain scientific knowledge); (2) users affected by model decisions (need to understand their situation and verify fairness); (3) regulatory entities and agencies (need to certify compliance with legislation); (4) data scientists, developers, and product owners (need to ensure/improve efficiency and research new functionalities); and (5) managers and executive board members (need to assess regulatory compliance and understand corporate AI applications). Each audience has a different explainability requirement. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

XAI publications grew steeply after 2017, driven by national research agendas (especially the US DARPA XAI programme) and regulatory pressure from frameworks such as the EU GDPR's right-to-explanation provisions. Finance, medicine, law, and defence are consistently identified as the highest-priority deployment domains. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

## Variations / sub-concepts

- [[black-box-problem]] — the core problem XAI addresses: opaque models that cannot be explained
- [[post-hoc-explainability]] — XAI techniques applied after training to explain otherwise opaque models
- [[responsible-ai]] — the broader framework that treats XAI as one of several required AI principles
- Transparent models — models interpretable by design (linear regression, decision trees, rule-based learners, GAMs, Bayesian models)
- LIME (Local Interpretable Model-agnostic Explanations) — a widely used post-hoc local explanation technique
- SHAP (SHapley Additive exPlanations) — a post-hoc feature-relevance method grounded in game theory
- Attention mechanisms — in Transformer/DNN architectures, weighted attention can serve as a partial explanation
- Saliency maps / layer-wise relevance propagation (LRP) — visualization methods for explaining DNN decisions on images

## Key claims across sources

- Interpretability is a passive characteristic: the degree to which a model makes sense to a human on its own; explainability is an active characteristic: deliberate procedures taken to clarify internal model functions. The two concepts are related but distinct — not synonyms. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Audience is the cornerstone of XAI: the same model may be "explainable enough" for one audience (e.g., data scientists) and "not explainable" for another (e.g., a regulator or affected user). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Finance is explicitly identified as a high-stakes XAI domain alongside medicine and law — black-box AI decisions in financial contexts cannot be justified, legitimated, or regulated without explanatory procedures. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Model interpretability improves implementability for three reasons: (1) enables bias detection and impartiality; (2) facilitates robustness testing against adversarial inputs; (3) ensures only meaningful variables infer the output (causality preservation). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- There is a fundamental performance-interpretability trade-off: more powerful models (DNNs) tend to be less interpretable; this trade-off, rather than pure accuracy, should be the primary design criterion when deploying ML in high-stakes contexts. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Model interpretability / explainability is flagged as a key barrier to practitioner adoption of AI tools in M&A — even high-performing models face skepticism without transparent reasoning for their recommendations. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Explainability serves three regulatory goods simultaneously in the context of ADM credit systems: (1) building trust between algorithm and affected user; (2) providing visibility over unknown model flaws; and (3) enabling performance and control improvements by allowing questioning of the validity of decision-making. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Without explainability, existing antidiscrimination law (ECOA, Fair Housing Act) cannot be practically enforced against biased ADM platforms — explainability is a legal enforcement prerequisite, not only a technical preference. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- The ACM's principle that institutions using ADM should "produce explanations regarding both the procedures followed by the algorithm and the specific decisions that are made" provides a concrete institutional standard for XAI requirements in regulated industries. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

## XAI taxonomy (Arrieta et al. 2020)

**Taxonomy 1: By model transparency**

| Model type | Transparency level |
|---|---|
| Linear/Logistic Regression | Simulatable, decomposable, algorithmically transparent |
| Decision Trees | Simulatable to decomposable (depending on size) |
| K-Nearest Neighbors | Simulatable (if features/K manageable) |
| Rule-based Learners (incl. fuzzy) | Decomposable to algorithmically transparent |
| Generalized Additive Models (GAMs) | Decomposable |
| Bayesian Models | Simulatable to decomposable |
| Tree Ensembles (Random Forests, XGBoost, LightGBM) | Not transparent — require post-hoc |
| Support Vector Machines | Not transparent — require post-hoc |
| Multi-layer Neural Networks / DNNs / CNNs / RNNs | Not transparent — require post-hoc |

**Taxonomy 2: Post-hoc technique types**

- Text explanations — symbolic/rule representations of model behaviour
- Visual explanations — visualizations of model decisions (e.g., saliency maps, heat maps)
- Local explanations — explanations of individual predictions (e.g., LIME, SHAP)
- Explanations by example — representative training instances that explain predictions
- Explanations by simplification — surrogate/distilled models (e.g., LIME globally)
- Feature relevance — quantifying each variable's contribution to the output (e.g., SHAP)

## Related

- [[black-box-problem]] — the core problem motivating XAI
- [[post-hoc-explainability]] — the main technical toolbox of XAI
- [[responsible-ai]] — XAI is positioned as the core pillar of Responsible AI
- [[deep-learning]] — the model family most in need of XAI, due to its opacity
- [[ai-governance-in-ma]] — governance frameworks must incorporate XAI requirements
- [[ai-in-ma]] — XAI is the critical adoption barrier for ML models in M&A
- [[ml-target-selection]] — ML models for M&A target selection (e.g., LightGBM) require post-hoc XAI
- [[gradient-boosting]] — tree ensemble methods (LightGBM, XGBoost) are high-performing but not transparent by design

## Open questions

- Does GDPR's right-to-explanation (Article 22) apply to M&A target selection or valuation decisions, where the "affected subject" is a target company, not an individual?
- Which post-hoc XAI method (SHAP, LIME, or attention) is most appropriate for explaining LightGBM-based M&A synergy prediction models to M&A practitioners (non-technical audience)?
- Is there empirical evidence that adopting XAI methods in finance/M&A actually increases practitioner adoption rates, or does interpretability remain under-valued relative to accuracy?
- How does the EU AI Act (2024) — which explicitly regulates high-risk AI systems — interact with AI tools used in M&A due diligence and target selection?
- Johnson et al. (2019) argue that explainability requirements are a necessary but not sufficient governance tool — regulators also need institutional capacity to audit outcomes and enforce disparate-impact norms. Does the XAI literature address this enforcement dimension, or does it treat explainability as an end in itself?
