---
title: "MAUD: An Expert-Annotated Legal NLP Dataset for Merger Agreement Understanding"
type: source
created: 2026-05-06
updated: 2026-05-06
sources: []
origin: research/input/papers/wang-et-al-2023-maud-merger-agreement-understanding.pdf
author: Steven H. Wang, Antoine Scardigli, Leonard Tang, Wei Chen, Dimitry Levkin, Anya Chen, Spencer Ball, Thomas Woodside, Oliver Zhang, Dan Hendrycks
date: 2023-12
aliases: [Wang et al. 2023, MAUD, Merger Agreement Understanding Dataset, EMNLP 2023 MAUD]
---

# MAUD: An Expert-Annotated Legal NLP Dataset for Merger Agreement Understanding

**Wang et al. (2023) introduce [[maud-dataset]], an expert-annotated legal NLP benchmark for answering structured deal-point questions over public merger agreements. It is highly relevant for measuring what AI can and cannot reliably do in M&A legal document review.**

## Bibliographic Note

- Venue: EMNLP 2023.
- DOI: 10.18653/v1/2023.emnlp-main.1019.
- Source file: `research/input/papers/wang-et-al-2023-maud-merger-agreement-understanding.pdf`.

## Key Takeaways

- MAUD contains 39,000+ examples and 47,457 expert annotations from 152 English-language public merger agreements.
- The dataset converts merger agreement review into a reading-comprehension task: given a deal-point question and a relevant contract excerpt, a model predicts standardized answer labels.
- The annotation process is unusually strong for legal NLP: law students received extensive training and experienced lawyers reviewed labels.
- Transformer baselines achieve useful but clearly imperfect performance. The best multi-task LegalBERT model reaches 76.1% micro-F1 and 59.7% macro-F1, which supports AI-assisted review but not autonomous legal judgment.
- Hard categories include Conditions to Closing, Deal Protection and Related Provisions, and Material Adverse Effect clauses.
- Long legal text remains a structural challenge: many examples exceed the token limits of standard transformer encoders.

## Relevance For The Seminar Paper

This is one of the strongest sources for the question of error rates or measurable AI performance inside the M&A process. Unlike broad practitioner articles, it provides a task-specific benchmark, quantitative model results, and clearly defined legal-document labels.

The paper fits best in a section on AI-assisted due diligence / legal document review and in the critical reflection on AI limits. It shows that AI can help structure repetitive legal analysis, but also that complex clauses and long-context reasoning remain difficult.

## Links

- [[maud-dataset]]
- [[merger-agreement-understanding]]
- [[due-diligence]]
- [[llms-in-ma]]
- [[ai-in-ma]]
- [[the-atticus-project]]
- [[steven-wang]]
