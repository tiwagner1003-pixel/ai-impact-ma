---
title: LegalBERT
type: entity
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]
aliases: [Legal-BERT, LEGAL-BERT]
entity_kind: model
---

# LegalBERT

**A BERT-based pre-trained language model adapted for legal text, introduced by Chalkidis et al. (2020, EMNLP); Jang & Stikkel (2024) find it does not outperform standard BERT on M&A due diligence classification tasks.**

## Overview

LegalBERT (Chalkidis et al. 2020, "LEGAL-BERT: The Muppets Straight Out of Law School") is a family of BERT models further pre-trained on a large corpus of legal text (legislation, court cases, contracts). It is one of the most widely cited legal-domain PLMs and the standard baseline for evaluating whether domain-specific pre-training benefits legal NLP downstream tasks. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

In the Jang & Stikkel (2024) experiments on the KIRA M&A due diligence dataset, LegalBERT (used as the single-sentence classification encoder) did not demonstrate a substantial performance advantage over standard BERT-base. On topic 1086, LegalBERT achieved F1 = 0.82 vs BERT-base's 0.78; on topic 1244, LegalBERT's F1 dropped to 0.54 vs BERT-base's 0.69 — underperforming the general model on the harder topic. This finding aligns with the results of Geng et al. (2021), who similarly found that legal PLMs do not always help. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

The authors interpret this result as evidence that sequential sentence-level structure (captured by the hierarchical architecture) matters more than encoder domain-specificity for the due diligence task. The extreme label skew in KIRA may also overwhelm domain-specific encoding benefits. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Key facts

- Introduced by Chalkidis et al. (2020), published at EMNLP 2020 (Findings). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- On KIRA topic 1086: LegalBERT F1 = 0.82, BERT-base F1 = 0.78 (LegalBERT marginally better). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- On KIRA topic 1244: LegalBERT F1 = 0.54, BERT-base F1 = 0.69 (LegalBERT underperforms general model). [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- LegalBERT was not tested in context-aware or hierarchical architectures, only single-sentence classification. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Related

- [[pre-trained-language-models]] — the broader model class LegalBERT belongs to
- [[kira-dataset]] — the evaluation dataset where LegalBERT was benchmarked
- [[due-diligence]] — the downstream task evaluated
- [[hierarchical-sentence-extraction]] — the architecture that outperforms both BERT and LegalBERT on DD

## Open questions

- Would LegalBERT fine-tuned on a larger set of KIRA topics show a different pattern?
- Do newer legal LLMs (e.g., Lawformer, SaulLM) outperform general-domain models on M&A due diligence?
