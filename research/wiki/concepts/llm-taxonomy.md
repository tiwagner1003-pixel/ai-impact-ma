---
title: LLM Taxonomy (Four-Generation Language Model Framework)
type: concept
created: 2026-05-05
updated: 2026-05-05
sources: [2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [four-generation LM taxonomy, language model generations, LM evolution]
---

# LLM Taxonomy (Four-Generation Language Model Framework)

**The canonical four-generation framework for classifying language model research: Statistical LM (1990s), Neural LM (2013–), Pre-trained LM (2018–), and Large Language Model (2020–), each generation expanding the task-solving capacity of language models.**

## Summary

Zhao et al. (2023) define the evolution of language modeling research in terms of four generations, shown in Figure 2 of the survey. The taxonomy maps onto a corresponding progression in task-solving capacity — from narrow, task-specific tools to general-purpose solvers — and provides the foundational categorization used in the LLM literature. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Generation 1 — Statistical Language Models (SLM, ~1990s):** Based on Markov assumption; build word prediction models from n-gram statistics. Representative: bigram and trigram models. Strength: interpretable probability estimation and wide IR/NLP application. Limitation: curse of dimensionality for high-order n-grams; smoothing strategies required (back-off, Good-Turing). Task-solving capacity: "Specific task helper" — assists in specific tasks such as retrieval or speech tasks. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Generation 2 — Neural Language Models (NLM, ~2013–):** Characterize word sequence probability using neural networks (MLP, RNN). Representative: NPLM (Bengio et al. 2003), word2vec (Mikolov et al. 2013), NLPS. Key contribution: distributed representations of words (word vectors). Strength: reduce manual feature engineering; learn context features. Task-solving capacity: "Task-agnostic feature learner" — reduces efforts for human feature engineering. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Generation 3 — Pre-trained Language Models (PLM, ~2018–):** Pre-train context-aware word representations on large-scale corpora using Transformer architecture; fine-tune for downstream tasks. Representative: ELMo (biLSTM), BERT (bidirectional Transformer, 2019), GPT-1/2, BART, T5. Paradigm: "pre-training + fine-tuning." Task-solving capacity: "Transferable NLP task solver" — solves typical NLP tasks. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Generation 4 — Large Language Models (LLM, ~2020–):** Researchers find that scaling PLMs significantly (model size, data size, compute) leads to improved model capacity and qualitatively new "emergent abilities." Representative: GPT-3 (175B), PaLM (540B), Galactica (120B), LLaMA, ChatGPT, GPT-4. Paradigm: "pre-training + adaptation tuning + prompting." Task-solving capacity: "General-purpose task solver" — solves various real-world tasks. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

The key distinguishing claim: LLMs are not simply larger PLMs — they exhibit qualitatively different behaviors (emergent abilities) that smaller PLMs do not possess, making the category distinction meaningful beyond mere parameter count. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Variations / sub-concepts

- [[pre-trained-language-models]] — Generation 3; the immediate predecessor class to LLMs
- [[emergent-abilities-llms]] — the defining qualitative feature of Generation 4
- [[scaling-laws]] — the quantitative mechanism explaining the Generation 3 → 4 transition
- [[deep-learning]] — the broader neural network family underlying Generations 2–4

## Key claims across sources

- The four-generation taxonomy provides the canonical definitional framework for LLMs, distinguishing them from earlier language model classes by emergent abilities rather than parameter count alone. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Each generation corresponds to a specific task-solving capacity: SLM = specific task helper; NLM = task-agnostic feature learner; PLM = transferable NLP task solver; LLM = general-purpose task solver. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- GPT-3 (175B, 2020) is the landmark transition from PLM to LLM, empirically proving that scaling a generative pre-training architecture to significant size can lead to a large increase in model capacity and in-context learning ability. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related

- [[pre-trained-language-models]] — Generation 3; parent concept
- [[scaling-laws]] — the quantitative driver of the PLM-to-LLM transition
- [[emergent-abilities-llms]] — the defining feature of Generation 4 (LLMs)
- [[chatgpt]] — the primary public milestone of the LLM generation
- [[gpt-4]] — the most capable model at time of survey publication
- [[llms-in-ma]] — application of Generation 4 LLMs to M&A tasks

## Open questions

- Does the four-generation taxonomy remain adequate as post-GPT-4 multimodal and agent-based systems emerge?
- Where do retrieval-augmented generation (RAG) systems fit in this taxonomy?
