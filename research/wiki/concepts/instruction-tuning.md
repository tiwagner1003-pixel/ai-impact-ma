---
title: Instruction Tuning
type: concept
created: 2026-05-05
updated: 2026-05-05
sources: [2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [instruction fine-tuning, supervised fine-tuning, multi-task prompted training]
---

# Instruction Tuning

**A supervised fine-tuning method that trains pre-trained LLMs on a collection of natural-language-formatted task instances (instruction + input + expected output), enabling the model to follow instructions for new, unseen tasks without explicit examples.**

## Summary

Instruction tuning is the approach to fine-tuning pre-trained LLMs on formatted instances in the form of natural language, which is highly related to supervised fine-tuning and multi-task prompted training. The core idea: rather than fine-tuning on task-specific labeled data (the PLM-era paradigm), instruction tuning trains on diverse tasks described in natural language, causing the model to learn to follow instructions as a general capability. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

An instruction-formatted instance consists of: (1) a task description (instruction), (2) optional input, (3) the expected output, and (4) optional demonstrations. Datasets include NLP task datasets (FLAN, P3), daily chat datasets (ShareGPT, OpenAssistant, Dolly), and synthetic datasets (Self-Instruct-52K, Alpaca). [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

Key findings from Zhao et al. (2023):

- **Diversity over quantity:** Diversity and quality of instructions are more important than the number of instances. InstructGPT and LLaMA-2-Chat use fewer but more diverse instructions than Flan-series LLMs, yet perform better.
- **Task generalization:** After instruction tuning, LLMs generalize to related tasks across languages; BLOOMZ-P3 achieves a >50% improvement in multilingual task completion compared to BLOOM, using only English-only instructions.
- **Domain specialization:** Instruction tuning can adapt general LLMs to domain-specific experts — e.g., Med-PaLM (medical), BenTsao and LawGPT (law), and FinGPT (finance) are instruction-tuned variants of general LLMs.
- **Scale interaction:** Larger models benefit more from instruction tuning; LLaMA (13B) instruction-tuned outperforms LLaMA (7B) instruction-tuned on most benchmarks. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

Instruction tuning is less costly than pre-training: the amount of instruction data required is significantly smaller than pre-training data, and parameter-efficient variants (LoRA) can further reduce compute requirements. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Variations / sub-concepts

- NLP task-formatted instruction tuning (FLAN, P3) — best for QA benchmarks
- Chat-formatted instruction tuning (ShareGPT, Dolly, OpenAssistant) — best for conversational tasks
- Synthetic instruction tuning (Self-Instruct, Alpaca) — scalable but lower instruction quality
- Parameter-efficient fine-tuning (LoRA, prefix tuning) — reduces compute cost at slight performance cost
- Multi-stage instruction tuning — task-formatted first, then chat-formatted

## Key claims across sources

- Instruction tuning unlocks the "instruction-following" emergent ability in LLMs, enabling them to generalize to unseen tasks from natural language descriptions without explicit examples. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Diversity and quality of training instructions matter more than sheer quantity; a small but diverse and high-quality instruction set can outperform a large homogeneous one. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Instruction tuning is a general-purpose performance enhancement that works across model architectures and scales, and is much less costly than pre-training. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Finance-domain instruction tuning (FinGPT, BloombergGPT-style approaches) is an active research direction for creating LLMs specialized in financial tasks. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related

- [[reinforcement-learning-from-human-feedback]] — the complementary alignment technique; RLHF typically follows instruction tuning in the LLM development pipeline
- [[emergent-abilities-llms]] — instruction following is one of the three canonical emergent abilities that instruction tuning unlocks
- [[pre-trained-language-models]] — the base models on which instruction tuning is applied
- [[prompt-engineering]] — at inference time, instruction-tuned LLMs respond to prompts; instruction tuning and prompt design are complementary
- [[llms-in-ma]] — instruction-tuned models such as GPT-4 are the LLMs applied to M&A tasks; fine-tuned LLMs for M&A (Bozman et al. 2026) are instruction-tuned on domain-specific data

## Open questions

- What is the minimum viable instruction dataset size and diversity for finance/M&A domain specialization?
- Does instruction tuning on M&A-specific data risk overfitting to historical deal patterns in a way that interacts with the memorization problem?
