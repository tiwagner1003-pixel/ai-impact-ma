---
title: CrunchBase
type: entity
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-zhang-et-al-2024-ai-ma-target-selection]
aliases: [Crunchbase]
entity_kind: dataset
---

# CrunchBase

**Commercial business data platform providing information on companies, funding rounds, acquisitions, and people; used as the primary data source for the Zhang et al. (2024) ML M&A study.**

## Overview

CrunchBase is a widely used commercial database of company information, funding data, and M&A transaction records. Zhang et al. (2024) assembled their 10,000-deal M&A dataset (2010–2023) from CrunchBase, covering four industries (Technology, Healthcare, Finance, Manufacturing) with 61 features per deal and a 7.3% missing value rate. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

As a data source, CrunchBase's coverage is stronger for venture-backed technology companies than for traditional industrial acquirees, which may introduce selection bias toward tech-sector deals in the Zhang et al. dataset.

## Key facts

- Primary data source for the Zhang et al. (2024) hybrid ML model; 10,000 M&A deals, 2010–2023. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Dataset has 61 raw features and a 7.3% missing value rate. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Industries covered: Technology, Healthcare, Finance, Manufacturing. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Related

- [[ml-target-selection]] — the ML methodology applied to this data
- [[ai-in-ma]] — the research domain

## Open questions

- How representative is CrunchBase of cross-border and non-tech M&A deals?
- What definition of "successful synergy" was used to label deals in this dataset?
