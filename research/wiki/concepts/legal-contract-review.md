---
title: Legal Contract Review
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-hendrycks-et-al-2021-cuad-contract-review, 2026-05-07-dwivedi-kamps-2025-icl-due-diligence, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence, 2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]
aliases: [AI contract review, legal document review, contract analysis]
---

# Legal Contract Review

**The process of identifying, extracting, and evaluating legally significant clauses, obligations, risks, and deal terms in contracts; the best-evidenced subdomain for AI-assisted due diligence.**

## Summary

Legal contract review is the strongest empirical bridge between general Legal NLP and M&A due diligence. CUAD shows that expert-labeled contract review is feasible but data-intensive; KIRA-based DD studies show the same "needle-in-a-haystack" problem in M&A due diligence; MAUD adds a merger-agreement understanding benchmark for public deal documents. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]] [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]] [[2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]]

For the seminar paper, this concept helps keep the evidentiary scope honest: AI performance evidence is strongest for legal and contract-document tasks, not for the full 13-16 discipline DD universe. [[2026-05-07-bhagwan-et-al-2018-systematic-review-dd-ma]]

## Key claims across sources

- CUAD contains more than 500 contracts and 13,000 expert annotations across 41 label categories, making it a major benchmark for contract review. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]
- Contract review is sparse and high-recall: important clauses can be a small number of pages or sentences inside long documents. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]
- KIRA-style DD passage retrieval has the same high-recall requirement because missing a key legal risk can be more costly than reviewing extra false positives. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Jang & Stikkel (2024) remain the core M&A-specific source because they evaluate PLMs/LLMs directly on M&A DD documents. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Dwivedi & Kamps (2025) extend KIRA-based evaluation to all 50 DD topics and show few-shot LLMs achieve competitive recall (Gemma2: 0.873, Dolphin-Llama3: 0.926) without any labeled training data, strengthening the case for prompt-based legal contract review. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The supervised CRF-PA baseline on the LLM evaluation subset achieves near-perfect precision (0.999) with recall 0.886 and F1 0.938 — the current upper bound for fully supervised legal DD sentence retrieval. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[due-diligence]]
- [[kira-dataset]]
- [[contract-understanding-atticus-dataset]]
- [[maud-dataset]]
- [[hierarchical-sentence-extraction]]
- [[in-context-learning-for-due-diligence]]

## Open questions

- How far can results from generic contract review datasets such as CUAD be transferred to confidential M&A DD data rooms?
- What minimum recall threshold should be acceptable in Legal DD where missing a clause can materially affect transaction terms?
