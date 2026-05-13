---
title: In-Context Learning for Due Diligence
type: concept
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]
aliases: [ICL for DD, few-shot due diligence prompting, zero-shot due diligence prompting]
---

# In-Context Learning for Due Diligence

**Use of zero-shot or few-shot LLM prompting to classify or retrieve due-diligence-relevant passages without task-specific model training.**

## Summary

In-context learning (ICL) for due diligence exploits LLMs' ability to follow natural-language instructions without gradient-based fine-tuning. The approach is motivated by the scarcity and high cost of labeled DD data: both KIRA and CUAD required months of expert annotation to build, and KIRA access is restricted to academics. ICL allows a practitioner to specify the DD topic through a title and description, optionally add a handful of example sentences, and obtain a classifier with no training pipeline. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]] [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]]

The key practical insight from Dwivedi & Kamps (2025) is that detailed topic descriptions originally written for human legal annotators — already present in the KIRA dataset — transfer directly to LLM prompts. This links AI performance to DD process design: the same structured instructions that guide lawyers also guide models. The paper evaluates five LLMs (Dolphin-Llama3, Gemma2, Llama3.1, GPT-4o-mini, and in a targeted sub-study GPT-4o and DeepSeek-R1:8B) across all 50 KIRA due diligence topics using three prompt configurations: Title Only, Title + Description, and Title + Description + Examples. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

Jang & Stikkel (2024) separately demonstrate GPT-4 few-shot ICL on a single KIRA topic (1243) with 100 samples, achieving recall 0.93–0.96 and F1 0.81–0.82 — outperforming the supervised CRF baseline on F1. Dwivedi & Kamps (2025) substantially extend this by covering all 50 topics, introducing open-source models, and conducting prompt sensitivity and cross-topic robustness analyses. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]

## Key claims across sources

- Few-shot LLMs (Title + Description + Examples) achieve acceptable recall across all 50 KIRA topics with no labeled training data: Dolphin-Llama3 0.926, Gemma2 0.873, Llama3.1 0.818 recall. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Detailed topic descriptions are the single most important prompt component; their inclusion drives larger performance gains than adding example sentences alone. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Open-source models (Gemma2, Llama3.1) perform comparably to closed-source GPT-4o-mini on recall; GPT-4o-mini achieves higher precision but lower recall, making it less suited for high-recall DD. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Cross-topic analysis confirms LLMs rely on topic-specific prompt cues: mismatched prompts (prompt from topic A, data from topic B) cause F1 to approach zero in most cases. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Prompt sensitivity analysis (four example sets P1–P4, Gemma2) shows no statistically significant variation in precision, recall, or F1 — the approach is robust to modest example choice variation. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- GPT-4 (2–8 shots) on KIRA topic 1243: recall 0.93–0.96, F1 0.81–0.82 — outperforms the supervised CRF baseline on both metrics despite using no training data. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- ICL-based approaches are more adaptable to new topics, languages, and jurisdictions than supervised models: adapting prompts requires drafting precise instructions (low cost) vs. annotating extensive corpora (high cost). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Variations / sub-concepts

- [[zero-shot-learning]] — Title Only or Title + Description prompts without examples
- [[few-shot-learning]] — Title + Description + Examples prompts with 3–8 labeled demonstrations

## Related

- [[prompt-engineering]] — the craft of designing effective ICL prompts
- [[legal-contract-review]] — the AI subdomain where ICL is being benchmarked
- [[kira-dataset]] — the primary evaluation benchmark
- [[due-diligence-quality]] — the quality framework within which ICL recall performance is evaluated
- [[pre-trained-language-models]] — the model class enabling ICL
- [[conditional-random-fields]] — the supervised baseline ICL is compared against
- [[high-recall-information-retrieval]] — the task framing demanding recall-first evaluation
- [[few-shot-learning]] — the stronger ICL variant with examples
- [[zero-shot-learning]] — the lower-resource ICL variant without examples

## Open questions

- Are prompt-based DD systems stable enough across topics, languages, and jurisdictions for high-stakes DD workflows? All KIRA data is English-language US credit agreements.
- How should DD teams validate few-shot prompts before using them in live data rooms?
- Can active example selection (choosing examples similar to the test document) improve recall further without training data?
- Would a two-stage pipeline (ICL for high-recall first pass, supervised model for precision re-ranking) outperform either approach alone?
