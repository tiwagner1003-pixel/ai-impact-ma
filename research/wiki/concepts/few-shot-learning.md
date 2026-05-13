---
title: Few-Shot Learning
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]
aliases: [few-shot prompting, few-shot ICL, few-shot in-context learning]
---

# Few-Shot Learning

**An LLM prompting strategy in which a small number of labeled examples are included in the prompt alongside the task description, enabling the model to adapt its behavior to the task without any gradient-based fine-tuning.**

## Summary

Few-shot learning (in the LLM context) refers to in-context learning with a handful of demonstrations — typically 2–8 labeled input-output pairs — embedded directly in the prompt. The model observes these examples and infers the expected output format and decision boundary for new inputs, without updating any model weights. This approach was introduced at scale by GPT-3 (Brown et al., 2020) and is now standard for adapting LLMs to specialized tasks. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

For legal due diligence, few-shot learning is particularly valuable because annotated training data is scarce, access-restricted, and costly to produce. The KIRA dataset requires academic licensing; CUAD required expensive expert annotation over months. Few-shot prompting allows practitioners to specify a task and provide a handful of examples without any corpus-level annotation — a dramatic reduction in setup cost relative to training supervised models. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

In Dwivedi & Kamps (2025), the Title + Description + Examples prompt configuration (three relevant + three non-relevant example sentences per topic) consistently produces the best recall performance across open-source models. Dolphin-Llama3 reaches 0.926 recall, Gemma2 0.873, and Llama3.1 0.818 — all substantially higher than their zero-shot counterparts. The few-shot examples are drawn from the training split of the KIRA evaluation subset. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Jang & Stikkel (2024) also demonstrate few-shot GPT-4 performance: 2–8 examples yield recall 0.93–0.96 and F1 0.81–0.82 on a single KIRA topic (1243), outperforming the CRF baseline on both recall and F1. This is consistent with Dwivedi & Kamps (2025) in showing that few-shot LLMs can match or exceed CRF recall despite using no training data. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Variations / sub-concepts

- [[zero-shot-learning]] — the weaker variant with no examples
- Title + Description + Examples — the specific three-component prompt structure in Dwivedi & Kamps (2025)
- Prompt sensitivity — robustness of few-shot performance to different example sets (tested with P1–P4 variants using Gemma2)

## Key claims across sources

- Few-shot LLMs (Title + Description + Examples) achieve acceptable recall across all 50 KIRA topics without any domain-specific training data. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Prompt sensitivity analysis (four different example sets) shows no statistically significant variation in Gemma2 performance, indicating robustness to modest example choice variation. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Few-shot learning reduces the dependence on extensive labeled training corpora that has been the primary bottleneck for supervised legal NLP at scale. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Open-source few-shot models (Gemma2, Llama3.1) perform comparably to or exceed closed-source GPT-4o-mini on recall; the open/closed performance gap is smaller than expected. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- GPT-4 few-shot (2–8 examples) on topic 1243: recall 0.93–0.96, F1 0.81–0.82 — superior to the KIRA CRF baseline on both metrics. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- Detailed topic descriptions (from KIRA) are the critical prompt component; examples further improve performance but descriptions alone substantially close the gap with few-shot. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[in-context-learning-for-due-diligence]] — the broader concept encompassing few-shot DD prompting
- [[zero-shot-learning]] — the lower-resource alternative
- [[prompt-engineering]] — the craft of designing effective few-shot prompts
- [[kira-dataset]] — the benchmark for evaluating few-shot legal DD classification
- [[high-recall-information-retrieval]] — the task framing that makes recall the primary optimization target
- [[due-diligence-quality]] — the quality dimension few-shot LLMs partially address

## Open questions

- Does active example selection (choosing examples most similar to the test sentence) substantially improve few-shot recall over random selection?
- Can a practitioner without NLP expertise reliably construct effective few-shot prompts from KIRA-style topic descriptions?
- How does few-shot performance generalize to new legal topics not in the KIRA training distribution?
