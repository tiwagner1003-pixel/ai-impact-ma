---
title: Dolphin-Llama3
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [dolphin-2.9-llama3-8b, Dolphin Llama3, dolphin-llama3-8b]
entity_kind: model
---

# Dolphin-Llama3

**An open-source fine-tuned variant of Llama 3 8B (Hartford, Atkins & Fernandes, 2024), available via Hugging Face; tested in Dwivedi & Kamps (2025) for legal due diligence passage retrieval and notable for achieving the highest recall (0.926) of all models in the few-shot setting at the cost of very low precision.**

## Overview

Dolphin-2.9-Llama3-8B is a community fine-tune of Meta's Llama 3 8B base model, created by Hartford, Atkins & Fernandes (2024) and distributed via Hugging Face (cognitivecomputations/dolphin-2.9-llama3-8b). It was selected for the Dwivedi & Kamps (2025) study based on its performance within the Ollama framework as of July 2024. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Dolphin-Llama3 achieves the highest recall (0.926) of all models tested in the few-shot setting but at a very high cost to precision (0.397), resulting in a low F1 score (0.524). This extreme overclassification — flagging far more sentences as relevant than are actually relevant — makes it unsuitable for stand-alone production use in DD workflows but potentially valuable as a first-pass recall-maximizing filter in a two-stage pipeline. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

The model benefits substantially from adding examples to prompts: in the Title Only setting recall is 0.745 (lower) but adding Title + Description + Examples brings recall to 0.926. This suggests strong sensitivity to in-context guidance. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- T+D+Examples (50 topics): precision 0.397, recall 0.926, F1 0.524 — highest recall, lowest precision. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Title Only (50 topics): precision 0.439, recall 0.745, F1 0.503. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Run via Ollama locally on the Snellius national supercomputer. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[llama3-1]] — the base model family this variant builds on
- [[in-context-learning-for-due-diligence]] — the task it was evaluated on
- [[kira-dataset]] — the benchmark dataset
- [[ollama]] — the local inference platform used
- [[high-recall-information-retrieval]] — the recall-first framing where it excels

## Open questions

- Is Dolphin-Llama3's overclassification structurally linked to its fine-tuning objectives, or is it a prompt-design artifact?
- Could a precision-focused post-filter after Dolphin-Llama3's output yield a usable two-stage DD pipeline?
