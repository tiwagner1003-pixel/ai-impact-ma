---
title: Pre-Trained Language Models
type: concept
created: 2026-05-04
updated: 2026-05-05
sources: [2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence, 2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [PLMs, pretrained language models, BERT, transformer models]
---

# Pre-Trained Language Models

**Neural language models (typically transformer-based) trained on large text corpora in a self-supervised manner, then fine-tuned on downstream tasks; the category includes general-domain models (BERT, GPT) and domain-specific variants (LegalBERT).**

## Summary

Pre-trained language models (PLMs) emerged from the Transformer architecture (Vaswani et al. 2017) and were popularised by BERT (Devlin et al. 2019). The key insight is that large-scale self-supervised pre-training on text produces representations that transfer effectively to a wide range of downstream NLP tasks via fine-tuning. GPT-family models are also PLMs, scaled up and shifted towards autoregressive generation. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

In the legal domain, PLMs were further adapted by training on legal corpora, producing domain-specific variants such as [[legalbert]] (Chalkidis et al. 2020), Lawformer (Xiao et al. 2021), and others. The widespread assumption is that domain-specific pre-training improves performance on legal downstream tasks. However, Jang & Stikkel (2024) find this assumption does not hold for M&A due diligence: LegalBERT does not reliably outperform general-domain BERT on the KIRA dataset, in line with Geng et al. (2021) who similarly found that legal transformer models "may not always help." [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

A structural limitation of standard PLMs (including BERT-class models) for legal DD is their 512-token input limit, which prevents processing full legal documents averaging 3,308 sentences. This limitation motivates the [[hierarchical-sentence-extraction]] architecture. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Variations / sub-concepts

- BERT (general-domain, encoder-only)
- [[legalbert]] (legal-domain, encoder-only)
- Sentence-BERT / all-MiniLM-L6-v2 (sentence embedding model)
- GPT-family (decoder-only, scales to LLM range — see [[gpt-4]])
- Legal LLMs: Lawformer, SaulLM (newer entrants not tested in Jang & Stikkel)

## Key claims across sources

- PLMs based on the Transformer architecture have driven the application of NLP to legal tasks, giving rise to legal-specific variants and benchmark datasets (LexGLUE, ContractNLI). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Legal-domain PLMs (LegalBERT) do not necessarily outperform general-domain PLMs (BERT) on the M&A due diligence sentence classification task. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Standard PLMs are limited to ~512 tokens, making them unsuitable as standalone document processors for long legal documents; hierarchical architectures are required to handle this. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Fine-tuned PLMs can fail entirely on tasks with heavily skewed label distributions (BERT-base as document-level decoder predicts all non-relevant on KIRA), suggesting that model scale and domain-specificity are secondary to task-appropriate architecture and sampling strategies. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Related

- [[legalbert]] — a leading domain-specific legal PLM
- [[deep-learning]] — the broader model family PLMs belong to
- [[hierarchical-sentence-extraction]] — the architecture that uses PLMs as sentence-level encoders
- [[llms-in-ma]] — large-scale PLMs (GPT-4) applied to M&A tasks
- [[due-diligence]] — the legal downstream task evaluated in Jang & Stikkel (2024)
- [[kira-dataset]] — the benchmark dataset on which PLMs were evaluated

## Key claims across sources (continued)

- In the four-generation LM taxonomy, PLMs constitute Generation 3 ("Pre-trained LM," ~2018–), following Statistical LM and Neural LM; they are characterized by the "pre-training + fine-tuning" paradigm and task-solving capacity described as "Transferable NLP task solver." [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- ELMo captured context-aware word representations via biLSTM pre-training; BERT (Devlin et al. 2019) pre-trained bidirectional Transformer models with specially designed pre-training tasks on large-scale unlabeled corpora; GPT-1/2 established the generative pre-training paradigm. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- LLMs (Generation 4) extend PLMs primarily by scale and exhibit emergent abilities absent in smaller PLMs — distinguishing them qualitatively, not merely quantitatively, from Generation 3 models. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related (updated)

- [[legalbert]] — a leading domain-specific legal PLM
- [[deep-learning]] — the broader model family PLMs belong to
- [[hierarchical-sentence-extraction]] — the architecture that uses PLMs as sentence-level encoders
- [[llms-in-ma]] — large-scale PLMs (GPT-4) applied to M&A tasks
- [[due-diligence]] — the legal downstream task evaluated in Jang & Stikkel (2024)
- [[kira-dataset]] — the benchmark dataset on which PLMs were evaluated
- [[llm-taxonomy]] — the four-generation framework positioning PLMs as Generation 3
- [[scaling-laws]] — the quantitative mechanism driving the PLM → LLM transition
- [[emergent-abilities-llms]] — the defining feature LLMs gain that PLMs lack

## Open questions

- How do newer long-context transformer models (e.g., Longformer, BigBird) perform on KIRA compared to the hierarchical Bi-LSTM approach?
- Does the "domain-specific PLMs don't always help" finding generalise to other legal sub-domains beyond due diligence sentence classification?
