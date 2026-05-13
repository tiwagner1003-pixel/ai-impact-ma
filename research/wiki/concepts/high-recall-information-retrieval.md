---
title: High-Recall Information Retrieval
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]
aliases: [high-recall IR, high-recall retrieval, recall-oriented IR]
---

# High-Recall Information Retrieval

**An information retrieval paradigm that prioritizes minimizing false negatives (missed relevant items) over minimizing false positives (retrieved non-relevant items), used in legal, medical, and compliance domains where overlooking a relevant document has severe consequences.**

## Summary

High-recall IR inverts the standard web-search optimization target. Whereas web search optimizes early precision (top results are relevant), high-recall IR demands that the system return all or nearly all relevant items, accepting a higher rate of irrelevant results in exchange for completeness. The cost asymmetry is domain-driven: in legal due diligence, missing a key contractual clause can expose an acquirer to undisclosed liabilities worth hundreds of millions of dollars, while reviewing one extra false-positive sentence costs only minutes of analyst time. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Legal due diligence passage retrieval is one of the most extreme high-recall IR tasks documented in the NLP literature. On the KIRA dataset, relevant sentences represent only 0.01–0.7% of all sentences per topic across 15 million total sentences — a class imbalance exceeding 99.3%. This "needle-in-a-haystack" structure means that a model predicting all sentences as non-relevant would achieve 99%+ accuracy but 0% recall, making accuracy a meaningless metric and recall the primary measure of success. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

The high-recall framing has direct methodological implications: evaluation should prioritize recall and F1 (with a recall-weighted interpretation) over precision; training objectives should favor recall-oriented optimizers (e.g., Passive-Aggressive vs. L-BFGS in CRFs); and model selection in practice should accept lower precision in exchange for higher recall unless a reliable post-filter exists. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Variations / sub-concepts

- Technology-assisted review (TAR) — human-in-the-loop high-recall retrieval used in e-discovery
- Total recall challenge — TREC shared task for high-recall retrieval benchmarking
- Annotation-level vs. sentence-level evaluation — annotation-level is more lenient, treating nearby sentences as a unified passage

## Key claims across sources

- Legal DD has "needle-in-a-haystack" properties: relevant sentences are 0.01–0.7% of the total corpus per topic, making recall the primary success metric. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- In high-recall IR, missing a relevant item has critical implications; this asymmetry justifies training objectives that maximize recall even at precision cost. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The Passive-Aggressive (PA) CRF optimizer is preferred over L-BFGS for high-recall DD because PA updates only on errors, producing more inclusive classifications. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- LLMs operating in few-shot mode can achieve recall comparable to or exceeding supervised CRF baselines (Dolphin-Llama3: 0.926 vs. CRF-PA: 0.847), despite using no labeled training data. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- GPT-4 (few-shot) achieves recall 0.93–0.96 on a single KIRA topic, demonstrating high-recall viability of LLMs on a smaller evaluation. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Related

- [[due-diligence]] — the primary application domain requiring high-recall IR
- [[kira-dataset]] — the benchmark exemplifying extreme high-recall requirements
- [[conditional-random-fields]] — the supervised model class optimized for high-recall with PA
- [[in-context-learning-for-due-diligence]] — the LLM approach achieving competitive recall without training
- [[due-diligence-quality]] — quality framework within which recall is a key dimension
- [[legal-contract-review]] — the closest AI subdomain with shared high-recall requirements

## Open questions

- What is the minimum acceptable recall threshold for a due diligence retrieval tool to be used in professional M&A without human review of all rejected sentences?
- Can active learning techniques reduce annotation cost while maintaining high-recall performance for new DD topics?
