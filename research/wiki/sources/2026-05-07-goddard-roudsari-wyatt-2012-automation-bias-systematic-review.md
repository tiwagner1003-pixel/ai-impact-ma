---
title: "Automation Bias: A Systematic Review of Frequency, Effect Mediators, and Mitigators"
type: source
created: 2026-05-07
updated: 2026-05-07
sources: []
origin: research/input/papers/goddard-roudsari-wyatt-2012-automation-bias-systematic-review.pdf
author: Kate Goddard, Abdul Roudsari, Jeremy C. Wyatt
date: "2012"
aliases: [Goddard et al. 2012, Goddard automation bias review]
---

# Automation Bias: A Systematic Review of Frequency, Effect Mediators, and Mitigators

**Systematic review of 74 studies across aviation, healthcare, and human-computer interaction showing that automation bias is a robust cross-domain effect: when decision support systems give incorrect advice, users follow that advice and make incorrect decisions at a rate 26% higher than control groups without DSS support.**

## Key takeaways

- Automation bias (AB) is a robust, cross-domain effect identified across 74 studies spanning healthcare (computer-aided detection, ECG reading, diagnostic CDSS), aviation, and generic human-computer interaction research.
- Meta-analysis of four methodologically comparable healthcare studies produces a risk ratio of 1.26 (95% CI 1.11–1.44): erroneous decision support advice increases the probability of an incorrect decision by 26% compared with no decision support.
- Negative consultations — cases where a user had the correct answer before DSS use but changed it to an incorrect answer after — occur in 6–11% of cases in prospective healthcare studies, representing the clearest and most conservative measure of pure automation bias.
- Trust is the primary driver of over-reliance: automation bias increases when users trust the system highly, are less confident in their own judgment, or perceive the system as having high pedigree (expert vs. novice system). Trust calibration is the central target for AB mitigation.
- Automation bias occurs more often with task-inexperienced users but can also occur with experienced users; experienced physicians are less reliant on DSS and more likely to identify incorrect advice, but this result does not always hold.
- Key mitigation strategies include: (1) training users to recognize DSS error and increasing personal accountability; (2) DSS design factors — reducing display prominence of advice, providing dynamic confidence levels alongside recommendations, and presenting supportive information rather than commands.

## Claims

- Of 13,821 initially retrieved papers, 74 met inclusion criteria; the review covered aviation, healthcare (CAD, ECG, diagnostic systems), and generic HCI research from 1993–2009. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- A Mantel-Haenszel random effects meta-analysis of four comparable healthcare studies yields RR=1.26 (95% CI 1.11 to 1.44, p<0.0005); erroneous DSS advice increased the risk of an incorrect decision by 26%. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Negative consultation rates (user correct before DSS, incorrect after) range from 6% (Friedman et al.) to 11% (McKibbon & Fridsma) in prospective empirical studies. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Task-inexperienced users are more prone to automation bias; experienced physicians are more likely to recognize incorrect DSS advice. However, experience-based benefits are not universal — over-familiarity with a reliable system can produce complacency through desensitization. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Trust is the primary driver of over-reliance; it is most dangerous when incorrectly calibrated against actual system reliability. Users exhibit a "positivity bias" predisposing them to trust automated aids over human ones (Dzindolet et al. finding reviewed). [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Higher workload, task complexity, and time pressure shift users toward heuristic use of DSS output, increasing over-reliance when that output is incorrect. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Display prominence of advice directly affects AB: more prominently displayed incorrect advice is more likely to be followed. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- Automation bias can be mitigated by updating DSS confidence levels dynamically per piece of advice (rather than a fixed overall confidence), reducing screen prominence, and presenting information rather than commands. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- The optimal reliability threshold for DSS, below which users do not become complacent, is approximately 70% (Madhavan & Wiegmann); higher reliability paradoxically increases complacency-related errors. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]
- External accountability manipulations (being observed, knowing one is accountable) reduce commission errors significantly in two studies; internal perceptions of accountability are more effective than externally imposed accountability in a third study. [[2026-05-07-goddard-roudsari-wyatt-2012-automation-bias-systematic-review]]

## Entities mentioned

- [[kate-goddard]]
- [[abdul-roudsari]]
- [[jeremy-wyatt]]
- [[city-university-london]]
- [[university-of-warwick]]
- [[journal-of-the-american-medical-informatics-association]]

## Concepts mentioned

- [[automation-bias]]
- [[human-in-the-loop]]
- [[automated-decision-making]]
- [[due-diligence-quality]]
- [[black-box-problem]]
- [[ai-governance-in-ma]]
- [[algorithmic-bias]]

## Notes

- This review is foundational for the seminar paper's treatment of automation bias in Kap. 3.4 and 4.2. The 26% risk ratio (RR=1.26) is the single most-citable quantitative estimate of how erroneous algorithmic advice increases decision errors in a professional setting.
- Scope note for transfer to DD context: All 74 studies involve decision support in professional or near-professional settings (clinicians, pilots, military operators). The mechanism — cognitive heuristic replacement with DSS output under workload and time pressure — is domain-general and applies to due diligence analysts working under deal-timeline pressure.
- The review distinguishes automation bias (commission errors: following wrong advice) from automation-induced complacency (omission errors: not acting because no alert was given). Both are relevant to AI-assisted DD: commission = acting on a false positive risk flag; omission = missing a real risk because AI did not flag it.
- Authors explicitly recommend examining negative impacts of CDSS introduction alongside positive effects — a methodological call that applies directly to AI DD platform evaluations.
- Key quote (p. 121): "there is often a failure to recognize the new errors that CDSS can introduce."
- JAMIA publication: J Am Med Inform Assoc 2012;19:121–127. DOI: 10.1136/amiajnl-2011-000089
- Limitation acknowledged: heterogeneity of study designs and outcomes prevented a larger meta-analysis; the pooled RR is based on four studies with common methodology.
