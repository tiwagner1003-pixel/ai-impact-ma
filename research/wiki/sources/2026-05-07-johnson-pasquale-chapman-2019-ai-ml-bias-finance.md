---
title: "Artificial Intelligence, Machine Learning, and Bias in Finance: Toward Responsible Innovation"
type: source
created: 2026-05-07
updated: 2026-05-07
sources: []
origin: research/input/papers/johnson-pasquale-chapman-2019-ai-ml-bias-finance-fordham.pdf
author: Kristin Johnson, Frank Pasquale, Jennifer Chapman
date: 2019
aliases: [Johnson Pasquale Chapman 2019, AI ML Bias Finance Fordham]
---

# Artificial Intelligence, Machine Learning, and Bias in Finance: Toward Responsible Innovation

**A legal-academic essay arguing that algorithmic bias in fintech credit markets is structurally produced by biased training data and proxy variables, that the OCC's 2018 Fintech Charter Decision removes the state-level consumer-protection safeguards most likely to catch and correct such bias, and that coordinated state-federal regulation requiring algorithmic transparency and explainability is the only credible remedy.**

## Key takeaways

- Automated decision-making (ADM) platforms do not eliminate discrimination; they shift its locus from human bias to biased training data, flawed feature selection, and proxy variables that reproduce discrimination against legally protected groups — even when developers explicitly program the algorithm not to discriminate on a protected trait.
- The OCC's 2018 Fintech Charter Decision allows nondepository fintech firms to apply for Special Purpose National Bank (SPNB) charters, preempting state consumer-protection and antidiscrimination laws that have historically served as the primary defense for low-income and minority borrowers.
- Explainable AI is framed not merely as a technical preference but as a regulatory necessity: without algorithmic transparency and auditability, existing federal discrimination laws (Equal Credit Opportunity Act, Fair Housing Act) cannot practically be enforced against ADM platforms.
- The authors argue the appropriate regulatory response is not simply "fixing" black-box AI, but coordinated state-federal oversight establishing a uniform floor of consumer-protection standards — and in some instances a strict ban on algorithmic use in consumer credit markets.
- Credit-scoring algorithms incorporating alternative data (social media, shopping patterns, internet browsing) risk encoding socioeconomic proxies for race and gender in ways that are structurally harder to detect and challenge than overt human discrimination.
- Federal preemption by the OCC undermines state financial regulators and attorneys general — who are often the first and most nimble enforcers of consumer-protection norms — as algorithm-driven fintech markets evolve.

## Claims

- ADM platforms may shift, rather than eliminate, discrimination: bias moves from the bank manager's human judgment to the programmer's training set and the data scientist's feature choices. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- A learning algorithm may independently identify a facially neutral attribute as a proxy for a legally protected trait and execute discriminatory results — even when the developer explicitly programmed it not to discriminate on that protected trait. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- AI/ML systems can aggregate data and analyze information gathered through image or voice data that reflects unconscious bias; disparate impacts are a major concern even for facially neutral algorithmic systems. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Data mining systems "are capable of reproducing the biases created by human decisions" because the data inputted into the computer has been simplified to teach the computer to learn by example — often a flawed example. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- A 2004 NASPIRG study found 79 percent of consumer credit reports contained errors; 25 percent contained significant errors resulting in denial of credit — building these errors into ADM systems will amplify inaccuracy and entrench it into automated systems that are faster, more ubiquitous, and nearly impossible to correct. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Alternative data sources used by fintech firms for credit scoring (social media activity, shopping patterns, browsing history) introduce socioeconomic proxies for race, gender, and geography that are structurally harder to detect than explicit protected-characteristic use. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- The OCC's 2018 Fintech Charter Decision is the first attempt in the agency's 140-year history to regulate nondepository institutions as "banks," enabling fintech firms holding SPNB charters to escape state interest-rate caps, usury laws, antidiscrimination statutes, and registration and licensing fees. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Fintech firms operating as money transmitters and payday lenders historically subject to state (not federal) regulation may, with SPNB charters, preempt state consumer-protection laws that "save billions of dollars each year in predatory payday loan fees." [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Explainable AI builds trust, provides visibility over unknown model flaws, and enables performance and control improvements — the authors cite the ACM principle that institutions using ADM "produce explanations regarding both the procedures followed by the algorithm and the specific decisions that are made." [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Explainability enables three regulatory goods simultaneously: (1) greater trust between algorithm and user; (2) visibility over unknown flaws; and (3) improved model performance and control through the ability to question the validity of decision-making. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Coordinated state-federal regulation — preserving the power of state attorneys general alongside CFPB oversight — is required to establish a uniform consumer-protection floor; OCC preemption of state oversight leaves this floor without enforcement. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Regulators should evaluate the use of machine-learning algorithms in consumer credit markets and establish formal rules that limit or, in some instances, strictly ban the use of algorithms where bias risks cannot be mitigated through transparency. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Accurately identifying sources of bias in credit decisions "may be as critical to risk management oversight as predicting default and prepayment risks." [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Machine learning does not require higher-order cognitive skills like reasoning or abstract understanding; it is oriented to outcomes, not process — leaving it vulnerable to pursuing forms of analysis that an experienced finance professional would set aside as suspect. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

## Entities mentioned

- [[kristin-johnson]]
- [[frank-pasquale]]
- [[jennifer-chapman]]
- [[fordham-law-review]]
- [[office-of-the-comptroller-of-the-currency]]
- [[consumer-financial-protection-bureau]]
- [[new-york-dfs]]

## Concepts mentioned

- [[algorithmic-bias]]
- [[automated-decision-making]]
- [[fintech-regulation]]
- [[disparate-impact]]
- [[black-box-problem]]
- [[xai-explainable-ai]]
- [[responsible-ai]]
- [[ai-governance-in-ma]]
- [[information-asymmetry]]
- [[due-diligence]]
- [[machine-learning]]
- [[deep-learning]]

## Notes

The paper was prepared for the Fordham Law Review symposium "Rise of the Machines: Artificial Intelligence, Robotics, and the Reprogramming of Law" (February 15, 2019). It is not empirical — it is a legal-policy essay that synthesises ML/AI technical literature with regulatory and antidiscrimination law analysis.

Useful quotable passages:

- "ADM may only shift the locus of discrimination from the bank manager's desk to the programmer's computer screen or to the data scientists' training sets since data are never brute or raw — they are always collected, analyzed, and used by people, who may have the same conscious calculations, barely conscious emotions, or unconscious biases at play in their own observations." (p. 506)
- "Machine learning is in this way reminiscent of an idiot savant: like a calculator multiplying fifteen-digit numbers faster than any human can, in a narrow, well-specified area, it can reach conclusions faster than any human can." (p. 508)
- "The intelligence of a machine learning algorithm is oriented to outcomes, not process; a 'smart' algorithm is designed to reach consistently accurate results on a chosen task, even if the algorithm does not 'think' like a person." (p. 508)
- "Accurately identifying sources of bias in credit decisions may be as critical to risk management oversight as predicting default and prepayment risks." (p. 523)
- "[U]sers need to be confident that the model will perform well on real-world data." (p. 524)

Key open questions raised by the paper:
- Does the CFPB have sufficient statutory and institutional capacity to enforce ADM bias standards in fintech credit markets, particularly after recent reorganization?
- Can explainability requirements be made legally binding on fintech firms holding SPNB charters, or does federal preemption remove state levers?
- Is an outright ban on algorithmic use in certain consumer credit markets (e.g., payday lending) legally and practically feasible?

Seminar paper usage note: This paper provides the core theoretical and regulatory framework for the "risks from algorithmic bias" portion of the research question. It should anchor the Kritische Reflexion section (alongside Herbosch & Mertens 2025 and Arrieta et al. 2020). Johnson et al. argue that bias is not merely a technical problem but a structural regulatory one — a framing that complements the technical XAI arguments in Arrieta et al. (2020) and the legal liability analysis in Herbosch & Mertens (2025).

Published in: Fordham Law Review, Vol. 88, No. 2, November 2019, pp. 499–530. (Peer-reviewed symposium essay; HeinOnline URL: https://heinonline.org/HOL/Page?handle=hein.journals/flr88&id=515)
