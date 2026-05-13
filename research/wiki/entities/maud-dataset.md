---
title: MAUD Dataset
type: entity
created: 2026-05-06
updated: 2026-05-06
sources: [2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]
aliases: [MAUD, Merger Agreement Understanding Dataset]
entity_kind: dataset
---

# MAUD Dataset

**MAUD is an expert-annotated legal NLP dataset for [[merger-agreement-understanding]], introduced by Wang et al. (2023) at EMNLP.**

## Overview

MAUD is built from public merger agreements and deal-point questions inspired by the ABA Public Target Deal Points Study. It contains 39,000+ examples and 47,457 annotations over 152 public merger agreements. [[2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]]

The dataset is relevant to [[due-diligence]] and M&A legal review because it provides a measurable benchmark for AI systems interpreting real merger-agreement clauses rather than only general legal text.

## Key Facts

- Task type: legal reading comprehension over merger agreements.
- Annotation quality: trained law students plus experienced lawyer review.
- Best reported multi-task baseline: LegalBERT with 76.1% micro-F1 and 59.7% macro-F1.
- Main limitation for models: long, complex legal clauses and hard deal-point categories.

## Related

- [[merger-agreement-understanding]]
- [[due-diligence]]
- [[llms-in-ma]]
- [[kira-dataset]]
- [[the-atticus-project]]
- [[steven-wang]]
