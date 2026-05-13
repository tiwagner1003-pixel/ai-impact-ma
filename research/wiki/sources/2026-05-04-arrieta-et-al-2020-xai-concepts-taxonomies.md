---
title: "Explainable Artificial Intelligence (XAI): Concepts, taxonomies, opportunities and challenges toward Responsible AI"
type: source
created: 2026-05-04
updated: 2026-05-04
sources: []
origin: research/input/inbox/1-s2.0-S1566253519308103-main.pdf
author: Alejandro Barredo Arrieta, Natalia Díaz-Rodríguez, Javier Del Ser, Adrien Bennetot, Siham Tabik, Alberto Barbado, Salvador Garcia, Sergio Gil-Lopez, Daniel Molina, Richard Benjamins, Raja Chatila, Francisco Herrera
date: 2020
aliases: [Arrieta et al. 2020, XAI survey 2020]
---

# Explainable Artificial Intelligence (XAI): Concepts, taxonomies, opportunities and challenges toward Responsible AI

**The most-cited survey of XAI (6,000+ citations), providing a unified conceptual framework, dual taxonomy of transparent vs. post-hoc explainability methods, and a "Responsible AI" framework requiring fairness, explainability, and accountability for large-scale AI deployment.**

## Key takeaways

- Black-box ML models — especially Deep Neural Networks — produce opaque decisions that are hard to justify, legitimate, or explain, creating adoption barriers in high-stakes domains including finance, medicine, and law.
- Explainability is a crucial feature for the practical deployment of AI models: without it, domain experts, regulators, and managers cannot appropriately trust, audit, or manage AI systems.
- The paper draws a precise terminological distinction between interpretability (passive: a model makes sense to a human by itself) and explainability (active: deliberate procedures taken to clarify a model's internal functions).
- Two main families of XAI approaches exist: (1) transparent models (interpretable by design — linear regression, decision trees, rule-based learners, GAMs, Bayesian models) and (2) post-hoc explainability techniques (LIME, SHAP, attention mechanisms, saliency maps, layer-wise relevance propagation) applied after training to opaque models.
- "Responsible AI" is the paper's culminating concept: a framework requiring that AI deployed in real organizations meet standards for fairness, model explainability, and accountability simultaneously — XAI is positioned as the core enabling pillar.
- Five distinct target audiences for XAI each have different needs: domain experts (trust, scientific knowledge), affected users (fair decisions), regulatory entities (compliance, audits), data scientists/developers (efficiency, new functionalities), and managers/board members (regulatory compliance assessment, understanding corporate AI).
- Interpretability improves model implementability for three reasons: (1) it ensures impartiality and enables bias detection; (2) it facilitates robustness testing against adversarial perturbations; (3) it guarantees that only meaningful variables infer the output — i.e., that causality-consistent variable relationships hold.

## Claims

- There is a fundamental performance-interpretability trade-off in ML: as models become more powerful (particularly Deep Neural Networks), they become more opaque, making their decisions harder for humans to examine, critique, or trust. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Interpretability is defined as a passive characteristic: the degree to which a given model makes sense to a human observer on its own, without additional procedures — also expressible as transparency. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Explainability is an active characteristic: any action or procedure taken by a model with the intent of clarifying or detailing its internal functions to a target audience. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- The paper's formal definition of an explainable AI is: "Given an audience, an explainable Artificial Intelligence is one that produces details or reasons to make its functioning clear or easy to understand." Audience is the cornerstone — what counts as sufficient explanation depends entirely on who is being explained to. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Transparent ML models — those interpretable by design — fall into three levels: simulatable (a human can mentally simulate the whole model), decomposable (each part can be individually explained), and algorithmically transparent (the full learning process is mathematically analysable). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Transparent model families include: linear/logistic regression, decision trees, K-Nearest Neighbors, rule-based learners (including fuzzy systems), Generalized Additive Models (GAMs), and Bayesian models. Tree ensembles, SVMs, multi-layer neural networks, CNNs, and RNNs all require post-hoc techniques. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Post-hoc explainability techniques are divided by method type: text explanations, visual explanations, local explanations, explanations by example, explanations by simplification (model-agnostic surrogates), and feature relevance methods (e.g., SHAP, LIME). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Nine XAI goals identified in the literature: trustworthiness, causality, transferability, informativeness, confidence, fairness, accessibility, interactivity, and privacy awareness. Trustworthiness and informativeness are the most commonly cited; causality is important for managers and regulators but less frequently operationalised. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- The finance sector is explicitly listed as one of the high-stakes domains where explainability is most critical — alongside medicine, law, autonomous systems, and defence — because black-box decisions in these domains cannot be justified, legitimated, or regulated without explanatory procedures. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Three reasons interpretability improves model implementability: (1) ensures impartiality/detects training-data bias; (2) facilitates robustness by exposing potential adversarial perturbations; (3) guarantees that only meaningful variables infer the output (causality). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Responsible AI, as defined in this paper, requires that AI models simultaneously meet standards for fairness, model explainability, accountability, transparency, privacy, ethics, and security/safety — these principles interact and cannot be addressed in isolation. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- The implementation of Responsible AI principles in organizations must balance two requirements: (1) major cultural and organizational changes to enforce such principles; (2) feasibility and compliance of implementation with existing IT assets and policies. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- The paper reviewed approximately 400 contributions to the XAI literature (Scopus data through December 2019); the number of publications on "Explainable Artificial Intelligence" rose steeply after 2017, driven in part by national government XAI research agendas (particularly DARPA's XAI programme). [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Data fusion contexts introduce additional XAI challenges: knowledge-level fusion can help discover new knowledge through complex DL model interactions, but model-level fusion (e.g., tree ensembles) makes overall models opaque even when constituent models are transparent; privacy risks arise when XAI techniques allow reverse-engineering of sensitive training data. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]

## Entities mentioned

- [[alejandro-barredo-arrieta]]
- [[natalia-diaz-rodriguez]]
- [[javier-del-ser]]
- [[information-fusion]]

## Concepts mentioned

- [[xai-explainable-ai]]
- [[black-box-problem]]
- [[post-hoc-explainability]]
- [[responsible-ai]]
- [[deep-learning]]
- [[ai-governance-in-ma]]
- [[ai-in-ma]]

## Notes

### Key quotes worth preserving

"The danger is on creating and using decisions that are not justifiable, legitimate, or that simply do not allow obtaining detailed explanations of their behaviour." (p. 83)

"Given a certain audience, explainability refers to the details and reasons a model gives to make its functioning clear or easy to understand." (p. 85 — the paper's core working definition)

"XAI will create a suite of machine learning techniques that enables human users to understand, appropriately trust, and effectively manage the emerging generation of artificially intelligent partners." (p. 84, citing D. Gunning / DARPA definition)

"A responsible implementation and use of AI methods in organizations and institutions worldwide will be only guaranteed if all these AI principles are studied jointly." (p. 108, conclusion)

### Relevance to Thema 7 (Einfluss von KI auf M&A)

This paper is foundational for the critical reflection section of the seminar paper. The core argument for the paper's Kritische Reflexion section is: high-performing ML models (the technology demonstrated by Zhang et al. 2024, Degen et al. 2024) face a structural adoption barrier in M&A because their black-box nature prevents justification, auditability, and regulatory compliance. Arrieta et al. (2020) provides the academic grounding for why this barrier is not merely perceptual but structural, and what methods (XAI) exist to address it.

Specific connections to existing sources:
- [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]] already flagged model interpretability as a practitioner adoption barrier — Arrieta et al. (2020) provides the theoretical underpinning for that observation.
- [[2026-05-04-bremen-2024-ai-accelerates-ma]] and [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]] both reference trust and governance concerns — Arrieta et al. (2020) provides the Responsible AI framework that explains why trust requires XAI.
- [[2026-05-04-singh-2023-ai-transformative-potential-ma]] argues AI must complement (not replace) human judgment — the XAI literature supports this by showing explainability is precisely the mechanism through which human oversight is preserved.

### Open questions / future reading

- GDPR's Article 22 creates a "right to explanation" for automated decision-making affecting individuals — does M&A deal-making (targeting a company, not a person) trigger this right? The paper cites this regulatory pressure but does not resolve the M&A case specifically.
- DARPA's XAI programme (Gunning 2017) is cited as a key driver — worth checking if any M&A-specific XAI applications have been funded or published under this programme.
- The paper identifies finance (alongside medicine/law) as a high-stakes XAI domain but does not discuss M&A specifically — a gap the Thema 7 paper can explicitly address.
- SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-agnostic Explanations) are the two most prominent post-hoc XAI methods referenced — both are directly applicable to the Zhang et al. (2024) LightGBM model, which could be explainability-augmented.

### Citation note

Full citation (Harvard style): Arrieta, A.B., Díaz-Rodríguez, N., Del Ser, J., Bennetot, A., Tabik, S., Barbado, A., Garcia, S., Gil-Lopez, S., Molina, D., Benjamins, R., Chatila, R. and Herrera, F. (2020) 'Explainable Artificial Intelligence (XAI): Concepts, taxonomies, opportunities and challenges toward responsible AI', *Information Fusion*, 58, pp. 82–115. doi:10.1016/j.inffus.2019.12.012.

Published in *Information Fusion*, Vol. 58 (2020), pp. 82–115 (Elsevier). Received 22 October 2019; accepted 25 December 2019; available online 26 December 2019. DOI: https://doi.org/10.1016/j.inffus.2019.12.012. Citation count: 6,000+ (as of early 2026).
