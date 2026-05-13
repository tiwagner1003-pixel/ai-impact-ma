---
title: "Large Language Models and M&A: Can ChatGPT help forecast M&A activity?"
type: source
created: 2026-05-03
updated: 2026-05-03
sources: []
origin: research/input/papers/ssrn-4862121.txt
author: Dominik Degen, Jens Kengelbach, Daniel Kim, Soenke Sievers, Yiran Wang
date: "2024-07-01"
aliases: [Degen et al. 2024, SSRN 4862121, LLMs and M&A forecasting paper, MASS paper]
---

# Large Language Models and M&A: Can ChatGPT help forecast M&A activity?

**Degen, Kengelbach, Kim, Sievers & Wang (2024) construct a ChatGPT-derived M&A Sentiment Score (MASS) from earnings call transcripts of S&P Global 1200 companies and demonstrate it has statistically significant forecasting power for aggregate M&A deal volume up to 18 months ahead, adding incremental explanatory power beyond established sentiment indices and fundamental macroeconomic drivers.**

## Key takeaways

- MASS (M&A Sentiment Score) built from GPT-4.0 scoring of earnings call paragraphs predicts future aggregate M&A deal volume with an in-sample adj. R2 of 9.1% (18-month lag) and an out-of-sample R2 of 9.4% — outperforming Baker-Wurgler, Huang et al., and UM Consumer Confidence indices.
- The optimal predictive lag is 18 months, consistent with the timeline of deal preparation, target identification, due diligence, and regulatory review; this economic grounding strengthens the causal interpretation.
- MASS retains statistical significance (t > 1.81) when combined with each of six macroeconomic fundamentals, adding 4–12 percentage points to adj. R2 in every paired regression.
- Among six LLMs tested (GPT-4.0, GPT-4o, GPT-3.5-Turbo, Perplexity AI, Claude, Gemini), GPT-4.0 shows the highest phi-coefficient correlation with a four-person human M&A expert consensus panel, validating the model selection.
- The OECD Business Confidence Index is a surprisingly strong standalone predictor (out-of-sample R2 = 49.1%); combining it equally with MASS yields an out-of-sample R2 of 50.5%, a statistically significant improvement.
- Only extreme quintiles of 18-month lagged MASS (top and bottom 20%) have statistically significant association with deal activity; middle-range sentiment is non-predictive.
- The study is funded by DFG/TRR 266 and co-authored by four BCG practitioners and one Paderborn University academic; potential conflicts of interest should be flagged when citing.

## Claims

- The dataset covers 40,776 earnings call transcripts (July 2013 – December 2023) for S&P Global 1200 companies; after 25% random subsampling, 37,549 M&A-relevant paragraphs are analyzed.
- Paragraph scoring uses role-prompting ("As a finance expert…"), a structured JSON output, integer scale –2 to +2, and API temperature = 0 for reproducibility.
- The raw MASS is constructed by averaging paragraph scores to transcript level, averaging monthly, then applying a 3-month rolling average to smooth quarterly reporting cycles.
- A one-standard-deviation increase in MASS is associated with a 3–9% decrease in predicted monthly M&A deal volume — the negative sign reflects late-cycle mean-reversion, not a direct negative relationship.
- In-sample, the combined MASS + OECD_BCI model explains 44.1% of variation in monthly M&A deal counts.
- Forecast encompassing tests (Harvey et al. 1998) show MASS encompasses the predictive content of HUANG_ET_AL and UM_CSI but not BAKER_WURGLER or OECD_BCI alone.
- Out-of-sample, MASS achieves R2OS = 9.4% vs. 4.4% (Baker-Wurgler), –6.5% (Huang et al.), 3.2% (UM CSI), and 49.1% (OECD BCI).
- GPT-4.0 identifies 68% of paragraphs as M&A-related with average conditional sentiment 0.82; human consensus identifies 65% as M&A-related with average sentiment 0.64.
- Claude (Anthropic) shows the highest average conditional sentiment (1.26) and the lowest M&A identification rate (43%) — the most divergent from human consensus of all LLMs tested.
- Word clouds confirm construct validity: high-MASS (+2) paragraphs cluster around "well," "strong," "growth," "integration"; low-MASS (–2) paragraphs cluster around "negative," "failed," "impairment," "goodwill," "charge."
- MASS is negatively correlated (–46%) with the University of Michigan Consumer Sentiment Index and negatively correlated with OECD_BCI, confirming it captures corporate/insider sentiment rather than general consumer confidence.
- Dependent variable throughout is the monthly count of M&A deals with deal value >$100 million USD, sourced from Refinitiv/LSEG.
- The paper is TRR 266 Working Paper No. 150 (July 2024); first version February 2024; available at SSRN 4862121. Not peer-reviewed as of ingest date.
- Four of five authors (Degen, Kengelbach, Kim, Wang) are BCG employees; Sievers (Paderborn University) declares no competing interests.

## Entities mentioned

- [[dominik-degen]]
- [[jens-kengelbach]]
- [[soenke-sievers]]
- [[boston-consulting-group]]
- [[paderborn-university]]
- [[gpt-4]]
- [[sp-global-1200]]
- [[mass-index]]
- [[baker-wurgler-sentiment-index]]
- [[oecd-business-confidence-index]]

## Concepts mentioned

- [[llms-in-ma]]
- [[ai-in-ma]]
- [[merger-waves]]
- [[mergers-and-acquisitions]]
- [[ma-sentiment-analysis]]
- [[prompt-engineering]]
- [[earnings-conference-calls]]
- [[due-diligence]]
- [[memorization-problem-llms]]
- [[lookahead-bias]]

## Notes

**Research question (verbatim):** "Can the private information and expectations of managers about future M&A transactions – referred to as 'M&A sentiment' and derived through generative AI tools such as ChatGPT – serve as a predictive indicator for overall future M&A deal volume?"

**Key prompt (verbatim):** "As a finance expert, determine whether the paragraph is related to Mergers and Acquisitions (M&A). If it is M&A-related, rate its sentiment towards M&A on a scale from -2 to 2, where: -2 indicates a very negative sentiment / -1 indicates a mildly negative sentiment / 0 indicates a neutral sentiment / 1 indicates a mildly positive sentiment / 2 indicates a very positive sentiment. If the paragraph is not related to M&A, the sentiment should be marked as null. Furthermore, analyze if the paragraph indicates any reference towards future M&A activities. Format your response as a JSON object with the keys 'M&A related', 'Sentiment', and 'Future reference'."

**Prescribed reading context:** This is one of the four prescribed readings for Thema 7 ("Der Einfluss von KI auf M&A") at the Goethe-Universitat Frankfurt Bachelor seminar SS 2026 [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]. It is the most methodologically detailed of the four readings and provides the primary empirical grounding for claims about LLMs applied to M&A forecasting.

**Publication status:** Working paper — TRR 266 Working Paper Series No. 150, July 2024. Available at SSRN: https://ssrn.com/abstract=4862121. Funded by DFG/TRR 266 (Project-ID 403041268). Not yet peer-reviewed as of ingest date; cite accordingly in the seminar paper.

**Theoretical contributions:**
1. Introduces MASS as a novel aggregate M&A prediction index derived from LLM text analysis, bridging sentiment analysis and M&A wave literature.
2. Demonstrates that managerial private information embedded in earnings calls contains predictive power beyond market-observable fundamentals — consistent with expectation-driven investment theories (Gennaioli, Ma & Shleifer 2016).
3. Validates LLMs against human expert consensus for a specialized financial text classification task, contributing to the growing FinLLM methodology literature.

**Limitations not foregrounded by the authors:**
- Survivorship bias: only current (January 2024) S&P Global 1200 constituents; companies that were acquired, delisted, or merged out of the index are excluded.
- Only large-cap deals (>$100M threshold); findings may not generalize to mid-cap or small-cap M&A activity.
- A 25% random subsample of paragraphs was used due to API cost constraints; no sensitivity analysis on sample fraction reported.
- The one-decade sample (2013–2023) captures limited cross-cycle variation.
- The negative MASS coefficient (higher sentiment → fewer deals 18 months later) requires the cyclicality interpretation to hold consistently; the paper does not formally test a structural break or regime model.

**Validity challenge — memorization problem:** Lopez-Lira, Tang & Zhu (2025) [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]] explicitly identify Degen et al. (2024) as a study warranting caution. Their paper proves that LLM-based economic forecasting on pre-cutoff data is fundamentally non-identified: genuine forecasting ability and memorization are observationally equivalent. The MASS study's entire sample (2013–2023) is within GPT-4o's training period. M&A sentiment scoring is classified by Lopez-Lira et al. as a "future-variant" task (the model's judgment of relevance and sentiment would differ with knowledge of which deals materialized). The out-of-sample R2 of 9.4% is therefore observationally equivalent to memorization of realized M&A activity rather than genuine information extraction. This is the primary critical reflection point for the Thema 7 seminar paper (Abschnitt 4).

> ⚠️ Conflict: This source claims MASS reflects LLMs extracting genuine managerial private information [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]] proves this interpretation is non-identified and documents GPT-4o memorization of macroeconomic data at near-perfect precision for the same historical period. Unresolved.

**Suggested follow-up sources:**
- Lopez-Lira, Tang & Zhu (2025) — the memorization problem paper (arXiv 2504.14765) — critical methodological challenge; already ingested as [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- Bozman, Fairhurst & Greene (2025) — "Better Than a Coin Flip? Merger Success and AI Models" — cited by Lopez-Lira et al. as a methodologically valid post-cutoff LLM study for M&A
- Hansen & Kazinnik (2023) — LLMs decoding Fedspeak (SSRN 4399406)
- Kim et al. (2024) — LLMs for financial statement analysis (SSRN 4835311)
- Jha et al. (2024) — ChatGPT for corporate investment policies (SSRN 4521096)
