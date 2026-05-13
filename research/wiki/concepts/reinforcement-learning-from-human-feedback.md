---
title: Reinforcement Learning from Human Feedback
type: concept
created: 2026-05-05
updated: 2026-05-05
sources: [2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [RLHF, alignment tuning, human alignment, RLAIF]
---

# Reinforcement Learning from Human Feedback

**A three-step LLM alignment technique — supervised fine-tuning, reward model training, and RL fine-tuning via PPO — that adapts pre-trained LLMs to produce outputs that are helpful, honest, and harmless according to human preferences; the training method underlying ChatGPT and InstructGPT.**

## Summary

Reinforcement learning from human feedback (RLHF) is proposed to align LLMs with human values (helpfulness, honesty, harmlessness) by fine-tuning on human feedback data. While instruction tuning primarily aims to enhance or unlock LLM abilities, RLHF aims to align LLM behaviors with human values and preferences. The key exemplar systems are InstructGPT (OpenAI, January 2022) and ChatGPT (November 2022). [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Three-step RLHF process (Figure 12 in Zhao et al. 2023):**

1. **Supervised fine-tuning (SFT):** Collect a dataset of prompts and human-written desired outputs. Fine-tune the pre-trained LLM on these examples to initialize desired behavior. InstructGPT uses 175B GPT-3 for this step; labelers compose diverse prompts and write the expected outputs.

2. **Reward model training (RM):** Sample prompts and generate multiple outputs from the SFT model. Human labelers rank outputs from best to worst. Train a reward model (RM) to predict these human preferences. The RM provides learned guidance signals for step 3. InstructGPT uses a 6B GPT-3 as the RM; the RM takes on two forms — a fine-tuned LM or a new LM trained on human preference data.

3. **RL fine-tuning:** Formalize aligning the SFT LLM as a reinforcement learning problem. The LLM is the policy; it takes a prompt as input and returns an output text; the RM provides the reward signal. PPO (Proximal Policy Optimization) is the standard RL algorithm. To avoid diverging too far from the initial LM, a KL divergence penalty is incorporated into the reward. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Key alignment criteria:** Three representative alignment criteria have been widely adopted (from InstructGPT): Helpfulness (assist users in solving their tasks efficiently), Honesty (present accurate content rather than fabricating; convey uncertainty), and Harmlessness (avoid offensive, discriminatory, or dangerous content).

**Alignment tax:** Alignment tuning may harm the general abilities of LLMs to some extent — a potential loss of capability (e.g., in-context learning ability) may be paid as the cost of aligning to human values. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**RLAIF:** A recent variant replaces human labelers with an AI agent (usually an aligned LLM) to generate feedback; this is called "reinforcement learning from AI feedback (RLAIF)." [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Variations / sub-concepts

- InstructGPT — the primary academic RLHF exemplar (OpenAI, 2022)
- ChatGPT — sibling model to InstructGPT, additionally optimized for dialogue
- PPO (Proximal Policy Optimization) — the standard RL algorithm used in RLHF
- RLAIF (Reinforcement Learning from AI Feedback) — variant using AI rather than humans for feedback annotation
- Constitutional AI (Anthropic) — a related alignment approach using explicit AI principles

## Key claims across sources

- RLHF is the training method that produced ChatGPT and InstructGPT; it is the mechanism by which OpenAI ensures LLM outputs are helpful, honest, and harmless. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- ChatGPT was trained similarly to InstructGPT but additionally incorporates human-generated conversations (playing both user and AI roles) combined with InstructGPT data in a dialogue format. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The "alignment tax" — potential loss of general LLM capabilities as a side-effect of RLHF — is a recognized limitation and active research concern. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- PPO-based RLHF training is practically challenging to implement successfully; several strategies for effective reward model training and RL fine-tuning are documented in the survey. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related

- [[instruction-tuning]] — the preceding step in the LLM development pipeline; RLHF typically follows instruction tuning
- [[chatgpt]] — the primary public product built using RLHF
- [[gpt-4]] — also trained with RLHF; alignment is a core design principle
- [[emergent-abilities-llms]] — alignment tuning interacts with emergent abilities via the alignment tax
- [[responsible-ai]] — RLHF is the primary technical mechanism for achieving the "harmlessness" and "helpfulness" requirements of the responsible AI framework
- [[llms-in-ma]] — RLHF-aligned models (ChatGPT, GPT-4) are the LLMs applied to M&A tasks; their alignment properties affect reliability in M&A applications

## Open questions

- Does the alignment tax (loss of general abilities from RLHF) specifically affect finance/M&A domain performance?
- How do RLAIF-trained models compare to human-feedback-trained models for domain-specific business applications?
