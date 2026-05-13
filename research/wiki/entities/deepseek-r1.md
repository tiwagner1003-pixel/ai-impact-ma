---
title: DeepSeek-R1
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [DeepSeek-R1:8B, deepseek-r1-8b]
entity_kind: model
---

# DeepSeek-R1

**Open-source reasoning-focused LLM developed by DeepSeek (Guo et al., 2025), trained with reinforcement learning to incentivize reasoning; the 8B-parameter variant was evaluated for legal due diligence passage retrieval by Dwivedi & Kamps (2025).**

## Overview

DeepSeek-R1 was released shortly before Dwivedi & Kamps (2025) finalized their study. The 8B-parameter variant (DeepSeek-R1:8B) was added to the three-topic targeted analysis (Topics 1086, 1244, 1247) rather than the full 50-topic evaluation, due to time and computational constraints. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

In the few-shot (Title + Description + Examples) setting, DeepSeek-R1:8B shows high recall on all three topics (0.86 / 0.98 / 0.83) but substantially lower precision (0.58 / 0.26 / 0.63), indicating a strong tendency toward overclassification — it flags many non-relevant sentences as relevant. This profile is the inverse of GPT-4o-mini and reflects the model's reasoning-oriented design, which may favor completeness over conservatism. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

The paper notes that DeepSeek-R1:8B is "less effective than the GPT-4o models" overall and that "the closed-source models do not consistently outperform the open-source models" — the open/closed gap is smaller than anticipated. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- Evaluated only on Topics 1086, 1244, and 1247 due to release timing and compute constraints. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- T+D+Examples recall across three topics: 0.86 / 0.98 / 0.83 — very high. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- T+D+Examples precision across three topics: 0.58 / 0.26 / 0.63 — substantially lower than closed-source models. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- T+D+Examples F1 across three topics: 0.69 / 0.41 / 0.72. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Run via Ollama locally; model reference: Guo et al. (2025) CoRR abs/2501.12948. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[in-context-learning-for-due-diligence]] — the task it was evaluated on
- [[kira-dataset]] — the benchmark dataset
- [[high-recall-information-retrieval]] — the recall-oriented framing where DeepSeek-R1 performs well
- [[ollama]] — the local inference platform used to run the model
- [[few-shot-learning]] — the prompting paradigm tested

## Open questions

- Would DeepSeek-R1:8B's overclassification tendency diminish with structured output prompting or calibration?
- How does the full 70B DeepSeek-R1 model perform versus the 8B variant on legal DD tasks?
