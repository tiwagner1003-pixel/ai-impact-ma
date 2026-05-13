---
title: S&P Global 1200
type: entity
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [S&P Global 1200 Index, SPGLOBAL1200]
entity_kind: dataset
---

# S&P Global 1200

**A global equity index covering approximately 1,200 large-cap companies across major markets; used as the sampling frame for the MASS study's earnings call transcript corpus.**

## Overview

The S&P Global 1200 index is a composite index spanning multiple regional S&P indices, covering large-cap equities in developed and selected emerging markets. In Degen et al. (2024), the index constituents as of January 2024 define the universe of companies whose earnings call transcripts are collected via the Refinitiv (LSEG) database. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

The study collected 39,696 unique transcripts from July 2013 to December 2023, then drew a 25% random sample (9,805 transcripts) for processing due to API cost constraints. This introduces a survivorship bias: only companies still in the index as of January 2024 are included, excluding firms acquired or delisted during the sample period. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- Index constituents as of January 2024 define the study universe (survivorship bias risk). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- 39,696 unique transcripts available; 9,805 (25%) drawn as working sample; 9,421 contained M&A keywords; 37,549 M&A-relevant paragraphs identified. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Coverage period: July 2013 to December 2023 (10.5 years, approximately one full M&A market cycle). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Transcript data sourced from Refinitiv (now LSEG). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[mass-index]] — constructed from this index's company transcripts
- [[boston-consulting-group]] — research team that used this data
- [[mergers-and-acquisitions]] — the activity being measured

## Open questions

- Would a broader universe (e.g., S&P Global 3000 or Russell 3000) improve MASS predictive power?
- How does survivorship bias affect the sentiment distribution (presumably, acquired or failed companies had different M&A sentiment patterns)?
