---
title: Conditional Random Fields
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]
aliases: [CRF, CRFsuite, CRF-PA, CRF-LBFGS]
---

# Conditional Random Fields

**A discriminative probabilistic sequence model that labels input tokens or sentences by conditioning on the entire observed sequence; the baseline model class in the Roegiest et al. (2018) M&A due diligence benchmark, implemented via CRFsuite.**

## Summary

Conditional Random Fields (CRFs) are a class of undirected graphical models widely used for sequence labeling in NLP tasks such as named entity recognition and text classification. In the M&A due diligence context, CRFs are applied at the sentence level — each sentence is treated as an independent instance to be classified as relevant or non-relevant for a given legal topic, using hand-crafted token-level and sentence-level features. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

The CRFsuite implementation supports two optimizer variants that are important for the DD task: the Passive-Aggressive (PA) algorithm and the L-BFGS algorithm. PA updates only on misclassified examples, which produces more inclusive (higher-recall) classifiers — a significant advantage for high-recall tasks like legal DD. L-BFGS typically achieves higher precision but lower recall than PA. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Feature engineering is critical to CRF performance in this domain. The Roegiest et al. (2018) original study used a proprietary punkt tokenizer trained on 1M EDGAR documents and word2vec embeddings clustered via k-means — generating domain-specific bigram/trigram features not available to standard NLP pipelines. Dwivedi & Kamps (2025) show that standard text preprocessing reduces CRF-PA sentence-level recall from 0.851 to 0.721, quantifying the value of proprietary feature engineering. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

CRFs remain a strong baseline: the CRF-PA model trained on full KIRA data achieves near-perfect precision (0.999) with recall 0.886 and F1 0.938 on the LLM evaluation subset, representing the upper bound for fully supervised sentence-level DD retrieval. LLMs operating without any labeled training data cannot yet match this F1, but can achieve comparable recall. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Variations / sub-concepts

- CRF-PA (Passive-Aggressive optimizer) — recall-favoring variant, used as primary DD baseline
- CRF-LBFGS — precision-favoring variant
- SVMhmm — Support Vector Machine for sequence modeling, evaluated alongside CRF in Roegiest et al. (2018)
- Vowpal Wabbit — logistic regression classifier using n-gram hashing, also in the Roegiest et al. (2018) study

## Key claims across sources

- CRF-PA achieves sentence-level recall 0.847–0.851 and F1 0.881–0.883 on KIRA, confirming it as a strong high-recall baseline for legal DD. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- CRF models require extensive labeled training data and domain-specific feature engineering; their performance degrades substantially with standard (non-proprietary) preprocessing. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- A Python sklearn-crfsuite implementation reproduces Roegiest et al. (2018) CRF results within two decimal points, confirming cross-framework robustness. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- LLMs evaluated without any labeled training data approach but do not match CRF-PA on F1; on recall specifically, Dolphin-Llama3 in few-shot mode (0.926) exceeds CRF-PA (0.847–0.851). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- For M&A DD, the label distribution is so sparse (0.01–0.7% relevant per topic) that standard accuracy metrics are misleading; recall-focused training objectives like PA are structurally necessary. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Related

- [[kira-dataset]] — the benchmark on which CRF-PA is the primary baseline
- [[feature-engineering]] — the critical differentiator between proprietary and standard CRF performance
- [[high-recall-information-retrieval]] — the task framing that makes PA preferable to L-BFGS
- [[in-context-learning-for-due-diligence]] — the LLM alternative that requires no labeled training data
- [[due-diligence]] — the legal process CRFs are applied to
- [[adam-roegiest]] — lead author of the foundational CRF-based DD study

## Open questions

- Can CRF-style sequential labeling be combined with LLM embeddings (as features) to improve performance without full retraining?
- How do CRF performance levels transfer when applied to non-US, non-English credit agreements?
