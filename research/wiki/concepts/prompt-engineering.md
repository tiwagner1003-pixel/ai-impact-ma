---
title: Prompt Engineering
type: concept
created: 2026-05-03
updated: 2026-05-05
sources: [2026-05-03-degen-et-al-2024-llms-ma-forecasting, 2026-05-04-bremen-2024-ai-accelerates-ma, 2026-05-05-zhao-et-al-2023-survey-large-language-models, 2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [Prompting, Prompt Design]
---

# Prompt Engineering

**The practice of crafting natural-language instructions (prompts) to steer a large language model's output toward a specific, high-quality result for a given task.**

## Summary

Prompt engineering emerged as a critical skill with the rise of few-shot and zero-shot capable LLMs. Because LLMs respond to the framing, wording, and structure of their inputs, deliberate prompt design can substantially improve output quality, consistency, and task alignment (Brown et al., 2020; Reynolds & McDonell, 2021; White et al., 2024). [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

In finance research applications, prompt engineering determines whether an LLM produces structured, reproducible outputs (e.g., JSON objects with typed fields) or loose, variable text. Degen et al. (2024) use three key prompt engineering choices: (1) role prompting ("As a finance expert…") to orient the model toward domain expertise; (2) a JSON output format requirement for machine-parseable results; and (3) temperature = 0 to suppress stochastic variation and maximize reproducibility. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

The quality of MASS scores is directly dependent on prompt design: the prompt instructs the model to classify M&A relevance (boolean), assign sentiment on a –2 to +2 integer scale, and flag forward-looking statements (boolean) — all in a single API call. The authors note that improvements in prompting strategies represent a clear avenue for future development of the MASS methodology. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Variations / sub-concepts

- Role prompting (assigning a persona to the model)
- [[few-shot-learning]] — providing labeled examples in the prompt
- [[zero-shot-learning]] — task description only, no examples
- Chain-of-thought prompting (requesting reasoning steps)
- Structured output prompting (JSON / XML format enforcement)
- Temperature control (reproducibility vs. creativity tradeoff)

## Key claims across sources

- Prompt framing affects LLM output quality for financial sentiment analysis tasks; role prompting and structured output requirements are key techniques in the MASS methodology. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Setting temperature = 0 in the OpenAI API is used to obtain "answers as objective and reproducible as possible." [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- The authors suggest that deeper prompt engineering insights represent a specific area for future development of LLM-based M&A forecasting tools. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- From a practitioner perspective, M&A leaders use AI prompt engineering to enhance efficiency, focus review on key deal risks, detect unique patterns or discrepancies in diligence data, and identify risk-reduction opportunities — establishing prompt engineering as a practitioner skill, not only a research technique. [[2026-05-04-bremen-2024-ai-accelerates-ma]]

## Related

- [[chatgpt]] — the model whose outputs are shaped by prompt engineering in the MASS study
- [[gpt-4]] — the specific model version
- [[ma-sentiment-analysis]] — the task prompt engineering is applied to
- [[llms-in-ma]] — the broader application domain
- [[sentiment-analysis]] — the NLP parent discipline

## Key claims across sources (continued)

- Unlike smaller PLMs, the major approach to accessing LLMs is through the prompting interface (e.g., GPT-4 API); users must learn to format tasks in ways that LLMs can follow rather than fine-tuning the model on each task. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- In-context learning (ICL) is the fundamental prompting paradigm: given a natural language instruction and/or a few demonstrations, an LLM generates the expected output without gradient updates — introduced formally by GPT-3. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Chain-of-thought (CoT) prompting — incorporating intermediate reasoning steps — substantially improves LLM performance on complex reasoning tasks, but only for models above ~60B parameters; above 100B the advantage is most pronounced. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Task performance in prompting depends strongly on prompt format: adding task descriptions, providing appropriate demonstrations, and including CoT examples each improve generalization — but adding unhelpful components (reasons, suggestions) can have a negligible or adverse effect. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- For legal due diligence, detailed topic descriptions originally written for human annotators (as in the KIRA dataset) are the single most effective prompt component; they matter more than the choice of few-shot examples. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Prompt sensitivity analysis (four example sets, Gemma2 on 50 KIRA topics) finds no statistically significant variation in recall or F1, indicating that few-shot DD prompts are robust to modest example-choice variation. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related (updated)

- [[chatgpt]] — the model whose outputs are shaped by prompt engineering in the MASS study
- [[gpt-4]] — the specific model version
- [[ma-sentiment-analysis]] — the task prompt engineering is applied to
- [[llms-in-ma]] — the broader application domain
- [[sentiment-analysis]] — the NLP parent discipline
- [[emergent-abilities-llms]] — in-context learning and instruction following are the emergent abilities that make prompting effective
- [[instruction-tuning]] — the training-time complement to inference-time prompt design

## Open questions

- Do chain-of-thought prompts improve M&A sentiment classification accuracy compared to the direct single-call approach used in MASS?
- How sensitive is MASS to small wording changes in the prompt (prompt robustness)?
- Does few-shot prompting with example paragraphs improve alignment with human expert consensus?
