---
title: Emergent Abilities of LLMs
type: concept
created: 2026-05-05
updated: 2026-05-05
sources: [2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [emergent abilities, emergence in LLMs, emergent capabilities]
---

# Emergent Abilities of LLMs

**Capabilities that are absent in smaller language models but arise unpredictably once model scale crosses a threshold — the defining qualitative difference between large language models (LLMs) and their smaller pre-trained language model (PLM) predecessors.**

## Summary

Emergent abilities are formally defined in the LLM literature as "abilities that are not present in small models but arise in large models" (Wei et al. 2022, cited in Zhao et al. 2023). They are one of the most prominent features distinguishing LLMs from PLMs and are described as analogous to the phenomenon of phase transition in physics: performance rises significantly above random when scale reaches a certain level. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

Three canonical emergent abilities are identified by Zhao et al. (2023): [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**1. In-context learning (ICL):** Formally introduced by GPT-3. The LLM, provided with a natural language instruction and/or a few task demonstrations, generates the correct output for test instances without any gradient updates or additional training. ICL is an emergent property: GPT-3 (175B) exhibits strong ICL ability, whereas GPT-1 and GPT-2 do not. The specific capability also depends on the downstream task — for example, ICL for 3-digit arithmetic emerges for the 13B GPT-3, but 175B GPT-3 still fails on Persian QA.

**2. Instruction following:** Fine-tuning LLMs on multi-task datasets formatted with natural language descriptions (instruction tuning) enables the model to follow instructions for new, unseen tasks without explicit examples. This generalizes from training tasks to test tasks via instruction comprehension, not memorization of specific examples. Emerges at approximately 62B+ parameters (for PaLM performance on MMLU, BBH, TyDiQA, MGSM benchmarks).

**3. Step-by-step reasoning (Chain-of-Thought):** Using the CoT prompting strategy — including intermediate reasoning steps in the prompt — enables LLMs to solve complex multi-step tasks (e.g., mathematical word problems) that smaller models cannot handle. This ability appears above ~60B parameters and becomes more pronounced above 100B. An empirical study shows CoT prompting yields gains on PaLM and LaMDA variants above 60B, but not below.

Importantly, emergent abilities cannot be fully characterized by scaling laws alone because they are discontinuous and task-metric-dependent — they appear as sharp leaps rather than smooth curves. Some researchers argue these apparent emergent patterns may partially be artifacts of discontinuous evaluation metrics; altering metrics can make the sharpness disappear. Fundamental research on why emergence occurs remains an open problem. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Variations / sub-concepts

- In-context learning (ICL) — few-shot and zero-shot task solving from demonstrations
- Instruction following — generalizing to unseen tasks via natural language task descriptions
- Step-by-step reasoning / Chain-of-Thought (CoT) — multi-step reasoning via intermediate steps
- Task-level unpredictability — emergent abilities cannot be reliably predicted from scaling laws alone

## Key claims across sources

- Emergent abilities are the defining qualitative distinction between LLMs and smaller PLMs; they are not simply quantitative improvements but qualitatively new capabilities. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- In-context learning was formally introduced by GPT-3 and requires no gradient updates — the model learns from demonstrations embedded in the prompt. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Chain-of-thought prompting only provides performance gains for models above ~60B parameters; smaller models do not benefit from CoT and may even perform worse with it. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The relationship between emergent abilities and scaling laws is subtle: scaling law describes smooth, predictable improvement (measured by language modeling loss), while emergent abilities appear as discontinuous leaps (measured by task performance) — the two perspectives may give misaligned findings. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related

- [[scaling-laws]] — the quantitative framework that predicts continuous performance gains; emergent abilities appear as discontinuous events on top of this trend
- [[llm-taxonomy]] — emergent abilities define the transition from PLM (Generation 3) to LLM (Generation 4)
- [[pre-trained-language-models]] — the predecessor class that lacks emergent abilities
- [[prompt-engineering]] — the practical toolkit for eliciting emergent abilities at inference time
- [[instruction-tuning]] — the adaptation technique that unlocks instruction-following ability
- [[llms-in-ma]] — emergent abilities (especially ICL and instruction following) enable LLM applications in M&A due diligence and deal analysis

## Open questions

- Why do emergent abilities occur in LLMs but not smaller PLMs? This remains a fundamental open research problem.
- Are emergent abilities genuine phase transitions or artifacts of evaluation metric choices?
- Do the same emergence thresholds (~60–100B) apply to domain-specific tasks relevant to M&A?
