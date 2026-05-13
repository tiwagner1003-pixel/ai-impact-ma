---
title: Algorithmic Bias
type: concept
created: 2026-05-07
updated: 2026-05-07

sources: [2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance, 2026-05-07-sele-chugunova-2024-human-in-loop-adm, 2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]
aliases: [AI Bias, ML Bias, Data Bias, Bias in AI, Bias in Machine Learning]
---

# Algorithmic Bias

**The systematic, unfair, and often structurally invisible skewing of algorithmic outputs against legally protected groups — arising from biased training data, flawed feature selection, or the algorithmic identification of neutral variables as proxies for protected characteristics (race, gender, religion, national origin) — even when the model developer did not intend to discriminate.**

## Summary

Algorithmic bias is not the same as human bias simply "migrated" into software. It is a distinct and often harder-to-detect phenomenon because it can arise through three structurally separate channels: (1) biased or incomplete input data that encodes historical discrimination; (2) the training and programming stage, where developer choices about model architecture and feature selection introduce bias; and (3) the model's own pattern-recognition process, which may independently identify a facially neutral variable as a proxy for a protected characteristic and execute discriminatory outcomes — even when developers explicitly programmed the algorithm not to discriminate on that trait. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

A key insight from Johnson, Pasquale & Chapman (2019) is that automated decision-making (ADM) platforms shift, rather than eliminate, the locus of discrimination: "ADM may only shift the locus of discrimination from the bank manager's desk to the programmer's computer screen or to the data scientists' training sets since data are never brute or raw — they are always collected, analyzed, and used by people, who may have the same conscious calculations, barely conscious emotions, or unconscious biases at play in their own observations." [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

In credit markets specifically, algorithmic bias is amplified by the use of alternative data. Fintech firms incorporating social media activity, shopping patterns, internet browsing history, and peer payment networks into creditworthiness scoring introduce socioeconomic proxies for race, gender, and geographic redlining that are structurally harder to detect than explicit use of protected characteristics. Credit-scoring mechanisms "include factors that do not just assess the risk characteristics of the borrower; they also reflect the riskiness of the environment in which a consumer is utilizing credit, as well as the riskiness of the types of products a consumer uses" — importing environmental discrimination into individual scoring. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

Data quality compounds the problem: a 2004 NASPIRG study found that 79 percent of consumer credit reports contained errors and 25 percent contained significant errors resulting in denial of credit. Building these errors into ADM systems "will amplify inaccuracy and entrench errors into automated systems that are faster, more ubiquitous, and nearly impossible to correct." [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]

## Variations / sub-concepts

- Training-data bias — discrimination encoded in historical datasets used to train models
- Feature-selection bias — developer choices about which variables to include that systematically disadvantage protected groups
- Proxy discrimination — an algorithm using a neutral variable as a statistical proxy for a protected characteristic
- [[disparate-impact]] — the legal doctrine capturing the discriminatory effects of facially neutral algorithmic policies on protected groups
- Alternative-data bias — bias introduced through non-traditional credit data (social media, shopping patterns) that correlates with race, gender, or geography
- Feedback-loop bias — where biased model outputs generate biased training data for future model iterations
- [[automation-bias]] — user-side over-reliance on algorithmic recommendations, causing humans to under-correct erroneous outputs

## Key claims across sources

- A learning algorithm may independently identify a facially neutral attribute as a proxy for a legally protected trait and execute discriminatory results even when developers explicitly programmed the algorithm not to discriminate on that trait. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Data mining systems are capable of reproducing the biases created by human decisions because the data inputted has been simplified to teach the computer to learn by example — often a flawed one. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- AI/ML systems can aggregate image or voice data that reflects unconscious bias, creating disparate-impact risks even in facially neutral systems. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- 79 percent of consumer credit reports contained errors in 2004; 25 percent contained significant errors leading to credit denial — embedding such errors in automated systems entrenches and amplifies inaccuracy. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Accurately identifying sources of bias in credit decisions may be as critical to risk management oversight as predicting default and prepayment risks. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Advanced machine learning and AI will enhance the ability of creditors, payday lenders, and other predatory market participants to target vulnerable consumers, exacerbating extant predatory-lending problems. [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- Human oversight does not automatically neutralise algorithmic bias: in Sele & Chugunova's experiment, users followed algorithmic recommendations closely and were less likely to intervene when recommendations were least accurate. [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]

## Related

- [[automated-decision-making]] — the broader class of algorithmic systems within which bias operates
- [[disparate-impact]] — the legal framework for challenging algorithmic discrimination
- [[black-box-problem]] — algorithmic opacity makes bias detection and correction structurally difficult
- [[xai-explainable-ai]] — explainability is the primary technical tool for detecting and correcting algorithmic bias
- [[responsible-ai]] — the governance framework that treats bias mitigation as a core principle
- [[ai-governance-in-ma]] — bias is a named component of the practitioner M&A AI governance framework
- [[automation-bias]] — behavioural channel through which biased or inaccurate AI recommendations survive human review
- [[human-in-the-loop]] — governance mechanism that must be designed carefully to avoid rubber-stamping
- [[fintech-regulation]] — the regulatory context within which algorithmic bias in credit markets is governed
- [[frank-pasquale]] — leading scholar on algorithmic opacity as a structural source of bias
- [[kristin-johnson]] — lead author of the primary source on algorithmic bias in finance
- [[office-of-the-comptroller-of-the-currency]] — regulator whose preemption decisions affect bias-enforcement capacity

## Open questions

- Can existing antidiscrimination law (Equal Credit Opportunity Act, Fair Housing Act) reach algorithmic proxy discrimination, or does legislation need to be updated to address it explicitly?
- Is explainability a sufficient remedy for algorithmic bias, or does bias mitigation require additional regulatory tools such as algorithmic auditing requirements or outcome-based disparate-impact testing?
- How does algorithmic bias in credit scoring interact with M&A due diligence contexts — specifically, can biased creditworthiness data distort target valuations or acquisition risk assessments?
