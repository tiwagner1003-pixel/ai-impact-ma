---
title: "Leveraging Natural Language Processing and Large Language Models for Assisting Due Diligence in the Legal Domain"
type: source
created: 2026-05-04
updated: 2026-05-04
sources: []
origin: research/input/inbox/2024.naacl-industry.14.pdf
author: Myeongjun Erik Jang, Gábor Stikkel
date: 2024-06-16
aliases: [Jang & Stikkel 2024, NAACL 2024 Due Diligence]
---

# Leveraging Natural Language Processing and Large Language Models for Assisting Due Diligence in the Legal Domain

**The first study to apply pre-trained language models (PLMs) and LLMs to M&A due diligence, finding that a hierarchical sentence extraction architecture is the most practically efficient approach and that GPT-4 (few-shot) can meaningfully assist lawyers despite the extreme length and label skew of legal DD documents.**

## Key takeaways

- This is the first published study to employ PLMs and LLMs specifically for the due diligence problem in M&A, filling a gap identified by the scarcity of publicly available DD datasets and lack of NLP research on the topic.
- Due diligence is formulated as a binary sequential classification task: given a legal document, identify which sentences contain relevant information for a specific topic (e.g., "Evidence of Loans", "Collateral/Transaction Security").
- Legal documents in the KIRA dataset average 3,308 sentences per document but only 4.8 sentences are labelled as relevant — an extreme label imbalance (>99.8% non-relevant) that defeats standard NLP approaches.
- Among three architectures tested (single-sentence classification, context-aware classification, hierarchical sentence extraction), the hierarchical approach is the most suitable and practically efficient, because it handles long documents via a two-level encoder and achieves higher recall — the metric that matters most when relevant sentences are so rare.
- Legal-domain PLMs (LegalBERT) do not necessarily outperform general-domain PLMs (BERT) on DD, contradicting the widespread assumption that domain-specific pre-training always helps.
- GPT-4 in a few-shot setting achieves an F1 of 0.82 on one topic (vs. 0.78 for the KIRA CRF baseline), with very high recall (0.96 at 8 shots), demonstrating practical utility as a lawyer-assisting tool despite document-length constraints.
- The KIRA dataset (Roegiest et al. 2018) remains the only publicly available DD dataset; its restrictive academic-access policy limits reproducibility and progress in legal AI for M&A.

## Claims

- To the authors' knowledge, this is the first work leveraging PLMs and LLMs for due diligence in M&A. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- The KIRA dataset frames due diligence as a binary sequential classification task: each sentence in a legal document is labelled "relevant" or "non-relevant" for a given topic. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- KIRA documents average 3,308 sentences (std 473.5) but only 4.8 relevant sentences (std 5.4) — a label ratio exceeding 99.8% non-relevant, creating a severe class imbalance. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Single-sentence BERT and LegalBERT produce comparable or lower F1 than the KIRA CRF baseline, indicating that sentence-level sequential structure is more important than encoder complexity for this task. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- LegalBERT does not exhibit a substantial performance advantage over BERT on KIRA, challenging the assumption that legal-domain pre-training reliably improves legal downstream task performance. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Context-aware classification (incorporating surrounding sentences) performs similarly or worse than single-sentence classification, because the maximum token length limit prevents reliably incorporating all four context sentences for long legal documents. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Fine-tuned BERT-base as document-level decoder in the hierarchical architecture completely fails (predicts all sentences as non-relevant), an overfitting symptom on heavily skewed data; the Bi-LSTM document-level decoder succeeds. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Hierarchical Bi-LSTM models achieve substantially higher recall than the KIRA CRF baseline on four of five topics tested; higher recall is more practically valuable in DD because it minimises missed relevant sentences that lawyers would otherwise need to find manually. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- GPT-4 (2–8 shots) on topic 1243 achieves F1 of 0.81–0.82, recall of 0.93–0.96, and precision of 0.70–0.72, compared to the KIRA-baseline F1 of 0.78 (recall 0.71, precision 0.86). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Increasing the number of few-shot examples from 2 to 8 improves GPT-4 recall from 0.93 to 0.96 while precision remains stable around 0.72. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- A combined pipeline — LLM for high-recall paragraph screening followed by a high-precision model for exact sentence selection — is proposed as an efficient practical architecture for lawyer-assisted DD. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- The KIRA dataset covers 50 topics (legal contract subtopics), contains real-world documents annotated by law students, contract lawyers, and senior in-house lawyers, but is restricted to academic use only and requires formal access approval. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- The study is limited to five of 50 KIRA topics (10%) due to computing constraints and dataset size; broader topic coverage would provide stronger generalisability. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- The industry collaboration between University of Oxford (CS) and Clifford Chance (Data Science Lab) grounds the research in real practitioner requirements and validates practical applicability. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Entities mentioned

- [[myeongjun-erik-jang]]
- [[gabor-stikkel]]
- [[clifford-chance]]
- [[kira-dataset]]
- [[legalbert]]
- [[gpt-4]]

## Concepts mentioned

- [[due-diligence]]
- [[llms-in-ma]]
- [[hierarchical-sentence-extraction]]
- [[pre-trained-language-models]]
- [[mergers-and-acquisitions]]
- [[deep-learning]]
- [[prompt-engineering]]

## Notes

**Key quote (Abstract):** "To our knowledge, this is the first study that employs pre-trained language models (PLMs) and LLMs for the due diligence problem."

**Key quote (Section 4, on LegalBERT):** "LegalBERT did not exhibit a substantial performance advantage over BERT, implying that legal PLMs do not necessarily ensure improved performance in legal-domain downstream tasks."

**Key quote (Section 4, on hierarchical recall):** "The high recall model is more efficient than the high precision model from a practical viewpoint in due diligence, where the 'relevant' sentences account for an extremely small portion."

**Methodological note on GPT-4 experiment:** The GPT-4 experiment was conducted on only one topic (1243: "Collateral/Transaction Security") with 100 sampled examples per run, not the full dataset. This limits the scope of the LLM finding but the direction is clear: high recall, serviceable precision, practical utility. Full-dataset testing "is an extensive resource-consuming work."

**Imbalanced Sampler:** The authors devise a custom sampling strategy (IMBALANCED SAMPLER) using multinomial sampling weighted by inverse class frequency, combined with weighted binary cross-entropy loss, to address the class imbalance problem. The alpha weight (cross-entropy weight) is the most important hyperparameter and is tuned per-topic.

**Relevance to seminar paper (Abschnitt 3.2):** This is the primary empirical source for the section on AI in due diligence. It provides: (1) a formal task formulation for AI-assisted DD; (2) an architecture comparison with actionable recommendations; (3) a specific LLM benchmark (GPT-4 few-shot) with quantitative results; (4) a candid discussion of dataset limitations that constrains the field. Cite as Jang & Stikkel (2024) per Harvard author-date style.

**Open question:** The study's LLM evaluation uses only GPT-4 with a simplified binary paragraph-level task. Could instruction-tuned or fine-tuned LLMs (e.g., GPT-4 fine-tuned on KIRA-accessible data) perform substantially better? The authors suggest a combined LLM + discriminative model pipeline as future work.

**Related future sources to consider:** Roegiest, Hudek & McNulty (2018) for the original KIRA dataset paper; Chitta & Hudek (2019) for a QA-based approach to DD; MAUD dataset (Wang et al. 2023) as a newer legal NLP benchmark for merger agreements.
