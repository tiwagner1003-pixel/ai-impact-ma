---
title: GPT-4o-mini
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [gpt-4o-mini, GPT-4o Mini]
entity_kind: model
---

# GPT-4o-mini

**OpenAI's cost-efficient smaller variant of the GPT-4o family, optimized for fast and less complex tasks; evaluated by Dwivedi & Kamps (2025) for legal due diligence passage retrieval across all 50 KIRA topics.**

## Overview

GPT-4o-mini is OpenAI's smaller, more economical member of the GPT-4o model family. It was selected for the Dwivedi & Kamps (2025) LLM evaluation as a representative closed-source model accessible via the OpenAI API, specifically chosen because it is "optimized for fast and less complex tasks." [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

In the due diligence passage retrieval evaluation across 50 KIRA topics, GPT-4o-mini exhibits a distinctive performance profile: it achieves the highest precision (0.936) in the few-shot setting (Title + Description + Examples) but the lowest recall (0.663) among all tested models. This conservative classification behavior — high precision, lower recall — makes it a stronger fit for precision-oriented tasks than for the high-recall demands of legal due diligence. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

GPT-4o (the larger sibling) was also tested on three representative topics (1086, 1244, 1247) and achieved marginally better F1 scores (0.85 / 0.69 / 0.85) than GPT-4o-mini (0.46 / 0.24 / 0.81 in the same few-shot setting), confirming that scale confers some advantage but that open-source models remain competitive on recall. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- Precision (T+D+Examples, 50 topics): 0.936 — highest of all models tested. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Recall (T+D+Examples, 50 topics): 0.663 — lowest of all models tested. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- F1 (T+D+Examples, 50 topics): 0.754. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Accessed via the OpenAI API; run via standard API inference (no local execution). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[gpt-4]] — the larger GPT-4 family this model belongs to
- [[in-context-learning-for-due-diligence]] — the task it was evaluated on
- [[kira-dataset]] — the benchmark dataset used in the evaluation
- [[few-shot-learning]] — the prompting strategy that produced its best results
- [[high-recall-information-retrieval]] — the recall-oriented task framing where GPT-4o-mini underperforms

## Open questions

- Would fine-tuning GPT-4o-mini on a small set of labeled KIRA examples substantially improve its recall for legal DD?
- Does the precision/recall tradeoff observed here generalize to other legal domains or other languages?
