---
title: "Consumer-Lending Discrimination in the FinTech Era"
type: source
created: 2026-05-07
updated: 2026-05-07
sources: []
origin: research/input/papers/bartlett-et-al-2022-consumer-lending-discrimination-fintech.pdf
author: Robert Bartlett, Adair Morse, Richard Stanton, Nancy Wallace
date: "2022"
aliases: [Bartlett et al. 2022, Bartlett FinTech discrimination]
---

# Consumer-Lending Discrimination in the FinTech Era

**Using 9 million GSE and FHA mortgage loans (2009–2015 and 2018–2019) with full loan-level data on LTV, credit score, and race/ethnicity, this study shows that both FinTech and non-FinTech lenders charge Latinx/Black borrowers 4–5 basis points more interest than equally creditworthy non-minority borrowers — and that FinTech algorithmic lenders, while slightly less discriminatory for FHA loans, do not eliminate discrimination and cost minority borrowers over $450 million annually.**

## Key takeaways

- Minority borrowers (Latinx/Black) pay 4.7–4.9 basis points more in interest for GSE purchase loans and 1.5–1.6 basis points more for FHA loans than risk-equivalent non-minority borrowers, even after controlling for all legitimate-business-necessity creditworthiness variables available to lenders in the GSE and FHA pricing grids.
- FinTech algorithmic lenders show rate disparities similar to or only slightly lower than non-FinTech lenders for GSE loans; for FHA loans, FinTech discrimination is 27–37% lower than non-FinTech, but statistically significant disparities persist.
- The minority rate premium is geographically concentrated: in high-minority-share census tracts, Black/Latinx borrowers pay 9.7–16.2 basis points more than otherwise-equivalent non-minority borrowers in low-minority-share tracts — suggesting spatial pricing discrimination reinforced by both human and algorithmic lending.
- These differentials translate to minority borrowers paying over $450 million in excess interest annually on outstanding GSE and FHA mortgages (estimated from 2018–2019 HMDA data).
- The bias mechanism is pricing discrimination, not approval discrimination: minority borrowers who qualify for GSE/FHA loans within the same credit-score/LTV grid cell as non-minority borrowers still pay higher rates, which the authors argue constitutes legally impermissible disparate impact.

## Claims

- Controlling for all variables in the GSE credit-risk pricing grid (LTV bucket, credit score, loan type, loan month/year, lender, loan-amount decile), Latinx/Black borrowers pay 4.674 basis points more for GSE purchase loans and 4.866 basis points more for FHA purchase loans. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- Rate differentials are robust across multiple robustness tests: put-back risk, servicing costs, points paid, total loan costs, post-2012 subsamples, high-quality borrowers (FICO≥740, LTV≤60%), and bank-vs-nonbank splits. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- FinTech lenders produce rate differentials of 5.081 basis points for GSE purchase loans (not significantly lower than non-FinTech's 4.666 bp, p=0.117) and 3.550 basis points for FHA purchase loans (27% lower than non-FinTech's 4.877 bp, p=0.008). [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- Minority rate disparities are highest in high-minority-share census tracts: a minority borrower in a decile-10 minority-share census tract taking a GSE purchase loan pays, on average, 13.8 basis points more than an otherwise-equivalent non-minority borrower in a decile-1 census tract (FHA: 16.2 basis points). [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- In the 2018–2019 HMDA data controlling for total loan costs, differences of 7.7 bp (GSE purchase), 6.8 bp (GSE refi), 5.4 bp (FHA purchase), and 1.9 bp (FHA refi) are found. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- The identification strategy exploits the GSE pricing grid (8×8 LTV/credit-score matrix): any interest-rate difference within the same grid cell cannot reflect differential credit risk and therefore constitutes strategic pricing discrimination. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- FinTech lenders process mortgage applications 20% faster than traditional lenders and have default rates 25% lower (Fuster et al. 2019, cited), yet they do not eliminate pricing discrimination. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- Total excess interest cost to minority borrowers is over $450 million per year, extrapolated from estimated 2018–2019 HMDA differentials applied to the Federal Reserve's Z.1 and HUD data on outstanding GSE and FHA mortgages. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]
- The paper finds no evidence that results are driven by put-back risk (post-2012 subsample robust), servicing-cost differentials (default rates controlled), or minority borrowers' differential acceptance of discount points. [[2026-05-07-bartlett-et-al-2022-consumer-lending-discrimination-fintech]]

## Entities mentioned

- [[robert-bartlett]]
- [[adair-morse]]
- [[richard-stanton]]
- [[nancy-wallace]]
- [[uc-berkeley-school-of-law]]
- [[haas-school-of-business]]
- [[journal-of-financial-economics]]
- [[consumer-financial-protection-bureau]]
- [[fannie-mae]]
- [[freddie-mac]]
- [[hmda]]

## Concepts mentioned

- [[algorithmic-bias]]
- [[disparate-impact]]
- [[fintech-regulation]]
- [[automated-decision-making]]
- [[proxy-discrimination]]
- [[due-diligence]]
- [[black-box-problem]]
- [[algorithmic-lending]]

## Notes

- Central relevance to the seminar paper: This is the strongest empirical peer-reviewed evidence that algorithmic financial AI does not eliminate discrimination — it may merely redistribute it across a different set of mechanisms (pricing algorithms vs. loan-officer discretion). The key transfer to DD: if financial AI encoding proxy-variable bias persists even with perfect credit-risk controls, the same mechanism applies to DD AI tools trained on M&A data that embed historical deal-team biases.
- Identification strategy is particularly clean: GSE guarantee fees are determined exclusively by LTV and credit score, so any residual interest-rate variation within a credit/LTV bucket is lender-strategic, not credit-risk-based. This makes the setting one of the few in which all legitimate-business-necessity variables are fully observable.
- FinTech "40% less discrimination" figure: The widely cited statistic in popular accounts that "FinTech lenders discriminate 40% less" appears to derive from comparing the roughly 27% reduction on FHA loans; it is NOT found for GSE loans. Users should exercise caution with this figure and note the precise sub-segment it applies to.
- Proxy-variable mechanism: The paper does not directly identify which proxy variables drive the remaining FinTech discrimination, but it explicitly notes that algorithmic pricing can "naturally discover that higher prices could be quoted to profiles of borrowers or geographies associated with low-shopping tendencies" — which constitutes proxy discrimination even without explicit use of protected characteristics.
- Data: 5.65 million candidate loans from merged HMDA/ATTOM/McDash/Equifax (2009–2015); 5.65 million loans in 2018–2019 HMDA. Final analysis dataset is the 3.4 million GSE and 2.3 million FHA loans passing all filters.
- Authors' note: "Algorithmic pricing of loans applies estimation techniques over large sets of data to enable profit-maximizing pricing strategies. An algorithm could naturally discover that higher prices could be quoted to profiles of borrowers or geographies associated with low-shopping tendencies." This operationalizes the proxy-discrimination mechanism without requiring discriminatory intent.
- Journal of Financial Economics, 143(1), 30–56. DOI: https://doi.org/10.1016/j.jfineco.2021.05.047
