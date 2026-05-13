---
title: Scaling Laws for LLMs
type: concept
created: 2026-05-05
updated: 2026-05-05
sources: [2026-05-05-zhao-et-al-2023-survey-large-language-models]
aliases: [KM scaling law, Chinchilla scaling law, LLM scaling, neural scaling laws]
---

# Scaling Laws for LLMs

**Empirically derived power-law relationships between a language model's cross-entropy loss and three factors — model size (N), dataset size (D), and training compute (C) — that predict how performance improves with scale and guide compute-optimal training allocation.**

## Summary

Scaling laws are the quantitative foundation for understanding why increasing model size leads to improved LLM performance. Two representative scaling laws are identified in Zhao et al. (2023): the KM scaling law (Kaplan et al. 2020, OpenAI) and the Chinchilla scaling law (Hoffmann et al. 2022, Google DeepMind). [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**KM Scaling Law (Kaplan et al. 2020):** Proposed by the OpenAI team, the KM law models the power-law relationship between cross-entropy loss L and three factors independently:

- L(N) = (N_c / N)^α_N, α_N ≈ 0.076, N_c ≈ 8.8×10^13
- L(D) = (D_c / D)^α_D, α_D ≈ 0.095, D_c ≈ 5.4×10^13
- L(C) = (C_c / C)^α_C, α_C ≈ 0.050, C_c ≈ 3.1×10^8

The three laws were derived by fitting model performance with varied data sizes (22M to 23B tokens), model sizes (768M to 1.5B non-embedding parameters), and training compute. The KM law favors larger budget allocation to model size over data size given a fixed compute budget. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Chinchilla Scaling Law (Hoffmann et al. 2022):** Proposed by the Google DeepMind team as an alternative. Rather than treating the three factors independently, the Chinchilla law fits a joint loss function:

L(N, D) = E + A/N^α + B/D^β

with E = 1.69, A = 406.4, B = 410.7, α = 0.34, β = 0.28. By optimizing L(N, D) under a fixed compute budget C ≈ 6ND, the compute-optimal allocation is:

N_opt(C) = G(C/6)^a, D_opt(C) = G^-1(C/6)^b

The key finding: model size and dataset size should be scaled **equally** for compute-optimal training (similar values of a and b). This contradicts the KM law's preference for model-size-heavy allocation. Empirical proof: Chinchilla (70B parameters, more training tokens) outperforms Gopher (280B parameters) on the same compute budget. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

**Practical implications:** Scaling laws enable (1) predictable scaling — reliable estimation of larger model performance from smaller model experiments; (2) compute-efficient allocation — determining the optimal split of a compute budget between model size and data; (3) training monitoring — identifying abnormal performance early via deviations from the expected scaling curve. The paper also notes diminishing returns as models approach the irreducible loss (entropy of the true data distribution), and the phenomenon of "inverse scaling" where some task performance decreases as language modeling loss decreases. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Variations / sub-concepts

- KM scaling law (Kaplan et al. 2020) — independent per-factor power laws
- Chinchilla scaling law (Hoffmann et al. 2022) — joint model+data law favoring equal scaling
- Task-level scaling — scaling law behavior varies by task metric and can be non-monotone for emergent abilities

## Key claims across sources

- The KM scaling law establishes that model performance has a strong power-law dependence on model size, dataset size, and training compute, providing a basis for predicting larger model performance from smaller experiments. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- The Chinchilla scaling law shows that the KM law over-invests in model size relative to data; compute-optimal training requires equal scaling of both. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- Scaling law describes a smooth, predictable trend of performance improvement, while emergent abilities appear as discontinuous leaps — the two perspectives reflect different performance measurement approaches and may give "misaligned findings." [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related

- [[llm-taxonomy]] — scaling laws explain the PLM-to-LLM generation transition
- [[emergent-abilities-llms]] — the complementary (discontinuous) perspective on model scaling
- [[pre-trained-language-models]] — the model class to which scaling laws are applied
- [[deep-learning]] — the broader neural network framework within which scaling laws operate

## Open questions

- Do scaling laws derived on text data generalize to multimodal or code-heavy training corpora?
- How does the "data-constrained regime" (where public text may be exhausted) affect scaling law applicability?
