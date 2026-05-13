---
title: Zero-Shot Learning
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [zero-shot prompting, zero-shot inference, zero-shot ICL]
---

# Zero-Shot Learning

**An LLM prompting strategy in which the model is given only a task description (and optionally a topic title) but no labeled examples; the model must generalize to the task from its pre-training knowledge alone.**

## Summary

Zero-shot learning in the context of large language models refers to providing the model with a natural-language task description without any demonstration examples in the prompt. The model is expected to infer the correct classification or generation behavior from the instruction alone, relying on patterns absorbed during pre-training and instruction tuning. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

In the Dwivedi & Kamps (2025) due diligence evaluation, the "Title Only" prompt configuration is effectively a zero-shot setting — the LLM receives only the topic title (e.g., "Evidence of Loans") and is asked to classify sentences as relevant or not. Results across 50 KIRA topics show that zero-shot performance is highly variable and generally lower than few-shot performance, especially for models like Llama3.1 (recall 0.398 in Title Only vs. 0.818 in few-shot) and Dolphin-Llama3 (recall 0.745 vs. 0.926). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Adding a detailed topic description (Title + Description, no examples) substantially improves performance for most models, suggesting that the task-framing signal — not just the label examples — is the critical ingredient for LLM legal classification. This is the first step toward few-shot learning. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key claims across sources

- Zero-shot (Title Only) prompting yields inconsistent and generally lower recall than few-shot prompting for legal DD classification; Llama3.1 recall drops from 0.818 to 0.398 without examples. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- GPT-4o-mini in the Title Only setting achieves recall 0.704, which is its best recall configuration — uniquely, adding examples reduces its recall, suggesting a different sensitivity pattern from open-source models. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Adding a detailed legal description to the Title Only prompt (Title + Description) substantially boosts F1 for Gemma2 (0.678 → 0.778) and GPT-4o-mini (0.735 → 0.756) without requiring any labeled examples. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Variations / sub-concepts

- [[few-shot-learning]] — the natural extension adding labeled examples to the prompt
- Title Only prompt — minimal zero-shot configuration using only the topic name
- Title + Description prompt — enriched zero-shot configuration with expert topic description

## Related

- [[in-context-learning-for-due-diligence]] — the broader ICL paradigm encompassing both zero-shot and few-shot
- [[prompt-engineering]] — the craft of designing effective zero-shot task descriptions
- [[kira-dataset]] — the evaluation benchmark
- [[few-shot-learning]] — the stronger alternative approach

## Open questions

- Is zero-shot performance with detailed descriptions sufficient for preliminary screening of low-stakes DD topics?
- How does zero-shot performance vary across legal jurisdictions and document types outside US credit agreements?
