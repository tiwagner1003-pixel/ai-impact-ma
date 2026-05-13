---
title: Business Judgment Rule
type: concept
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]
aliases: [BJR, Business Judgment Doctrine, Geschäftsführerhaftung, Unternehmensermessen]
---

# Business Judgment Rule

**A judicial doctrine that limits courts' willingness to second-guess good-faith business decisions by boards of directors, shielding them from personal liability for errors of judgment provided they acted on an informed basis, in good faith, and in the honest belief that the action was in the company's best interest.**

## Summary

The business judgment rule originates in Delaware corporate law, where it operates as a presumption: when a board makes a business decision, the courts presume the directors acted on an informed basis, in good faith, and in the honest belief that the action was in the company's best interest. Plaintiff shareholders must rebut this presumption by showing gross negligence; if they fail, courts will not interfere even if the decision turned out poorly. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

In the AI context, the Delaware rule is relatively board-friendly: the decision to rely on an AI tool — including its selection, training, and supervision — is itself a business judgment. Gross negligence in AI use (e.g., reckless selection of a non-explainable tool when an equally accurate explainable alternative was available) must be proven by the plaintiff. This places directors in a comfortable position to experiment with AI advisory systems. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

Germany applies a version of the business judgment rule under § 93 AktG (the Bundesgerichtshof's ARAG v. Garmenbeck decision), but without the Delaware presumption: the board must affirmatively demonstrate that its decision rested on an appropriately informed basis and involved no irresponsible risks. When AI was the primary information source, the board must show that the AI system was properly selected, tested, and supervised. The German Ision-doctrine further requires a plausibility review of expert/AI output for high-stakes decisions. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

Belgium and the Netherlands apply "marginal review" rather than a full business judgment rule. Courts can review the substance of decisions, albeit cautiously. Crucially, the procedure leading to a decision — including its AI information basis — is subject to full judicial review, providing less structural protection for boards in those jurisdictions than in Delaware or Germany. The United Kingdom lacks a formal business judgment rule but courts traditionally refrain from second-guessing bona fide commercial decisions; empirical evidence suggests British courts are increasingly willing to review process. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

## Variations / sub-concepts

- Delaware business judgment rule — presumption of care; gross negligence standard
- German business judgment rule (§ 93 AktG / ARAG-Garmenbeck) — no presumption; board must prove informed basis and absence of irresponsible risk
- Ision-doctrine (Germany) — plausibility review requirement for reliance on expert/AI advice
- "Proper reliance" doctrine (Delaware / Germany) — protects directors from liability when relying on AI output in good faith, analogous to reliance on human expert advice
- Marginal review / "marginale toetsing" (Belgium, Netherlands) — courts can review substance cautiously; no reversal of burden of proof
- Entire fairness review (Delaware) — heightened review if gross negligence is proven; board must show fairness of price and process
- Corwin cleansing (Delaware) — a priori shareholder approval can eliminate entire fairness review
- "Enhanced scrutiny" (Delaware, Revlon context) — applies when board maximizes sale price in change-of-control transactions

## Key claims across sources

- Delaware law presumes board AI use complies with procedural due care; shareholders must prove gross negligence to rebut this, placing AI-related liability risk far from boards. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- German law requires boards to affirmatively demonstrate that AI was selected, tested, and supervised appropriately — a stricter burden; a board that cannot show proper AI use cannot invoke the German business judgment rule. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- The Smith v. Van Gorkom precedent established that board reliance on uninformed or inadequately investigated business data — including AI output — can constitute gross negligence and defeat the business judgment rule's protection. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- Deploying an unexplainable AI model when an equally accurate explainable alternative was available — and no other information sources were cross-checked — is the clearest pathway to a gross negligence finding under Delaware law for AI-related M&A decisions. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- Belgian and Netherlands courts can review the substance of AI-reliant board decisions, even if cautiously, because no equivalent to the Delaware presumption exists — this makes board liability more accessible to shareholders in those jurisdictions. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

## Related

- [[ai-governance-in-ma]] — the governance framework through which boards operationalize business judgment rule compliance
- [[ai-liability-ma]] — the broader liability framework in which the BJR is one doctrine
- [[responsible-ai]] — Responsible AI principles (explainability, accountability) map onto the informational standards the BJR requires
- [[xai-explainable-ai]] — explainability is a key enabler of meeting the informational duty underpinning the BJR
- [[due-diligence]] — the M&A phase where AI reliance and board informational duties interact most directly
- [[maarten-herbosch]] — primary source for comparative BJR analysis applied to AI
- [[floris-mertens]] — co-author of the comparative BJR analysis

## Open questions

- Have any Delaware courts expressly ruled on AI-based informational adequacy as a business judgment rule question? (No cases as of 2025.)
- Would a board's disclosure in its proxy statement that AI was used in due diligence satisfy any "transparency" component of the BJR's informed-basis requirement?
- Does the EU AI Act's Article 14 (human oversight for high-risk AI) functionally replicate the BJR's plausibility review requirement for companies operating in EU jurisdictions?
