---
title: "Mind the gap: the effect of cultural distance on mergers and acquisitions — evidence from Glassdoor reviews"
type: source
created: 2026-05-04
updated: 2026-05-04
sources: []
origin: research/input/inbox/s11846-024-00811-8.pdf
author: Marius Brede, Hannes Gerstel, Arnt Wöhrmann, Andreas Bausch
date: 2025 (accepted September 2024, published online October 2024)
aliases: [Brede et al. 2025, Brede et al. 2024, cultural distance Glassdoor paper]
---

# Mind the gap: the effect of cultural distance on mergers and acquisitions — evidence from Glassdoor reviews

**Uses Culture-BERT applied to ~400,000 Glassdoor employee reviews to construct an organizational cultural distance measure for 243 M&A deals, showing that cultural friction dominates cultural learning: higher distance predicts negative CARs, lower post-merger synergies, higher acquisition premiums, and reduced acquirer innovativeness.**

## Key takeaways

- Culture-BERT (a RoBERTa-based LLM fine-tuned on 2,000 Glassdoor reviews) applied to ~400,000 Glassdoor employee reviews from 437 firms provides an organizational cultural distance measure up to 28% more accurate than prior word2vec- and survey-based approaches.
- Organizational cultural distance negatively affects both short-term capital market reactions (acquirer CARs at announcement) and long-term synergy realization (sales growth 2 and 4 years post-deal), supporting the cultural friction hypothesis over the cultural learning hypothesis.
- Cultural distance positively predicts acquisition premiums (all three pre-announcement windows: 1-day, 1-week, 1-month), meaning acquirers systematically overpay when cultural distance is highest.
- Cultural distance negatively impacts acquirer post-deal innovativeness: patent growth and new product development (NPD) are both significantly lower 2 years post-deal; adhocracy differences drive the patent effect, hierarchy differences drive the NPD effect.
- Performance and premium effects are primarily driven by differences in market orientation between acquirers and targets; this dimension is most visible to outside investors because it maps directly onto observable market share and profitability metrics.
- The NLP/Glassdoor approach overcomes a key structural weakness of prior research: traditional survey methods relied on small samples of high-level employees and had low internal validity; voluntary, anonymous employee reviews provide individual-level, granular cultural data.
- The study is among the first to use transformer-based NLP on a large Glassdoor sample to infer organizational cultural distance in M&A — and the first to link that measure to acquisition premiums and long-term innovativeness simultaneously.

## Claims

- Culture-BERT (Koch and Pasch 2022) is applied to the merged pro and con text of each Glassdoor review, tokenized to max 300 tokens, yielding four CVF probability scores per review (Clan, Adhocracy, Market, Hierarchy); firm-level scores are cumulative means across all pre-deal reviews. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- The organizational cultural distance variable is computed using the Kogut and Singh (1988) index corrected per Konara and Mohr (2019), applied to the four CVF dimension scores. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- The final deal sample contains 243 completed M&A transactions from 2008 to 2021, drawn from 437 unique US, Canadian, Australian, and UK firms matched to Glassdoor via fuzzy string matching (cosine similarity threshold 0.8). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- The mean organizational cultural distance score is 0.201 (SD = 0.103); the dominant CVF culture differs between acquirer and target in 57% of deals; Market culture is the modal dominant dimension for both acquirers (34%) and targets (41%). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Acquirer CARs are significantly negative overall (mean −0.54% over [−5,5]); cultural distance is a significant negative predictor of acquirer CAR [−10,10] (t = −2.278, p < 0.05) and acquirer CAR [−5,5] (t = −2.081, p < 0.05) and combined deal CAR (t = −1.718, p < 0.1). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- H1b is supported: organizational cultural distance reduces acquirer sales growth at both 2-year (t = −1.892, p < 0.1) and 4-year (t = −2.972, p < 0.001) horizons after deal completion. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Market culture differences are the primary driver of the negative short-term CAR and long-term synergy effects (t < −4.346, p < 0.01 for CARs; t = −2.682, p < 0.01 for 4-year sales growth). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- H2 is supported: organizational cultural distance positively predicts acquisition premiums at all three pre-announcement periods (1-day: t = 2.009, p < 0.05; 1-week and 1-month: similarly significant), indicating systematic acquirer overpayment for culturally distant targets. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Market culture differences drive the premium effect (1-week and 1-month models: t > 2.94, p < 0.01), suggesting acquirers with specific market-culture values struggle to accurately value targets that do not share those values. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- H3a is supported: cultural distance significantly reduces acquirer patent growth 2 years post-deal (t = −2.573, p < 0.05); this effect is primarily driven by adhocracy dimension differences (t = −1.959, p < 0.1). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- H3b is supported: cultural distance significantly reduces acquirer new product development 2 years post-deal (t = −1.827, p < 0.1); this effect is driven by hierarchy culture differences (t = −3.085, p < 0.001). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Robustness checks include: Jensen-Shannon divergence as alternative distance measure, toehold-deal exclusion, cross-border deal exclusion (34 removed), quadratic distance term test (no nonlinear relationship found), propensity score matching (high cultural distance deals yield −0.089 points in synergies, 95% CI [−0.157, −0.021], p < 0.05), and synthetic counterfactual analysis (−0.122 points, 95% CI [−0.3729, −0.0209], p < 0.01). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- The study is limited to English-language reviews and firms with Glassdoor presence headquartered in English-speaking markets (US, Canada, Australia, UK), restricting generalizability; Glassdoor reviews are voluntary and may not represent the full workforce. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- The study is the first to use transformer-based NLP (Culture-BERT) on a large-scale Glassdoor corpus to measure organizational cultural distance and link it to M&A acquisition premiums and post-deal innovativeness simultaneously. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

## Entities mentioned

- [[marius-brede]]
- [[hannes-gerstel]]
- [[arnt-wohrmann]]
- [[andreas-bausch]]
- [[review-of-managerial-science]]
- [[culture-bert]]
- [[glassdoor]]
- [[sdc-securities-data-company]]
- [[sp-global]] (Capital IQ database for stock/financial data)

## Concepts mentioned

- [[cultural-fit-assessment]]
- [[competing-values-framework]]
- [[post-merger-integration]]
- [[ma-success-measurement]]
- [[mergers-and-acquisitions]]
- [[pre-trained-language-models]]
- [[sentiment-analysis]]
- [[llms-in-ma]]
- [[ai-in-ma]]
- [[information-asymmetry]]
- [[synergy-prediction]]

## Notes

**Placement in seminar paper:** Abschnitt 3.4 (KI in der Post-Merger-Integration). The paper demonstrates that an LLM (Culture-BERT) can operationalize a construct — organizational cultural distance — that was previously only measurable via subjective surveys, and that this AI-derived measure has superior predictive validity for M&A outcomes. This is a strong example of AI adding value at the pre-deal / transaction / PMI interface.

**Key quote (Abstract):** "Using a state-of-the-art large language model, we construct a novel measure of organizational cultural distance based on employee reviews from Glassdoor.com covering 243 M&A deals from 2008 to 2021."

**Key quote (Introduction):** "We utilize a state-of-the-art transformer model that has shown up to 28% higher accuracy in inferring organizational culture compared to previous methods (Koch and Pasch 2022), addressing several limitations of earlier analytical methods."

**Key quote (Conclusion):** "Our study provides several key insights. First, we confirm that organizational cultural distance negatively affects both announcement day market returns (H1a) and post-merger synergy realization (H1b). These findings align with the cultural friction hypothesis (Hofstede 1980), which posits that cultural distance increases coordination and integration costs, thereby hindering M&A performance."

**Cultural learning vs. cultural friction:** The paper frames its main theoretical contest as "cultural learning hypothesis" (Sørensen 2002, interorganizational learning; Chakrabarti et al. 2009; Morosini et al. 1998) vs. "cultural friction hypothesis" (Hofstede 1980; Vaara 2002; Weber 1996). Results consistently support friction. The learning hypothesis does NOT receive empirical support in this sample.

**CVF dimensions quick reference:**
- Adhocracy (Create): adaptability, flexibility, innovation
- Clan (Collaborate): collaboration, teamwork, employee development
- Market (Compete): task completion, goal achievement, profitability
- Hierarchy (Control): rules, instructions, strict controls

**Data sources:**
- SDC (Securities Data Company) — deal data
- Thomson Reuters Refinitiv — firm financial data
- Glassdoor.com — employee reviews (cultural distance measure)
- S&P Global Inc.'s Capital IQ — stock returns, patent data, NPD data

**JEL Classification:** M140 (Corporate Culture), G340 (Mergers, Acquisitions, Restructuring), C450 (Econometric and Statistical Methods using Machine Learning)

**DOI:** https://doi.org/10.1007/s11846-024-00811-8

**Open question for seminar paper:** The paper controls for national cultural distance (Hofstede measure) but restricts the sample to English-speaking markets. A follow-on question is whether Culture-BERT can be applied to non-English reviews, and whether organizational vs. national culture remains separable in non-Anglo-Saxon M&A contexts.

**Connection to other wiki sources:** This paper complements [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]] (LLMs for due diligence document review) as a second empirical case of transformer NLP improving M&A decision quality. Unlike the MASS study ([[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]), this paper uses Culture-BERT on data that pre-dates the deals being analyzed, making the memorization critique of [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]] largely inapplicable (the cultural distance measure is an input variable, not a forecast of the outcome itself).
