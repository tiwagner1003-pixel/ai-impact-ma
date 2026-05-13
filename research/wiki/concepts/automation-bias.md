---
title: Automation Bias
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-sele-chugunova-2024-human-in-loop-adm, 2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review, 2026-05-07-logg-minson-moore-2019-algorithm-appreciation]
aliases: [algorithm over-reliance, automation-induced complacency, AI overreliance]
---

# Automation Bias

**The tendency for humans to over-rely on automated recommendations, including failing to detect or correct erroneous algorithmic outputs.**

## Summary

Automation bias is directly relevant to KI-gestützte Due Diligence because DD teams may treat AI-generated risk flags, clause classifications, or scores as defaults. Sele & Chugunova (2024) find that participants followed algorithmic recommendations more closely than equally accurate human recommendations and were less likely to intervene when recommendations were least accurate. [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]

This creates a paradox for the seminar paper: human-in-the-loop is necessary for governance, but human oversight can fail if the human monitor rubberstamps AI output. Therefore, Automation Bias belongs in Kapitel 4.1 as a DD-specific bias source and in Kapitel 4.3 as a governance design problem. [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]

Goddard, Roudsari & Wyatt (2012) provide the foundational quantitative estimate: a systematic review of 74 studies across healthcare, aviation, and HCI yields a meta-analytic risk ratio of 1.26 (95% CI 1.11–1.44) — erroneous decision support advice increases the probability of an incorrect decision by 26% compared to no DSS support. This figure is directly applicable to the seminar paper's Kap. 3.4 framing of automation bias as a concrete risk. The mechanism — heuristic reliance on DSS output under cognitive load, time pressure, and high perceived system pedigree — is domain-general and transfers to DD analyst behavior. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]

Logg, Minson & Moore (2019) add an important nuance: while lay users show "algorithm appreciation" (systematically over-weighting algorithmic advice relative to the normative benchmark), experienced professionals show the inverse — they discount algorithmic advice, which paradoxically reduces their accuracy. DD professionals occupy the "expert" archetype in the Logg et al. framework, raising the possibility that the dominant risk for senior M&A professionals is strategic dismissal of AI signals, not rubber-stamping. Both risks must be addressed in governance design. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]

## Key claims across sources

- Participants preferred algorithmic recommendations over equally accurate human recommendations in 66% of cases. [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]
- Human-in-the-loop increased preference for algorithmic recommendations by 7 percentage points. [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]
- Participants were less likely to intervene with the least accurate recommendations, which undermines the intended quality-control function of human oversight. [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]
- Systematic review of 74 studies: when DSS gave erroneous advice, users followed it at a rate 26% higher than control groups without DSS (RR=1.26, 95% CI 1.11–1.44, p<0.0005). [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Negative consultation rates (user had correct answer before DSS, incorrect after) range from 6–11% in prospective healthcare studies — the most conservative, pure-AB measure. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Trust is the primary driver of AB: miscalibrated trust against actual system reliability amplifies over-reliance; higher perceived system pedigree further increases trust and AB risk. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Higher workload, task complexity, and time pressure increase heuristic DSS reliance; these are endemic to M&A deal timelines. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Display prominence of DSS output directly increases AB: more prominently displayed incorrect advice is more likely to be followed. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- AB can be mitigated by: dynamic confidence levels per recommendation (not fixed overall confidence), reduced display prominence, accountability emphasis, user training, and presenting information rather than commands. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Lay people display algorithm appreciation (over-weighting algorithmic vs. human advice) but experienced domain professionals discount algorithmic advice below a helpful threshold, reducing their accuracy. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]
- Expert professionals (national-security forecasters) weighted algorithmic advice significantly less than lay participants (d=0.60) and achieved lower forecast accuracy as a result. [[2026-05-07-logg-minson-moore-2019-algorithm-appreciation]]

## Related

- [[human-in-the-loop]]
- [[algorithmic-bias]]
- [[automated-decision-making]]
- [[due-diligence-quality]]
- [[ai-governance-in-ma]]
- [[algorithm-appreciation]] — inverse risk (expert under-reliance on algorithmic advice)
- [[kate-goddard]] — lead author of foundational systematic review
- [[jennifer-logg]] — lead author of algorithm appreciation paper

## Open questions

- How strong is automation bias among experienced M&A professionals compared with experimental participants?
- Which review designs reduce over-reliance: blind review, confidence scores, model explanations, counterfactual prompts, or mandatory challenge checklists?
- Does the expert-discounting effect (Logg et al.) apply to senior M&A professionals, and if so, how should governance design address both over-reliance (junior staff) and under-reliance (senior staff) simultaneously?
