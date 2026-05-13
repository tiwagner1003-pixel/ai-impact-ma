---
title: Due Diligence Quality
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-howson-2003-due-diligence-critical-stage, 2026-05-07-bhagwan-et-al-2018-systematic-review-dd-ma, 2026-05-07-puranam-et-al-2006-dd-signal-detection, 2026-05-07-hendrycks-et-al-2021-cuad-contract-review, 2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [DD quality, quality of due diligence, due diligence effectiveness]
---

# Due Diligence Quality

**The degree to which a DD process discovers relevant risks, interprets them correctly, and translates findings into deal decisions, negotiation terms, pricing, and post-deal planning.**

## Summary

For the DD-focused seminar paper, quality should be operationalized more narrowly than "better deal outcome." The literature supports a multi-dimensional view: completeness/recall, precision, consistency, decision relevance, explainability, and process coverage. Bhagwan et al. (2018) show DD is multidisciplinary and process-driven, while Puranam et al. (2006) show DD can fail even when negative information is discovered if decision makers do not interpret or act on it correctly. [[2026-05-07-bhagwan-et-al-2018-systematic-review-dd-ma]] [[2026-05-07-puranam-et-al-2006-dd-signal-detection]]

In AI-supported Legal DD, quality often becomes a retrieval metric problem: high recall is crucial because missed clauses can carry large deal risk. CUAD and Dwivedi & Kamps (2025) both support the view that contract review is a high-recall, sparse-label, "needle-in-a-haystack" task, where false negatives matter strongly and labeled expert data is a bottleneck. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]] [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Variations / sub-concepts

- Recall / completeness
- Precision
- Decision relevance
- Explainability / auditability
- Process coverage across DD areas
- [[due-diligence-signal-detection]]
- [[legal-contract-review]]

## Key claims across sources

- DD quality is undermined by adviser silos: lawyers, accountants, and management consultants each cover only their own domain; unclear mandates and weak reporting lines can cause identified risks to disappear before they reach the buyer's decision process. [[2026-05-07-howson-2003-due-diligence-critical-stage]]
- Cost pressure is a quality risk in classical DD: choosing advisers on fee minimisation rather than reputation and experience can produce a report worse than useless. [[2026-05-07-howson-2003-due-diligence-critical-stage]]
- DD quality includes process control and monitoring, because DD teams are increasingly asked to judge whether target value can be realised, whether timelines are achievable, and whether risks can be managed. [[2026-05-07-bhagwan-et-al-2018-systematic-review-dd-ma]]
- DD quality can fail at the interpretation stage: acquirers may discover negative information but fail to revise bids or withdraw. [[2026-05-07-puranam-et-al-2006-dd-signal-detection]]
- High recall is especially important in legal DD because relevant clauses or risks are sparse but costly to miss. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Contract-review AI still has substantial room for improvement even with expert-annotated datasets such as CUAD. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]

## Related

- [[due-diligence]]
- [[classical-due-diligence-process]]
- [[legal-contract-review]]
- [[due-diligence-signal-detection]]
- [[automation-bias]]

## Open questions

- Which quality metrics can realistically be measured in a seminar paper without primary data?
- How should precision/recall evidence from Legal DD be translated cautiously to broader DD areas such as cultural, operational, or commercial DD?
