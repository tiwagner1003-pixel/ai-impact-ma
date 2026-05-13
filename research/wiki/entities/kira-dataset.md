---
title: KIRA Dataset
type: entity
created: 2026-05-04
updated: 2026-05-07
sources: [2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence, 2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding, 2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [KIRA, Roegiest et al. 2018 dataset]
entity_kind: dataset
---

# KIRA Dataset

**The only publicly available dataset for M&A legal due diligence, released by Roegiest, Hudek & McNulty (SIGIR 2018), containing annotated sentence-level relevance labels across 50 legal contract topics; access is restricted to academic use only.**

## Overview

The KIRA dataset was collected and released by Adam Roegiest, Alexander K. Hudek, and Anne McNulty (2018) for the task of identifying relevant passages in legal documents during M&A due diligence. Documents were transformed into text via OCR and each sentence was annotated by KIRA's in-house team, including law students, contract lawyers, and senior in-house lawyers. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

The dataset covers 50 legal contract topics (e.g., "Evidence of Loans", "Collateral/Transaction Security", "EBITDA Definition", "Change of Control") and formulates due diligence as a binary sequential classification task — labelling each sentence as either "relevant" or "non-relevant" for a given topic. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

Two structural characteristics make KIRA extremely challenging for standard NLP methods: (1) documents average 3,308 sentences — far exceeding the 512-token limit of most transformer models — and (2) the label distribution is severely skewed with only 4.8 relevant sentences per document on average, a class imbalance exceeding 99.8% non-relevant instances. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

MAUD does not supersede KIRA; it complements it. KIRA benchmarks sentence-level relevance detection in due diligence documents, while [[maud-dataset]] benchmarks reading comprehension over merger agreement clauses. [[2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]]

Dwivedi & Kamps (2025) revisit KIRA-style DD passage retrieval through a reproducibility study and LLM in-context learning experiments. Their work strengthens the interpretation of KIRA as a high-recall, needle-in-a-haystack legal IR benchmark, and shows that detailed topic descriptions can be repurposed as prompts for LLM-based DD classification. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- Covers 50 legal contract topics across real-world M&A documents. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Average document length: 3,308 sentences (std 473.5). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Average relevant sentences per document: 4.8 (std 5.4). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Average documents without any relevant sentences: 95.4 per topic. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Dataset uses a 5-fold cross-validation structure (1 fold for evaluation, 4 for training, rotated). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Access is firmly restricted to academic usage; obtaining permission requires time and effort, limiting research progress. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Original baseline model: a CRF trained on human-crafted sentence features (Roegiest et al. 2018). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- KIRA topic descriptions can support prompt engineering for zero-shot and few-shot LLM due diligence passage retrieval. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Sentence-level relevance rate per topic ranges from 0.01% to 0.7% — making this one of the most extreme class-imbalance benchmarks in NLP. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The LLM evaluation subset selects all relevant sentences plus 1,000 randomly sampled non-relevant sentences per topic (minimum 240 characters each) for computational feasibility. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Relevant sentences per topic in the evaluation subset range from 15 to 1,307 (median 124, average 210). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Access requires a license request to Zuva (formerly Kira Systems); code for the original study is at [github.com/zuvaai/science](https://github.com/zuvaai/science). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[due-diligence]] — the legal process the dataset is designed to automate
- [[myeongjun-erik-jang]] — used KIRA as primary dataset in the NAACL 2024 study
- [[gabor-stikkel]] — industry collaborator on the NAACL 2024 study
- [[hierarchical-sentence-extraction]] — the architecture that best handles KIRA's document length
- [[pre-trained-language-models]] — the model class evaluated against the KIRA CRF baseline
- [[mergers-and-acquisitions]] — the transaction context from which the documents originate
- [[maud-dataset]] — complementary expert-annotated benchmark for merger-agreement understanding
- [[merger-agreement-understanding]] — related legal NLP task over deal-point clauses
- [[in-context-learning-for-due-diligence]] — prompt-based LLM approach tested on KIRA-style topics

## Open questions

- ~~Has any group published results on all 50 KIRA topics?~~ Resolved: Dwivedi & Kamps (2025) evaluate CRF and LLM baselines across all 50 topics. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- How should KIRA and MAUD be jointly used to measure AI performance across different M&A legal-document tasks?
- Could synthetic data augmentation from LLMs help address the label scarcity problem in KIRA?
- Do KIRA-trained models generalize to non-US, non-English credit agreements and other legal frameworks?
