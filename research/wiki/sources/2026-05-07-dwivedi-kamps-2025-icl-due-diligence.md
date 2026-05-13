---
title: "Effectiveness of In-Context Learning for Due Diligence: A Reproducibility Study of Identifying Passages for Due Diligence"
type: source
created: 2026-05-07
updated: 2026-05-07
sources: []
origin: research/input/papers/dwivedi-kamps-2025-in-context-learning-due-diligence-irrj.pdf
author: Madhukar Dwivedi & Jaap Kamps
date: 2025
aliases: [Dwivedi & Kamps 2025, ICL for Due Diligence, IRRJ 2025 DD]
doi: 10.54195/irrj.22626
journal: Information Retrieval Research, 1, 221–245
---

# Effectiveness of In-Context Learning for Due Diligence

**A reproducibility study that replicates the Roegiest et al. (2018) CRF baseline for legal M&A due diligence passage retrieval and then shows that few-shot LLM prompting achieves acceptable recall across all 50 KIRA topics without any labeled training data.**

## Key takeaways

- Legal due diligence is framed as an extreme high-recall information retrieval problem: the KIRA dataset has only 0.01–0.7% relevant sentences per topic across 15 million sentences in 4,412 documents — a severe needle-in-a-haystack challenge.
- The paper successfully reproduces Roegiest, Hudek & McNulty (2018) CRF results (CRF-PA recall 0.847, F1 0.881 at sentence level) using a Python/sklearn-crfsuite implementation, confirming cross-framework robustness.
- Few-shot LLMs (Title + Description + Examples prompt) achieve competitive recall without any domain-specific training: Dolphin-Llama3 reaches 0.926 recall, Gemma2 reaches 0.873 recall, and Llama3.1 reaches 0.818 recall across 50 topics.
- Detailed KIRA topic descriptions — originally written for human legal annotators — are the single most important prompt component; removing them causes large performance drops.
- Open-source models (Gemma2, Llama3.1) perform comparably to or better than GPT-4o-mini on recall for many topics; GPT-4o is marginally better than GPT-4o-mini but does not dominate open-source models uniformly.
- Generalization across languages, countries, and legal frameworks remains an open question: all KIRA documents are English-language US credit agreements.

## Claims

- Legal due diligence passage retrieval requires extremely high recall because the implications of overlooking key information present a significant financial challenge; precision is secondary to coverage. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The KIRA dataset comprises 4,412 legal M&A documents with over 15 million sentences annotated across 50 due diligence topics; sentence-level relevance rates range from 0.01% to 0.7% per topic. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The LLM evaluation subset was formed by selecting all relevant sentences plus 1,000 randomly sampled non-relevant sentences per topic (minimum 240 characters each) to keep inference computationally feasible. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The Python CRF-PA replication (sklearn-crfsuite) matches the original Roegiest et al. (2018) results to within two decimal points: sentence-level recall 0.851 vs. 0.85 original; annotation-level recall 0.943 vs. 0.94 original. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The Passive-Aggressive (PA) optimizer is favored for CRF training in high-recall tasks because it updates only on errors, producing more inclusive classifications; CRF-LBFGS achieves higher precision but lower recall than CRF-PA. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Using standard text preprocessing (without Kira Systems' proprietary punkt tokenizer and word2vec EDGAR features) reduces CRF-PA sentence-level recall from 0.851 to 0.721 and F1 from 0.881 to 0.809, demonstrating the high value of domain-specific feature engineering. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Across all 50 KIRA topics, few-shot LLMs (Title + Description + Examples) achieve: Dolphin-Llama3 recall 0.926 (F1 0.524), Gemma2 recall 0.873 (F1 0.813), Llama3.1 recall 0.818 (F1 0.802), GPT-4o-mini recall 0.663 (F1 0.754). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- GPT-4o-mini achieves the highest precision (0.936) in the few-shot setting but at the cost of lower recall (0.663); this reflects a conservative classification tendency versus open-source models' tendency toward overclassification. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- In three-topic targeted analysis (Topics 1086, 1244, 1247), GPT-4o achieves F1 0.85/0.69/0.85 and DeepSeek-R1:8B achieves recall 0.86/0.98/0.83 — DeepSeek shows high recall but lower precision (overclassification tendency). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Cross-topic analysis confirms that LLMs rely on topic-specific cues in the prompt: when tested with a mismatched prompt (prompt from one topic, data from another), F1 scores approach zero in most cases. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Prompt sensitivity analysis using four different example sets (P1–P4) in the Gemma2 few-shot setting shows no statistically significant differences in precision, recall, or F1 — the model is robust to modest variations in chosen examples. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- The CRF baseline (trained on full KIRA data) achieves near-perfect precision (0.999) with recall 0.886 and F1 0.938 on the LLM evaluation subset; this is the upper bound for fully supervised models on the same subset. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- LLM-based approaches offer a flexible path to new DD topics and jurisdictions because adapting prompts requires drafting precise instructions (low cost) rather than annotating extensive corpora (high cost). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Code for all experiments is published at [github.com/UAmsterdam/IRRJ_2025](https://github.com/UAmsterdam/IRRJ_2025); the original Roegiest et al. code is at [github.com/zuvaai/science](https://github.com/zuvaai/science). [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Entities mentioned

- [[madhukar-dwivedi]]
- [[jaap-kamps]]
- [[university-of-amsterdam]]
- [[information-retrieval-research]]
- [[kira-dataset]]
- [[gpt-4]]
- [[gpt-4o-mini]]
- [[deepseek-r1]]
- [[llama3-1]]
- [[gemma2]]
- [[dolphin-llama3]]
- [[ollama]]
- [[adam-roegiest]]

## Concepts mentioned

- [[in-context-learning-for-due-diligence]]
- [[legal-contract-review]]
- [[due-diligence]]
- [[hierarchical-sentence-extraction]]
- [[prompt-engineering]]
- [[pre-trained-language-models]]
- [[due-diligence-quality]]
- [[conditional-random-fields]]
- [[high-recall-information-retrieval]]
- [[zero-shot-learning]]
- [[few-shot-learning]]
- [[feature-engineering]]

## Notes

**Citation:** Dwivedi, M. & Kamps, J. (2025). Effectiveness of In-Context Learning for Due Diligence: A Reproducibility Study of Identifying Passages for Due Diligence. *Information Retrieval Research*, 1, 221–245. DOI: 10.54195/irrj.22626

**Relation to Jang & Stikkel (2024):** Dwivedi & Kamps extend Jang & Stikkel by evaluating all 50 KIRA topics (vs. 5 topics in Jang & Stikkel), using smaller open-source models alongside closed-source ones, and focusing more explicitly on the reproducibility dimension. Key added finding: Jang & Stikkel used only one topic (1243) for the LLM analysis with 100 samples, whereas Dwivedi & Kamps use the full evaluation subset across all 50 topics — a substantially broader scope. See [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]].

**Seminar paper relevance:** Chapter 3 (KI-Anwendungen in der Due Diligence): supports the claim that LLMs can achieve high recall for legal DD without labeled training data; provides quantitative benchmarks (recall, F1) directly comparable to CRF baselines; addresses the "Vollständigkeit" (recall/completeness) dimension of DD quality.

**Notable quote from conclusion:** "It is an attractive idea to closely couple the instructions of the human legal professional and the technology-assisted review models used by them, using identical instructions. Compared to annotating extensive corpora, the efforts involved in drafting precise instructions are minimal."

**Open questions flagged by the paper:**

- Generalization to other languages, countries, and legal frameworks (all KIRA data is English-language US credit agreements).
- Transition from sentence-level to passage-level (cleaned-up) data for LLM input.
- Evaluation on a larger set of models and more diverse topic distributions.
- Effect of higher-quality example selection (beyond random sampling) in few-shot prompts.
