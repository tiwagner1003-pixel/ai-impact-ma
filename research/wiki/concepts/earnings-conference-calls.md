---
title: Earnings Conference Calls
type: concept
created: 2026-05-03
updated: 2026-05-03
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting]
aliases: [Earnings Calls, Conference Call Transcripts, Earnings Call Transcripts]
---

# Earnings Conference Calls

**Quarterly investor calls in which corporate executives discuss financial results and strategic outlook; transcripts of these calls serve as a primary source of managerial private information in textual finance research.**

## Summary

Earnings conference calls are scheduled quarterly events in which a company's management team (typically CEO, CFO, and other C-suite members) presents financial results and forward-looking guidance, followed by a Q&A session with financial analysts and institutional investors. Both sections are transcribed and made available through data providers such as Refinitiv (LSEG). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

In textual analysis research, earnings call transcripts are valued because they contain a mix of prepared statements (management presentation) and more spontaneous responses (Q&A), offering insight into managerial beliefs, expectations, and private information not yet reflected in public filings. Degen et al. (2024) use both sections, arguing that Q&A sessions provide incremental information beyond financial reports and press releases (citing Matsumoto et al., 2011). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

For M&A sentiment extraction specifically, transcripts are filtered using a keyword list (see MASS methodology) to identify paragraphs discussing M&A-related topics. The resulting paragraphs are then scored by an LLM for sentiment and forward-looking content. The key advantage over formal filings (10-K, press releases) is the volume of informal, conversational language in which managers reveal strategic intentions — including M&A sentiment — that would not appear in formal disclosures. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Variations / sub-concepts

- Management presentation section (prepared remarks)
- Q&A section (analyst questions and management answers)
- Forward-looking statements within transcripts
- M&A-relevant paragraph extraction (keyword-filtered subset)

## Key claims across sources

- Both sections of earnings calls (management presentation and Q&A) provide incremental information compared to financial reports and press releases, justifying use of full transcripts. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Earnings call transcripts are the primary source for extracting managerial M&A sentiment in the MASS study; 39,696 unique transcripts from S&P Global 1200 companies are used. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- The 3-month rolling average used in constructing MASS is justified by the quarterly earnings call cadence, ensuring each company contributes one transcript per reporting cycle. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[mass-index]] — the aggregate index derived from earnings call transcript analysis
- [[ma-sentiment-analysis]] — the analytical method applied to transcripts
- [[sp-global-1200]] — the company universe from which transcripts are drawn
- [[llms-in-ma]] — LLMs as the technology for extracting information from transcripts
- [[prompt-engineering]] — the method used to query LLMs on transcript content

## Open questions

- Do earnings calls in non-English languages require language-specific LLMs or translation pipelines for comparable sentiment extraction?
- How does the information content of earnings call M&A sentiment compare to that of formal SEC filings or press releases?
- Is the forward-looking statement classification (the "Future reference" field in the MASS prompt) used in downstream analysis, or only for construct validation?
