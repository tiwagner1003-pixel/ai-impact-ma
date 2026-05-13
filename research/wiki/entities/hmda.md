---
title: HMDA
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]
aliases: [Home Mortgage Disclosure Act, HMDA data]
entity_kind: dataset
---

# HMDA

**U.S. regulatory dataset mandated by the Home Mortgage Disclosure Act; the primary source for borrower race/ethnicity and loan-level information in studies of mortgage discrimination, including Bartlett et al. (2022).**

## Overview

The Home Mortgage Disclosure Act (HMDA) requires most U.S. mortgage lenders to publicly disclose loan-level data including applicant income, race/ethnicity, loan amount, and lender name. Bartlett et al. (2022) use HMDA as the core source for minority-borrower identification (merged with ATTOM, McDash, and Equifax data to recover credit scores, LTVs, and loan terms missing from HMDA alone). [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]

HMDA covers approximately 90% of U.S. mortgage originations. Its primary limitation for discrimination research is the absence of detailed credit-risk variables (credit score, LTV, contract terms) — which the Bartlett et al. (2022) data-merge strategy overcomes.

## Key facts

- Core sample: 5.65 million candidate loans from merged HMDA/ATTOM/McDash/Equifax (2009–2015). [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- 2018–2019 vintage HMDA also used for robustness; this vintage includes points and total loan costs. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- Minority indicator in HMDA: self-reported race/ethnicity (Latinx or Black) from HDMA, plus borrower-name race/ethnicity algorithm (Kerr & Lincoln 2010) for loans missing HMDA indicators. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]

## Related

- [[algorithmic-bias]] — research topic enabled by HMDA
- [[disparate-impact]] — legal doctrine tested using HMDA data
- [[fannie-mae]] — GSE whose loan data is merged with HMDA
- [[freddie-mac]] — GSE whose loan data is merged with HMDA
- [[consumer-financial-protection-bureau]] — administrator of HMDA reporting requirements

## Open questions

- What is the coverage of HMDA for non-bank FinTech lenders? Bartlett et al. note FinTech lenders originated approximately 3.1% of GSE loans and 1.6% of FHA loans in their sample.
