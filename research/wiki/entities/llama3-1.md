---
title: Llama 3.1
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [Meta-Llama-3.1-8B, llama3.1, Llama3.1]
entity_kind: model
---

# Llama 3.1

**Meta's open-source LLM family (Dubey et al., 2024); the 8B-parameter variant (Meta-Llama-3.1-8B) was evaluated for legal due diligence passage retrieval across all 50 KIRA topics by Dwivedi & Kamps (2025).**

## Overview

Meta-Llama-3.1-8B is an 8B-parameter open-source model from Meta's Llama 3.1 series (Dubey et al., 2024). It was selected for the Dwivedi & Kamps (2025) study based on performance within the Ollama framework as of July 2024, and was run locally via Ollama for due diligence sentence classification across all 50 KIRA topics. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Llama3.1 benefits substantially from adding more context to prompts. In the Title Only setting it achieves only 0.398 recall, but this rises to 0.818 recall in the few-shot (Title + Description + Examples) setting. The model achieves the best-balanced F1 (0.802) in the few-shot setting among open-source models, comparable to Gemma2 (0.813), and substantially higher than in zero-shot or title-only settings. The Title + Description prompt (without examples) notably boosts precision to 0.894 but constrains recall to 0.617, suggesting the model becomes more conservative with description alone. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- T+D+Examples (50 topics): precision 0.824, recall 0.818, F1 0.802. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Title Only (50 topics): precision 0.666, recall 0.398, F1 0.454. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Three-topic (1086/1244/1247) few-shot: recall 0.75 / 0.98 / 0.77; F1 0.75 / 0.62 / 0.80. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Run via Ollama locally; classified input as 'Relevant' or 'Not Relevant'. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[in-context-learning-for-due-diligence]] — the task it was evaluated on
- [[kira-dataset]] — the benchmark dataset
- [[ollama]] — the local inference platform used to run the model
- [[few-shot-learning]] — prompting strategy producing best results
- [[high-recall-information-retrieval]] — recall-oriented task framing

## Open questions

- How do larger Llama 3.1 variants (70B, 405B) compare on the same KIRA evaluation?
- Does chain-of-thought prompting improve Llama3.1 legal classification accuracy?
