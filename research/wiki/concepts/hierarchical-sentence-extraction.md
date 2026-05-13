---
title: Hierarchical Sentence Extraction
type: concept
created: 2026-05-04
updated: 2026-05-07
sources: [2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence, 2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [hierarchical sentence classification, two-level encoder, hierarchical NLP]
---

# Hierarchical Sentence Extraction

**A two-level NLP architecture that first encodes individual sentences into fixed-size vectors and then applies a document-level sequence model to classify each sentence across the full document, enabling processing of very long texts that exceed standard transformer token limits.**

## Summary

Hierarchical sentence extraction addresses a fundamental limitation of transformer-based NLP models: their fixed maximum input length (typically 512 tokens), which is far shorter than real-world legal documents. The standard solution for long documents — truncation — discards most content. The hierarchical approach instead operates at two granularities: a sentence-level encoder (e.g., Sentence-BERT) converts each sentence independently into a dense vector, and a document-level encoder (e.g., Bi-LSTM or BERT) then processes the full sequence of sentence vectors and performs a binary classification decision for each sentence. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

Jang & Stikkel (2024) apply this architecture to M&A due diligence, specifically the task of identifying relevant sentences in legal contract documents from the [[kira-dataset]]. They find it is the most suitable architecture for this task and practically more efficient than the KIRA CRF baseline, primarily because it achieves substantially higher recall — the metric that matters most when relevant sentences constitute less than 0.15% of a document. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

The choice of document-level decoder matters significantly. Fine-tuned BERT-base as the document-level component completely fails on KIRA (predicts all sentences as non-relevant) due to overfitting on the heavily skewed label distribution. The Bi-LSTM decoder succeeds, and simpler Bi-LSTM configurations (fewer layers, lower hidden dimensions) generalise better, confirming that model scale does not always help with real-world skewed data. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Variations / sub-concepts

- Sentence-level encoder (Sentence-BERT/all-MiniLM-L6-v2 used by Jang & Stikkel)
- Document-level encoder: Bi-LSTM (recommended) vs. BERT-base (fails on KIRA)
- Single model vs. ensemble (majority voting over five models)
- Cut-off confidence score tuning (0.5 vs. 0.9 thresholds)

## Key claims across sources

- Hierarchical sentence extraction is the most suitable architecture for M&A due diligence and is practically more efficient than the KIRA CRF baseline. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- The two-encoder structure (sentence-level + document-level) is necessary because legal DD documents average 3,308 sentences, far exceeding standard 512-token limits. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Bi-LSTM document-level decoder outperforms fine-tuned BERT-base decoder in the hierarchical architecture due to overfitting resistance on highly skewed data. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Higher recall is the practical priority in due diligence: a high-recall model allows lawyers to review a small subset of "predicted relevant" sentences to catch false positives, whereas a high-precision/low-recall model forces review of nearly the full document to find missed relevant sentences. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- In-context learning provides an alternative to trained hierarchical classifiers: detailed KIRA topic descriptions can be converted into prompts, allowing LLMs to classify/retrieve due diligence passages with minimal labeled training data. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[pre-trained-language-models]] — the encoder technology underlying the sentence-level component
- [[due-diligence]] — the primary application domain where this architecture is most suitable
- [[kira-dataset]] — the benchmark dataset on which the architecture was evaluated
- [[deep-learning]] — the broader model family this architecture belongs to
- [[legalbert]] — a domain-specific PLM tested in simpler architectures on the same task
- [[in-context-learning-for-due-diligence]] — prompt-based alternative to supervised hierarchical extraction

## Open questions

- Can instruction-tuned LLMs with long-context windows (e.g., GPT-4 Turbo 128k, Claude 3 Opus) replace hierarchical architectures by directly processing full legal documents?
- How does hierarchical extraction performance scale with more KIRA topics beyond the five tested?
