---
title: S&P Global 1200
type: entity
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [S&P 1200, SP Global 1200, S&P Global 1200 Index]
entity_kind: dataset
---

# S&P Global 1200

**A global equity index covering approximately 1,200 large-cap companies across seven regional indices, representing roughly 70% of global stock market capitalization; used as the company universe in Degen et al. (2024) for earnings call transcript collection.**

## Overview

The S&P Global 1200 is a composite index combining the S&P 500 (USA), S&P Europe 350, S&P/TOPIX 150 (Japan), S&P/TSX 60 (Canada), S&P/ASX 50 (Australia), S&P Asia 50, and S&P Latin America 40. It provides broad global coverage of large-cap public companies. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

In the MASS study, the index constituents as of January 2024 are used as the source universe for earnings call transcripts obtained from Refinitiv (LSEG). This creates a survivorship bias: only companies that were in the index as of the collection date are included; firms that were acquired, delisted, or dropped from the index during the 2013–2023 sample period are excluded. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- Approximately 1,200 constituent companies, as of January 2024. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- 39,696 unique earnings call transcripts sourced for these companies from Refinitiv/LSEG, July 2013 – December 2023. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Index level data (SPIDX) and valuation multiple (SPVAL: EV/forward EBITDA) and leverage (SPLEV: net debt/EBITDA) are also used as fundamental control variables. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Survivorship bias risk: January 2024 constituents only. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[mass-index]] — the index built on S&P Global 1200 transcripts
- [[earnings-conference-calls]] — the primary data source extracted from these companies
- [[mergers-and-acquisitions]] — the deal activity being predicted

## Open questions

- Does S&P Global 1200's large-cap bias limit MASS applicability to mid-cap M&A markets?
- How much survivorship bias is introduced by using January 2024 constituents vs. a dynamic rolling constituency?
