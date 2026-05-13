---
title: M&A Sentiment Analysis
type: concept
created: 2026-05-03
updated: 2026-05-04
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting, 2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]
aliases: [M&A Sentiment, M&A Sentiment Score, MASS methodology]
---

# M&A Sentiment Analysis

**The extraction and aggregation of managerial sentiment toward merger and acquisition activity from textual sources — primarily earnings call transcripts — using natural language processing or large language models.**

## Summary

M&A sentiment analysis applies NLP or LLM-based techniques to corporate communications to measure how positively or negatively firm managers discuss M&A activity. The key theoretical premise is that managers have private information about their firms' deal intentions that is partially revealed through verbal cues in conference calls, earnings calls, and other communications — but is not yet publicly observable in deal announcement data. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

Degen et al. (2024) is the first study to apply a full LLM-based approach to construct an aggregate market-level M&A sentiment index (MASS) from earnings calls. Prior textual analysis in finance used dictionary-based methods (e.g., Loughran-McDonald word lists) or classical machine learning classifiers (naive Bayes, SVMs). LLMs represent a step change: they can understand syntactic nuance and context-dependent meaning that word-count methods miss. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

The MASS construction process involves: (1) keyword filtering to identify M&A-relevant paragraphs; (2) LLM scoring on a –2 to +2 scale with forward-looking classification; (3) averaging to transcript, monthly, and 3-month rolling average levels. The 18-month lagged version of the resulting index predicts aggregate M&A deal volume with statistically and economically significant power. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

A key empirical finding is that only extreme sentiment quintiles (top and bottom 20%) are statistically significant predictors. High positive sentiment signals a late-cycle phase after which deal activity typically declines (analogous to sentiment-driven mean reversion in equity markets). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Variations / sub-concepts

- Dictionary-based M&A sentiment (Loughran-McDonald word lists)
- ML-based sentiment classification (naive Bayes, SVM)
- LLM-based M&A sentiment scoring (MASS approach)
- Deal-level sentiment analysis (individual acquirer/target pair)
- Aggregate market-level M&A sentiment indices

## Key claims across sources

- ChatGPT (GPT-4.0) applied to earnings call paragraphs achieves higher M&A sentiment classification accuracy than other LLMs and aligns closely with human expert consensus. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- An 18-month lag between aggregate M&A sentiment and realized deal volume is optimal, reflecting the time required for deal preparation and execution. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- MASS provides statistically significant incremental predictive power above all four benchmark sentiment indices and all tested fundamental macroeconomic factors. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Very high M&A sentiment is a contrarian late-cycle signal: it predicts fewer deals 18 months later, not more. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[sentiment-analysis]] — the parent NLP discipline
- [[prompt-engineering]] — the technique for extracting structured sentiment from LLMs
- [[llms-in-ma]] — the application of LLMs to M&A tasks broadly
- [[mass-index]] — the specific index constructed via this methodology
- [[merger-waves]] — the aggregate phenomenon that M&A sentiment tracks
- [[chatgpt]] — the model used to score sentiment in the MASS study

## Validity challenge: the memorization problem

> ⚠️ Conflict: [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]] interprets the MASS index's predictive power (out-of-sample R2 = 9.4%) as evidence that LLMs extract genuine managerial private information from earnings calls. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]] demonstrates that this interpretation cannot be verified: the MASS study's entire sample (July 2013 – December 2023) falls within GPT-4o's training data, and M&A sentiment scoring is a "future-variant" task (the model's judgment of whether a paragraph signals M&A activity would differ if it knew which deals actually materialized). Any correct MASS prediction is observationally equivalent to memorization of realized M&A outcomes. The MASS study's predictive power therefore does not establish genuine forecasting ability. Unresolved.

Lopez-Lira et al. (2025) classify M&A sentiment scoring as a future-variant task because the concept of "M&A relevance" and "positive sentiment toward M&A" is judgment-laden: a model with knowledge of which deals actually occurred after a transcript date will assess the same paragraph differently than a model without that knowledge. This is not a minor technical concern but a fundamental methodological objection applicable to the entire pre-cutoff sample of Degen et al. (2024). [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

## Open questions

- Can M&A sentiment analysis be applied at the deal level to predict individual acquirer behavior?
- Do non-English transcripts (Japanese, German, French) require language-specific model fine-tuning to achieve comparable accuracy?
- How does LLM-based sentiment scoring hold up when applied to press releases, 10-K filings, or analyst reports rather than earnings calls?
- Is there a post-cutoff replication of the MASS methodology that would confirm or refute genuine forecasting ability independent of memorization?
