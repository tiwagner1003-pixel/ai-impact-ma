---
title: ChatGPT
type: entity
created: 2026-05-03
updated: 2026-05-05
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting, 2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [GPT, OpenAI ChatGPT]
entity_kind: tool
---

# ChatGPT

**OpenAI's conversational large language model system based on the GPT (Generative Pre-trained Transformer) architecture, accessed via API for large-scale sentiment analysis tasks in finance research.**

## Overview

ChatGPT is developed by OpenAI and uses the GPT architecture originally described in Vaswani et al. (2017) ("Attention is all you need"). As a large language model, it is trained on a diverse corpus of internet text, enabling coherent, context-sensitive text generation and classification. In Degen et al. (2024), ChatGPT is accessed through the OpenAI API to automate sentiment scoring of 37,549 earnings call paragraphs at scale. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

For the MASS study, the authors tested multiple ChatGPT versions (GPT-4.0, GPT-4o, GPT-3.5-Turbo) alongside competing models (Gemini, Claude, Perplexity AI). GPT-4.0 achieved the highest correlation with human M&A expert consensus and was selected for the main analyses. GPT-3.5-Turbo identified a lower share of paragraphs as M&A-related (53% vs 68% for GPT-4.0) and tended toward higher sentiment scores. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Key facts

- GPT-4.0 (the version used for MASS) correctly classified 68% of paragraphs as M&A-related, average conditional sentiment 0.82; this closely matched human expert consensus (65%, average 0.64). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Temperature set to zero in all MASS analyses to maximize reproducibility; this eliminates stochastic variation in responses. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- ChatGPT is accessible via the OpenAI API, enabling automation of sentiment analysis on tens of thousands of text fragments. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Related

- [[gpt-4]] — the specific model version used in the MASS study
- [[mass-index]] — the index constructed using ChatGPT
- [[prompt-engineering]] — the technique used to frame ChatGPT's scoring task
- [[llms-in-ma]] — the application domain
- [[sentiment-analysis]] — the task ChatGPT performs

## Technical background (Zhao et al. 2023)

Zhao et al. (2023) describe ChatGPT as a sibling model to InstructGPT, built on the GPT-3.5 and GPT-4 series, specially optimized for dialogue via RLHF. It was released in November 2022 and "has attracted widespread attention from society." Training incorporated human-generated conversations where labelers played both user and AI roles, combined with the InstructGPT dataset in a dialogue format. ChatGPT exhibited superior capacities including reasoning on mathematical problems, multi-turn context accuracy, and harmless response generation. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

Key milestones: ChatGPT is identified as one of two major LLM milestones (alongside GPT-4), triggering rethinking of AGI possibilities. The plugin mechanism (enabling external tool integration) was introduced post-launch and described as the "eyes and ears" of LLMs. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related (updated)

- [[gpt-4]] — the specific model version used in the MASS study; the more powerful underlying model
- [[mass-index]] — the index constructed using ChatGPT
- [[prompt-engineering]] — the technique used to frame ChatGPT's scoring task
- [[llms-in-ma]] — the application domain
- [[sentiment-analysis]] — the task ChatGPT performs
- [[reinforcement-learning-from-human-feedback]] — the training mechanism that produced ChatGPT
- [[llm-taxonomy]] — ChatGPT belongs to Generation 4 (LLM) in the four-generation taxonomy

## Open questions

- How does ChatGPT's performance on financial sentiment tasks compare to fine-tuned domain-specific FinLLMs?
- Does the GPT-4.0 advantage over other models persist on newer model generations?
