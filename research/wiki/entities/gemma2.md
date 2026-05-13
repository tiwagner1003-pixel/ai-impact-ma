---
title: Gemma2
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [gemma2-9B, Gemma 2, gemma2-9b]
entity_kind: model
---

# Gemma2

**Google's open-source LLM family (Mesnard et al., 2024) based on Gemini research; the 9B-parameter variant (gemma2-9B) was the best-performing open-source model in Dwivedi & Kamps (2025) for legal due diligence passage retrieval, showing the most balanced precision/recall profile across all 50 KIRA topics.**

## Overview

Gemma2-9B is an open-source model from Google's Gemma 2 family, based on Gemini research and technology (Mesnard et al., 2024). It was selected for the Dwivedi & Kamps (2025) study based on performance within the Ollama framework as of July 2024, and was run locally for due diligence sentence classification. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Gemma2 achieves the best F1 score (0.813) and the best overall precision-recall balance among open-source models in the few-shot setting. Unlike Dolphin-Llama3, which achieves higher recall at the cost of low precision, Gemma2 maintains relatively high precision (0.797) alongside competitive recall (0.873). It was selected as the model for prompt sensitivity analysis because of its strong and consistent baseline performance. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

The prompt sensitivity analysis (four different example sets P1–P4) using Gemma2 found no statistically significant differences across example configurations, confirming robust prompt-level stability. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- T+D+Examples (50 topics): precision 0.797, recall 0.873, F1 0.813 — best open-source F1. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Title Only (50 topics): precision 0.720, recall 0.712, F1 0.678. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Prompt sensitivity (P1–P4): recall stable at 0.873–0.869; no statistically significant variation. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Three-topic few-shot (1086/1244/1247): precision 0.71/0.39/0.83; recall 0.90/0.98/0.77; F1 0.79/0.55/0.80. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Run via Ollama locally; classified as 'Relevant' or 'Not Relevant'. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[in-context-learning-for-due-diligence]] — the task it was evaluated on
- [[kira-dataset]] — the benchmark dataset
- [[ollama]] — the local inference platform used
- [[few-shot-learning]] — prompting paradigm producing best results
- [[high-recall-information-retrieval]] — recall-oriented task framing

## Open questions

- How does Gemma2's prompt stability generalize to tasks outside legal classification?
- Do larger Gemma2 variants (27B) improve recall further at the cost of compute?
