---
title: Automated Decision-Making
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]
aliases: [ADM, Automated Decision Making, Algorithmic Decision-Making]
---

# Automated Decision-Making

**The use of algorithmic or AI-based systems to make or substantially inform consequential decisions — such as creditworthiness assessments, loan pricing, or screening — with reduced or no direct human deliberation in each individual decision.**

## Summary

Automated decision-making (ADM) platforms are the operational manifestation of machine learning and AI in consumer finance. Fintech advocates celebrate ADM because computer systems cannot, in themselves, hold the mental processes (conscious or unconscious bias) associated with human discriminatory decisions — arguing ADM platforms therefore mitigate discrimination against legally protected groups. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

Johnson et al. (2019) challenge this framing directly: ADM does not eliminate discrimination but shifts its locus. Bias migrates from the human decision-maker to: (1) the inputs (training data encoding historical discrimination), (2) the training and programming stage (developer choices about features and model architecture), and (3) the model's own pattern recognition (proxy discrimination). The paper identifies three stages in the development process of ADM platforms where programmers may unintentionally incorporate bias: inputs, training, and programming. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

A further concern is that ADM is oriented to outcomes, not process. The machine's "intelligence" is calibrated to reach consistently accurate results on a chosen task — it does not "reason" in a human sense. This leaves ADM platforms vulnerable to pursuing forms of analysis that an experienced finance professional would set aside as suspect but that achieve good short-term predictive scores by exploiting spurious correlations or socioeconomic proxies. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

In M&A contexts, ADM relevance extends beyond credit scoring: algorithmic tools increasingly underpin target identification (deal screening models), valuation models, and due-diligence document review. The same structural bias risks that Johnson et al. identify in consumer credit apply wherever ADM platforms process historically biased datasets or incorporate alternative data with demographic correlates.

## Variations / sub-concepts

- Creditworthiness ADM — automated credit scoring and loan underwriting (the primary focus of Johnson et al. 2019)
- Behavioral scoring — ADM using behavioral analytics (browsing, shopping, social media) to infer creditworthiness
- [[ml-target-selection]] — ADM applied to M&A deal sourcing and target ranking
- [[algorithmic-bias]] — the structural bias risks inherent in ADM design and deployment
- [[disparate-impact]] — the legal doctrine under which ADM outputs are challengeable

## Key claims across sources

- ADM platforms may shift, rather than eliminate, discrimination: bias moves from the human decision-maker to biased training data and developer feature choices. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- ADM is oriented to outcomes, not process — leaving it vulnerable to pursuing analyses that experienced professionals would reject as suspect but that achieve high predictive accuracy through spurious correlations. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Fintech firms increasingly describe creditworthiness decisions as behavioral scoring, using big-data profiling to detect patterns in consumers' daily lives and predict behavior. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- The three stages of ADM development where bias is most likely to be unintentionally incorporated are: inputs, training, and programming. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

## Related

- [[algorithmic-bias]] — the primary risk produced by ADM in consequential decision contexts
- [[black-box-problem]] — ADM opacity is the structural barrier to detecting and correcting bias
- [[xai-explainable-ai]] — explainability requirements are the primary technical governance tool for ADM
- [[machine-learning]] — the underlying technology enabling ADM
- [[fintech-regulation]] — the regulatory context governing ADM in credit markets
- [[disparate-impact]] — the legal doctrine under which biased ADM outputs are challengeable
- [[ml-target-selection]] — ADM applied to M&A deal-screening contexts
- [[responsible-ai]] — the overarching governance framework requiring fairness and accountability in ADM

## Open questions

- At what threshold of human oversight does an "automated" decision become sufficiently human-supervised to escape the structural bias risks that Johnson et al. identify?
- How should ADM governance in M&A deal screening differ from ADM governance in consumer credit — given that M&A counterparties are sophisticated actors rather than individual consumers?
