---
title: Algorithm Appreciation
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-logg-minson-moore-2019-algorithm-appreciation]
aliases: [algorithm preference, algorithmic advice preference]
---

# Algorithm Appreciation

**The tendency of lay people to give more weight to advice believed to come from an algorithm than to identical advice from a human advisor — the empirically documented inverse of "algorithm aversion."**

## Summary

Logg, Minson & Moore (2019) coin the term "algorithm appreciation" to describe the robust finding that, across six experiments and multiple judgment domains (visual estimation, forecasting songs, predicting attraction, geopolitical forecasting), participants weight identical numerical advice more heavily when told it comes from an algorithm than when told it comes from another person. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]

This directly challenges the "algorithm aversion" narrative common in the prior literature (Dietvorst et al. 2015), which argued that people reject algorithms, particularly after seeing them err. Logg et al. show that in the more common real-world condition — where people do not receive explicit performance feedback before deciding — lay individuals systematically prefer algorithmic advice.

A critical boundary condition is domain expertise. In Experiment 4, U.S. national-security forecasting professionals heavily discounted algorithmic advice relative to their own judgment, in direct contrast to lay participants. This expert discounting of algorithmic advice reduced their forecast accuracy below that of lay people who utilized algorithmic advice. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]

For the M&A seminar paper, algorithm appreciation creates a dual risk profile: lay decision-support users (e.g., junior analysts or non-specialist reviewers) are likely to over-weight AI DD outputs ([[automation-bias]] territory), while experienced DD professionals may under-weight valuable algorithmic signals, missing deals or risks that quantitative models detect.

## Variations / sub-concepts

- [[automation-bias]] — the related over-reliance phenomenon when following incorrect algorithmic recommendations
- Algorithm aversion — the inverse effect, empirically less robust for non-performance-feedback conditions; first described by Dietvorst et al. (2015)
- Weight on Advice (WOA) — the continuous measure of advice utilization used by Logg et al.; WOA = (final − initial) / (advice − initial)

## Key claims across sources

- Lay participants gave significantly more weight to algorithmically labeled advice than to identical human advice across all six experiments. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Algorithm appreciation held even in highly subjective domains (romantic attraction prediction) and regardless of whether the algorithm was described as a "black box" or given a process description. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- 66% of participants in Experiment 3 chose to have their bonus determined by the algorithm's estimate rather than their own; 88% chose the algorithm over another person's estimate. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Expert professional forecasters (national-security domain) showed algorithm appreciation significantly below lay participants (F(1,338)=32.39, p<0.001, d=0.60) and this reduced their accuracy relative to lay algorithm users. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Researchers in judgment-and-decision-making predicted algorithm aversion in lay participants but were directionally wrong — participants displayed algorithm appreciation instead, with an effect-size difference (d=1.25) between researchers' predictions and actual outcomes. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]

## Related

- [[automation-bias]] — overlapping concept; both involve human response to algorithmic advice
- [[human-in-the-loop]] — governance design context in which algorithm appreciation and aversion play out
- [[automated-decision-making]] — broader class of algorithmic systems
- [[black-box-problem]] — opacity of algorithms that participants nonetheless appreciate
- [[due-diligence-quality]] — the practical context in which appreciation vs. aversion affects DD outcomes
- [[jennifer-logg]] — lead author who coined the term
- [[julia-minson]] — co-author
- [[don-moore]] — co-author

## Open questions

- Does algorithm appreciation generalize to M&A due diligence professionals, who combine domain expertise (like the national-security experts) with financial/legal training?
- Does algorithm appreciation decrease when DD professionals receive performance feedback on past AI-assisted decisions (the Dietvorst et al. mechanism)?
- Is algorithm appreciation stronger or weaker when the algorithm is embedded in a commercial platform with vendor branding (higher perceived pedigree per Madhavan & Wiegmann, reviewed in Goddard et al. 2012)?
