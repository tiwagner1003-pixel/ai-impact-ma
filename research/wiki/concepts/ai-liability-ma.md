---
title: AI Liability in M&A
type: concept
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]
aliases: [AI Risk Allocation M&A, Liability for AI in Mergers and Acquisitions, AI-Haftung M&A]
---

# AI Liability in M&A

**The distribution of legal responsibility across tool providers, service providers (e.g., law firms), boards of directors, and shareholders when erroneous AI output causes harm or leads to an undesirable M&A transaction.**

## Summary

As AI tools become standard in M&A due diligence, the question of who bears the legal and financial consequences of AI errors has emerged as a critical governance issue. Herbosch and Mertens (2025) provide the most comprehensive comparative analysis to date, distinguishing two tracks: external liability (tool providers and service providers vis-à-vis the acquirer) and internal liability (board of directors vis-à-vis the company and its shareholders). [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

On the external track, the core insight is that AI's inherent imperfection means erroneous output does not in itself establish provider negligence. The decisive questions are whether the tool met contractually agreed performance standards, and whether — absent explicit standards — it was fit for its intended use. Service providers such as law firms must select AI tools with reasonable care, ensure adequate training, and maintain supervision; they cannot contractually disclaim the obligation to exercise some degree of oversight. The EU AI Act's standards for high-risk systems serve as an informal benchmark even where not strictly applicable. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

On the validity-of-contract track, the mistake doctrine can theoretically enable a buyer to annul an M&A agreement concluded on the basis of erroneous AI output, but only if the mistake was "excusable" (a contextual, subjective assessment), related to an essential contractual element (not mere value), and was not contractually allocated to the buyer through representations and warranties or risk allocation clauses. Sellers who deliberately deploy subpar AI tools to mislead buyers face a lower bar for the buyer to invoke fraudulent misrepresentation. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

On the internal track, boards face liability exposure measured against their informational duty of care — the obligation to base business decisions on a reasonably accurate, cross-verified information basis. The standard varies by jurisdiction (see [[business-judgment-rule]]), but across all five jurisdictions analyzed the board cannot blindly rely on AI output for economically significant decisions. Key protective measures are: (a) careful selection and testing of the AI system; (b) cross-verification of AI output against other sources for major decisions; and (c) use of explainable AI models where cost-efficient. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

The overall risk distribution conclusion is that shareholders of acquiring companies bear the residual risk from AI-related M&A errors, because contractual terms typically burden the buyer's claims against providers, and business judgment protections (especially in Delaware) shield boards from most shareholder liability suits arising from AI reliance. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

## Variations / sub-concepts

- Tool provider liability — contractual performance standards and fitness-for-use
- Service provider (deployer) liability — duty of best efforts, tool selection, supervision
- Contract validity challenges — mistake doctrine, fraudulent misrepresentation
- Board internal liability — duty of care, informational duty, business judgment rule
- Shareholder residual risk — the default risk-bearer when other liability claims fail
- Contractual risk allocation clauses — reps and warranties, liability limitations, indemnities

## Key claims across sources

- The inherent imperfection of AI means that erroneous output does not constitute provider negligence per se; liability hinges on whether contractually agreed performance standards were met or, absent explicit standards, whether the tool was fit for its intended use. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- Service providers (law firms, consultants) deploying AI tools for M&A clients cannot contractually exclude the obligation to exercise supervision, even if AI use is disclosed; the minimum duty of care for the service relationship persists. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- The mistake doctrine is the key external legal mechanism for challenging M&A contract validity when AI produces erroneous output; German law is notably more permissive (no excusability requirement) than French, Belgian, English, and US law. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- Sellers using AI chatbots or information tools to communicate with prospective buyers can face fraudulent misrepresentation claims if the AI tool was knowingly subpar or designed to mislead — this is a dual liability scenario identified as particularly concerning. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- Explainability is a legal safeguard for both external service providers (enables supervision to spot obvious errors) and internal board members (enables the plausibility review required under the German Ision-doctrine and defensible decision records in Delaware). [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- Shareholders are the ultimate residual risk-bearers for AI-related M&A errors; they have limited practical tools to prevent this ex ante, as they generally lack direct say over how AI is used in the deal process. [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]

## Related

- [[ai-governance-in-ma]] — the governance framework that minimizes liability exposure
- [[business-judgment-rule]] — the judicial doctrine governing internal board liability
- [[responsible-ai]] — the broader normative framework; compliance reduces liability risk
- [[xai-explainable-ai]] — explainability is a central legal safeguard in both external and internal liability tracks
- [[due-diligence]] — the primary M&A phase where AI liability exposure materializes
- [[information-asymmetry]] — the structural condition that AI tools aim to reduce but can also create (via seller-provided information)
- [[maarten-herbosch]] — primary source author
- [[floris-mertens]] — primary source author
- [[eu-ai-act]] — referenced as benchmark even for low-risk AI systems in M&A contexts

## Open questions

- Are there any decided court cases (in any of the five jurisdictions) where an M&A party sought to annul a deal on grounds of erroneous AI output? (No known cases as of 2025.)
- How will standard M&A representations and warranties provisions evolve to address AI-generated due diligence findings specifically?
- Does the EU AI Liability Directive (proposed) change the burden-of-proof analysis for AI errors in M&A relative to the current regime?
- Is there a practical threshold of AI reliance (e.g., sole information source vs. one of many) at which liability risk qualitatively increases?
