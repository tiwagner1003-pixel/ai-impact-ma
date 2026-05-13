---
title: Glassdoor
type: entity
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]
aliases: [Glassdoor.com]
entity_kind: product
---

# Glassdoor

**Online platform where current and former employees anonymously review employers across standardized categories (rating, career opportunities, compensation, work-life balance, diversity, senior management, culture); primary data source for the organizational cultural distance measure in Brede et al. (2025).**

## Overview

Glassdoor.com enables employees to review their employers anonymously, providing 5-star ratings for: Overall Rating, Career Opportunities, Compensation & Benefits, Work/Life Balance, Diversity & Inclusion, Senior Management, and Culture & Values. Reviewers must also provide free-text pros and cons ("Share some of the best reasons [downsides] to work at…"). To ensure review quality, Glassdoor uses a "give to get" policy requiring new users to submit a review or salary information before accessing others' reviews. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

Glassdoor's 5-star ratings are approximately normally distributed (Chemmanur et al. 2019), indicating that reviews are not systematically skewed by response bias. The platform was launched in 2008, which determines the start of the Brede et al. (2025) sample period. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

As a data source for organizational culture research, Glassdoor's key advantages over traditional survey methods are: (1) individual-level data from a broad cross-section of employees (not limited to high-level employees), (2) voluntary and anonymous contributions that reduce social desirability bias, and (3) longitudinal availability across firms. The main limitation is self-selection: reviewers may have particularly strong positive or negative views, and voluntary reviews may not represent the full workforce. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

In Brede et al. (2025), approximately 400,000 Glassdoor reviews from 437 firms were processed using Culture-BERT to construct the organizational cultural distance variable for 243 M&A deals (2008–2021). Firms were matched to the SDC deal database via fuzzy string matching (cosine similarity threshold 0.8; manual verification below threshold). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

## Key facts

- Platform type: employer review aggregator (anonymous, voluntary). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Founded: 2008 (determines sample start for Glassdoor-based M&A research). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Data used in Brede et al. (2025): ~400,000 reviews, 437 firms, pro and con text sections processed by Culture-BERT. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Matching method: fuzzy string matching between Glassdoor company names and SDC deal database (cosine similarity ≥ 0.8 automated; below threshold manually verified). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Key limitation: self-selection bias — reviewers may not represent the full workforce. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

## Related

- [[culture-bert]] — LLM applied to Glassdoor text to produce CVF scores
- [[competing-values-framework]] — cultural taxonomy used to classify reviews
- [[cultural-fit-assessment]] — research application in M&A
- [[marius-brede]] — applied Glassdoor data in the 2025 M&A cultural distance study

## Open questions

- How has Glassdoor's coverage of small/mid-cap firms changed over time?
- Does the "give to get" policy introduce systematic biases compared to open review platforms?
