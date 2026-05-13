---
title: "A Survey of Large Language Models"
type: source
created: 2026-05-05
updated: 2026-05-05
sources: []
origin: research/input/papers/24595_A_Survey_of_Large_Langua.pdf
author: Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, Yifan Du, Chen Yang, Yushuo Chen, Zhipeng Chen, Jinhao Jiang, Ruiyang Ren, Yifan Li, Xinyu Tang, Zikang Liu, Peiyu Liu, Jian-Yun Nie, Ji-Rong Wen
date: 2023-11-24
aliases: [Zhao et al. 2023, LLM Survey RUC]
---

# A Survey of Large Language Models

**A comprehensive ~100-page academic survey of large language models (LLMs) covering their four-generation taxonomy, pre-training, adaptation tuning, utilization via prompting, and capability evaluation, serving as the de facto foundational reference for LLM taxonomy in the literature.**

> Note: This is an arXiv preprint (arXiv:2303.18223v13, version 13 as of November 24, 2023). It has not been published in a peer-reviewed journal. However, with ~15,000+ citations as of early 2026, it is the most widely cited LLM survey and is routinely treated as a primary reference for definitional and taxonomic claims about LLMs. Authors are primarily from the Gaoling School of Artificial Intelligence and School of Information, Renmin University of China; Jian-Yun Nie is with DIRO, Université de Montréal. Cite as: Zhao et al. (2023).

## Key takeaways

- Language model research has evolved through four distinct generations: Statistical LM (1990s, n-gram/Markov), Neural LM (2013–, word2vec/RNN), Pre-trained LM (2018–, BERT/ELMo/GPT-1/2), and Large Language Model (2020–, GPT-3/PaLM/ChatGPT/GPT-4) — each generation expanding task-solving capacity from "specific task helper" to "general-purpose task solver."
- LLMs exhibit "emergent abilities" — capabilities not present in smaller models that arise unpredictably once model scale crosses a threshold — including in-context learning, instruction following, and step-by-step (chain-of-thought) reasoning.
- Two quantitative scaling laws govern LLM training: the KM scaling law (Kaplan et al. 2020, OpenAI) shows model size, data, and compute each independently follow a power-law; the Chinchilla scaling law (Hoffmann et al. 2022, DeepMind) demonstrates that compute-optimal training requires proportional scaling of both model size and data.
- The dominant LLM development paradigm is pre-training on large diverse corpora followed by adaptation tuning (instruction tuning and/or RLHF), after which models are deployed primarily through a prompting interface — a major shift from the PLM-era practice of task-specific fine-tuning.
- Prompt design is the central technique for utilizing LLMs: zero-shot prompting, few-shot in-context learning, and chain-of-thought prompting each elicit qualitatively different capabilities, and prompt quality directly determines output quality.
- ChatGPT (November 2022) and GPT-4 (March 2023) are identified as the two major milestones of LLM development, triggering widespread AI community and societal attention and rethinking about artificial general intelligence (AGI).
- The survey covers four aspects of LLMs: pre-training (data, architecture, training), adaptation tuning (instruction tuning, RLHF), utilization (prompting strategies), and capability evaluation (benchmarks, tasks).

## Claims

- LLMs are defined in this survey as Transformer language models with significantly large parameter scales (typically tens to hundreds of billions), distinguishing them from smaller PLMs by their emergent abilities. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The four-generation taxonomy of language models (Statistical LM → Neural LM → Pre-trained LM → LLM) is shown in Figure 2 of the paper and maps onto a corresponding progression of task-solving capacity: specific task helper → task-agnostic feature learner → transferable NLP task solver → general-purpose task solver. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Emergent abilities are formally defined as "abilities that are not present in small models but arise in large models," and are identified as one of the most prominent features distinguishing LLMs from PLMs. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- In-context learning (ICL) was formally introduced by GPT-3: given a natural language instruction and/or demonstrations, LLMs generate expected output without requiring additional training or gradient update. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Instruction following enables LLMs fine-tuned on multi-task datasets formatted with natural language descriptions to perform well on unseen tasks described in instructions, without explicit examples. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Chain-of-thought (CoT) prompting — including intermediate reasoning steps — substantially improves LLM performance on complex reasoning tasks and only shows advantages at model sizes above ~60B parameters. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The KM scaling law (Kaplan et al. 2020) established power-law relationships between cross-entropy loss and each of model size (N), dataset size (D), and training compute (C) independently, providing a quantitative basis for predicting larger model performance. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The Chinchilla scaling law (Hoffmann et al. 2022) revised the KM law by showing that model size and number of training tokens should be scaled equally for compute-optimal training; Chinchilla (70B) outperforms Gopher (280B) trained on the same compute by using more training tokens. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The Transformer architecture (Vaswani et al. 2017) is the de facto backbone of all LLMs; three main architectural variants exist: causal decoder (GPT-series), prefix decoder (U-PaLM, GLM-130B), and encoder-decoder (T5, FLAN-T5). [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Instruction tuning is an approach to fine-tuning pre-trained LLMs on formatted instances in the form of natural language; it unlocks emergent abilities and improves generalization to unseen tasks, with diversity and quality of instructions more important than sheer quantity. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Reinforcement learning from human feedback (RLHF) aligns LLMs with human values (helpfulness, honesty, harmlessness) via a three-step process: supervised fine-tuning, reward model training, and RL fine-tuning using PPO; ChatGPT and InstructGPT are the primary exemplars. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- ChatGPT was released in November 2022 as a sibling model to InstructGPT, built on GPT-3.5/GPT-4 series, specially optimized for dialogue, trained with RLHF; it is described as the most powerful chatbot in AI history up to the time of writing. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- GPT-4 was released in March 2023, extended input to multimodal signals, shows stronger capacities on complex tasks than GPT-3.5, and surpasses average human performance on AGIEval (86.4% in 5-shot MMLU). [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- LLaMA (Meta AI, February 2023) is identified as the most popular open-source LLM family, comprising 7B, 13B, 30B, and 65B parameter versions; LLaMA 2 added RLHF and is reported to outperform other open-source models across helpfulness and safety benchmarks. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- LLMs are prone to hallucinations — generating information that either conflicts with the existing source (intrinsic hallucination) or cannot be verified (extrinsic hallucination) — even in the most powerful models such as GPT-4 and ChatGPT. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Entities mentioned

- [[wayne-xin-zhao]]
- [[renmin-university-of-china]]
- [[chatgpt]]
- [[gpt-4]]

## Concepts mentioned

- [[llm-taxonomy]]
- [[scaling-laws]]
- [[emergent-abilities-llms]]
- [[pre-trained-language-models]]
- [[instruction-tuning]]
- [[reinforcement-learning-from-human-feedback]]
- [[prompt-engineering]]
- [[deep-learning]]
- [[llms-in-ma]]

## Notes

Key quotes worth preserving:

- On emergent abilities: "In the literature, emergent abilities of LLMs are formally defined as 'the abilities that are not present in small models but arise in large models', which is one of the most prominent features that distinguish LLMs from previous PLMs." (Section 2.1)

- On in-context learning: "Assuming that the language model has been provided with a natural language instruction and/or several task demonstrations, it can generate the expected output for the test instances by completing the word sequence of input text, without requiring additional training or gradient update." (Section 2.1)

- On the LLM taxonomy: "From the perspective of task solving, the four generations of language models have exhibited different levels of model capacities." (Section 1, Figure 2 caption)

- On the pre-training + prompting paradigm shift: "Unlike small PLMs, the major approach to accessing LLMs is through the prompting interface (e.g., GPT-4 API). Humans have to learn to understand how LLMs work and format their tasks in a way that LLMs can follow." (Section 1)

**Open questions / relevance to seminar paper:**

- For Section 2.2 of the seminar paper ("KI-Verfahren: Einordnung und Relevanz für M&A"), this survey provides the canonical four-generation LLM taxonomy and the definitional framework for "large language model" that should be cited when introducing GPT-4 and ChatGPT in the paper.
- The emergent abilities concept explains why GPT-4 (but not GPT-2) can perform few-shot M&A due diligence classification (Jang & Stikkel 2024) and why fine-tuning adds value for domain-specific tasks (Bozman et al. 2026).
- The RLHF section explains the training mechanism behind ChatGPT and is background for understanding why the model's outputs on M&A sentiment tasks are shaped by human preference data.
- Zhao et al. (2023) is an arXiv preprint — note this explicitly in the seminar paper's bibliography entry and source evaluation; the citation should acknowledge the preprint status while noting the exceptional citation count as justification for use.
- Section 8 (Applications) mentions finance as a domain but does not specifically address M&A — the bridge to M&A applications must be made via the domain-specific papers already in the wiki.
