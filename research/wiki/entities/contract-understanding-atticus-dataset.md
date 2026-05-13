---
title: Contract Understanding Atticus Dataset
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-hendrycks-et-al-2021-cuad-contract-review]
aliases: [CUAD]
entity_kind: dataset
---

# Contract Understanding Atticus Dataset

**Expert-annotated legal contract review dataset containing 500+ contracts and 13,000+ annotations across 41 clause categories.**

## Overview

CUAD was created by Hendrycks, Burns, Chen & Ball with The Atticus Project to benchmark legal contract review. It asks models to highlight contract passages important for human legal review, such as salient obligations and red-flag clauses. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]

CUAD is relevant to the DD paper as a broader contract-review benchmark. It is not M&A-specific in the way KIRA and MAUD are, but it helps show why Legal DD automation depends on scarce expert annotations and why performance remains imperfect even in well-structured contract tasks. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]

## Key facts

- 500+ contracts, 9,283 pages, 25 contract types. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]
- 13,000+ expert annotations across 41 label categories. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]
- Annotators received 70-100 hours of training and followed 100+ pages of annotation standards. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]
- Each annotation was verified by three additional annotators. [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]

## Related

- [[legal-contract-review]]
- [[the-atticus-project]]
- [[kira-dataset]]
- [[maud-dataset]]
- [[due-diligence-quality]]

## Open questions

- How transferable is CUAD performance to confidential M&A data-room documents?
