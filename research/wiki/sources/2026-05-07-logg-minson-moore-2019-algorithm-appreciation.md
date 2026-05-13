---
title: "Algorithm Appreciation: People Prefer Algorithmic to Human Judgment"
type: source
created: 2026-05-07
updated: 2026-05-07
sources: []
origin: research/input/papers/logg-minson-moore-2019-algorithm-appreciation.pdf
author: Jennifer M. Logg, Julia A. Minson, Don A. Moore
date: "2019"
aliases: [Logg et al. 2019, Algorithm Appreciation]
---

# Algorithm Appreciation: People Prefer Algorithmic to Human Judgment

**Across six experiments, lay participants consistently give more weight to advice they believe comes from an algorithm than to identical advice from a human — a phenomenon the authors call "algorithm appreciation" — while experienced professionals do the opposite, discounting algorithmic advice in ways that hurt their accuracy.**

## Key takeaways

- Lay people display robust "algorithm appreciation": they adhere more to the same numeric advice when told it comes from an algorithm than from another person, across estimation tasks (weight, song rank) and subjective forecasting tasks (romantic attraction, geopolitical events).
- Algorithm appreciation persists even when advisors are evaluated jointly (Experiment 2), when participants can choose their advisor themselves, and even when participants trust their own judgment most (Experiment 3).
- Experienced professionals (U.S. national-security forecasters) show the inverse pattern — they discount algorithmic advice below 30% WOA, heavily rely on their own judgment, and consequently achieve lower accuracy than lay participants when receiving algorithmic advice (Experiment 4).
- The key moderator is expertise: domain experts who make forecasts regularly for their job are significantly less willing to rely on algorithmic advice than lay participants, and this difference reduces forecast accuracy.
- The effect is robust across algorithm descriptions ("black box" vs. explained) and across separate and joint evaluation paradigms, suggesting algorithm appreciation is a stable lay heuristic, not an artifact of experimental design.

## Claims

- Participants gave significantly more weight to algorithmically labeled advice than identically worded human advice across all three estimation domains (weight: M_algo=0.45 vs. M_human=0.30; songs: M_algo=0.37 vs. M_human=0.21; attraction: M_algo=0.38 vs. M_human=0.26). [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- In Experiment 3 (self vs. algorithm choice), 66% of participants chose to base their bonus on the algorithm's estimate rather than their own, and 88% preferred the algorithm to another participant's estimate. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- National-security experts discounted advice from algorithms significantly more than lay participants did (F(1,338)=32.39, p<0.001, η²=0.08, d=0.60). [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Expert participants who heavily discounted algorithmic advice achieved lower forecast accuracy than lay participants who received algorithmic advice (Brier score interaction: F(1,366)=4.16, p=.042). [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Algorithm appreciation appeared even in the most subjective domain tested (predicting romantic attraction from a photo) and was robust to whether the algorithm was presented as a "black box" or described with a simple process explanation. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Researchers in the judgment-and-decision-making field consistently predicted that participants would show algorithm aversion; actual participants showed algorithm appreciation instead — the expert researchers had negative predictive accuracy (d=1.25 effect size difference between predictions and outcomes). [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Lay participants underweighted algorithmic advice relative to the normative benchmark (WOA=0.66 vs. M=0.34), suggesting room for even greater improvement in accuracy through better algorithm utilization. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- The effect of age, gender, numeracy, and algorithm familiarity did not significantly mediate algorithm appreciation in Experiments 1A–1C (all ps > 0.37). [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]

## Entities mentioned

- [[jennifer-logg]]
- [[julia-minson]]
- [[don-moore]]
- [[harvard-kennedy-school]]
- [[haas-school-of-business]]
- [[organizational-behavior-and-human-decision-processes]]

## Concepts mentioned

- [[algorithm-appreciation]]
- [[automation-bias]]
- [[human-in-the-loop]]
- [[automated-decision-making]]
- [[due-diligence-quality]]
- [[black-box-problem]]

## Notes

- The paper uses the Judge-Advisor System (JAS) paradigm: participants make an initial judgment, receive advice, then make a revised final judgment. Weight on Advice (WOA) = (final − initial) / (advice − initial); WOA of 0 = ignored, 1 = fully adopted.
- The Dietvorst et al. (2015) "algorithm aversion" paper — widely cited as showing people reject algorithms after seeing them err — actually found algorithm preference in control conditions (no performance feedback). Logg et al. replicate this and label the phenomenon more precisely.
- Key quote for the seminar paper (Kap. 3.4): "Paradoxically, experienced professionals, who make forecasts on a regular basis, relied less on algorithmic advice than lay people, which hurt their accuracy."
- Key implication for DD teams: due diligence professionals are the "expert" archetype, not the "lay" archetype. Per Experiment 4, they are likely to under-weight AI DD outputs — the opposite of automation bias. This nuances the governance discussion in Kap. 4.2: the risk for DD experts may not be over-reliance but strategic dismissal of valuable algorithmic signals.
- Logg et al. cite "theory of machine" as a proposed research framework: how people represent the internal processes, inputs, and outputs of algorithms (analogous to "theory of mind" for persons). This framing connects to the [[black-box-problem]]: opacity may reduce algorithm appreciation among experts who feel they should understand the tool.
- Publication: Organizational Behavior and Human Decision Processes, 151 (2019), pp. 90–103. DOI: https://doi.org/10.1016/j.obhdp.2018.12.005
- Pre-registrations and materials available at: https://osf.io/b4mk5/
