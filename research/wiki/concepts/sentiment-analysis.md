---
title: Sentiment Analysis
type: concept
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [Opinion Mining, Textual Sentiment Analysis, NLP Sentiment]
---

# Sentiment Analysis

**A sub-discipline of natural language processing (NLP) concerned with the computational identification and categorization of subjective opinions, emotions, or attitudes within text data.**

## Summary

Sentiment analysis encompasses a range of methods for extracting evaluative content from text — determining whether text is positive, negative, neutral, or expressive of more nuanced emotions. In finance and accounting research, it is applied to corporate disclosures, earnings calls, news, and social media to extract signals that predict market outcomes. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

The main methodological families are: (1) rule-based / dictionary methods, which count positive and negative words using established lexicons (e.g., the Loughran-McDonald word lists developed specifically for financial text); (2) classical machine learning classifiers (naive Bayes, support vector machines, gradient boosting); (3) hybrid methods combining lexicons and ML; and (4) large language models (LLMs) such as GPT, BERT, FinBERT, which can capture contextual meaning and nuance beyond word-count approaches. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

Degen et al. (2024) position LLM-based sentiment analysis (specifically GPT-4.0) as superior to prior dictionary-based methods for M&A sentiment extraction, arguing that LLMs understand context-dependent meaning (e.g., the word "charge" is negative in an impairment context but neutral in a pricing context) that word lists cannot capture. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Variations / sub-concepts

- [[ma-sentiment-analysis]] — sentiment analysis applied specifically to M&A activity
- Dictionary-based sentiment (Loughran-McDonald, Harvard GI dictionary)
- ML-based sentiment classification (naive Bayes, SVM)
- LLM-based sentiment scoring (GPT-family, FinBERT)
- Aspect-based sentiment analysis (sentiment toward specific topics within a text)

## Key claims across sources

- LLMs represent a qualitative advance over dictionary-based sentiment methods by capturing contextual and syntactic nuance. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- GPT-4.0 achieves the highest alignment with human expert M&A sentiment judgments among all LLMs tested, including GPT-4o, GPT-3.5-Turbo, Gemini, Claude, and Perplexity AI. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Temperature = 0 in LLM-based sentiment scoring improves reproducibility by suppressing stochastic variation in model responses. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[ma-sentiment-analysis]] — the M&A-specific application
- [[prompt-engineering]] — the technique for structured LLM-based sentiment extraction
- [[chatgpt]] — the primary model used for sentiment scoring in the MASS study
- [[llms-in-ma]] — the broader domain of LLM application in M&A
- [[earnings-conference-calls]] — the primary text corpus for financial sentiment analysis

## Open questions

- How does GPT-4.0-based sentiment analysis compare to specialized FinLLMs (e.g., BloombergGPT, FinGPT) on M&A-specific text?
- Does multi-label sentiment (positive toward M&A but negative toward specific deal terms) require aspect-based methods beyond the current approach?
