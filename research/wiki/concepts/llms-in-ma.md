---
title: Large Language Models in M&A
type: concept
created: 2026-05-03
updated: 2026-05-06
sources: [2026-05-03-bachelorseminar-ma-ss2026-syllabus, 2026-05-03-degen-et-al-2024-llms-ma-forecasting, 2026-05-03-zhang-et-al-2024-ai-ma-target-selection, 2026-05-04-singh-2023-ai-transformative-potential-ma, 2026-05-04-bremen-2024-ai-accelerates-ma, 2026-05-04-bain-2024-genai-ma-hope-meets-hype, 2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence, 2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms, 2026-05-05-zhao-et-al-2023-survey-large-language-models, 2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]
aliases: [LLMs in M&A, ChatGPT in M&A, LLM M&A Forecasting]
---

# Large Language Models in M&A

**The application of large language models (LLMs) — including GPT-family models — to M&A tasks such as deal activity forecasting, document analysis, and target identification.**

## Summary

LLMs are a specific AI technology subcategory within the broader [[ai-in-ma]] domain. One of the four prescribed readings for Thema 7 of the SS 2026 seminar — Degen, Kengelbach, Kim, Sievers & Wang (2024), "Large Language Models and M&A: Can ChatGPT help forecast M&A activity?" — focuses specifically on whether LLMs can predict M&A deal activity, making this the most technically precise starting point for the user's paper. [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]

LLM capabilities most relevant to M&A include: natural language processing of deal documents and filings (due diligence automation), text-based extraction of strategic signals from earnings calls and press releases (deal prediction/sourcing), question-answering over large document corpora (data room analysis), and structured information extraction (target profiling). [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]

Degen et al. (2024) empirically demonstrate that ChatGPT (GPT-4.0) applied to 37,549 M&A-relevant paragraphs extracted from earnings call transcripts of S&P Global 1200 companies produces an aggregate M&A Sentiment Score (MASS) that predicts deal volume 18 months ahead. The 18-month lag reflects deal preparation timelines. MASS achieves an out-of-sample R2 of 9.4% and provides incremental predictive power above established sentiment indices and macroeconomic fundamentals. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

This complements the Zhang et al. (2024) paper on classical ML for target selection and synergy prediction, forming a two-technology comparison relevant to Thema 7. Where Degen et al. uses LLMs on unstructured text to predict aggregate deal volume, Zhang et al. uses gradient boosting, SVM, and MLP on structured financial data plus TF-IDF text features to predict individual deal synergy success — the two approaches are methodologically complementary and cover different parts of the M&A AI landscape. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]

## Variations / sub-concepts

- LLM-based M&A deal forecasting
- NLP document review in due diligence
- LLM-assisted synergy identification
- Generative AI in M&A target profiling
- [[ma-sentiment-analysis]] — aggregate sentiment index construction from LLM scoring

## Key claims across sources

- Degen et al. (2024) is the primary academic source specifically testing LLM capabilities for M&A activity forecasting (ChatGPT). [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- LLMs represent a qualitative shift from prior quantitative ML approaches to M&A prediction because they operate on unstructured text rather than structured financial data. [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- GPT-4.0 applied to earnings call transcripts achieves higher M&A sentiment classification alignment with human expert consensus than GPT-4o, GPT-3.5-Turbo, Gemini, Claude, or Perplexity AI. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- The 18-month lag between LLM-extracted M&A sentiment and realized deal volume is the optimal prediction horizon, reflecting deal preparation and execution timelines. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- MASS provides statistically significant incremental predictive power above all four benchmark sentiment indices (Baker-Wurgler, Huang et al., UM CSI, OECD BCI) and above each of six macroeconomic fundamental variables. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- The paper is a working paper (TRR 266 WP No. 150, July 2024; SSRN 4862121), co-authored by BCG practitioners and Paderborn University. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]

## Foundational LLM taxonomy context

The LLMs applied in M&A research (ChatGPT, GPT-4) belong to the fourth generation of language model research as defined by Zhao et al. (2023). The four-generation taxonomy (Statistical LM → Neural LM → Pre-trained LM → LLM) contextualizes why GPT-4-class models can perform M&A tasks that earlier models could not: only the LLM generation exhibits the emergent abilities (in-context learning, instruction following) that enable few-shot document classification, zero-shot sentiment scoring, and instruction-following without fine-tuning on M&A-specific data. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

The pre-training + adaptation tuning + prompting paradigm described in Zhao et al. (2023) directly explains the deployment pattern observed across all wiki M&A sources: (1) GPT-4 is pre-trained on massive corpora, (2) aligned via RLHF (ChatGPT/InstructGPT), (3) accessed through a prompting interface by M&A practitioners and researchers. Fine-tuning on M&A-specific data (as in Bozman et al. 2026) represents the instruction-tuning sub-step. [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]

## Related

- [[ai-in-ma]] — the broader concept this subcategory belongs to
- [[due-diligence]] — due diligence document review is a primary LLM application in M&A
- [[mergers-and-acquisitions]] — the transaction context
- [[ma-success-measurement]] — LLM-assisted processes may improve measurable deal outcomes
- [[ma-sentiment-analysis]] — the specific methodology developed in Degen et al. (2024)
- [[sentiment-analysis]] — the parent NLP discipline
- [[prompt-engineering]] — key technique for structured LLM output in financial text analysis
- [[earnings-conference-calls]] — the primary text corpus for M&A sentiment extraction
- [[mass-index]] — the aggregate index developed by Degen et al.
- [[chatgpt]] — the LLM tool at the center of the MASS study
- [[ml-target-selection]] — the classical ML counterpart to LLM approaches in M&A AI
- [[lightgbm]] — gradient boosting tool used in the Zhang et al. (2024) ML approach
- [[deep-learning]] — neural network family underpinning LLMs and other unstructured-data AI approaches
- [[hierarchical-sentence-extraction]] — recommended architecture for long-document DD when LLMs hit context limits
- [[pre-trained-language-models]] — the broader PLM class; includes BERT, LegalBERT, and GPT-4
- [[kira-dataset]] — the only publicly available M&A DD dataset; primary benchmark for LLM DD evaluation
- [[maud-dataset]] — expert-annotated merger-agreement understanding benchmark with quantitative transformer baselines
- [[merger-agreement-understanding]] — legal reading-comprehension task over M&A deal documents
- [[legalbert]] — legal-domain PLM; does not reliably beat general BERT on DD tasks
- [[memorization-problem-llms]] — fundamental validity challenge for pre-cutoff LLM forecasting tasks
- [[lookahead-bias]] — the broader methodological family; memorization is the LLM-specific structural form
- [[alejandro-lopez-lira]] — lead author of the memorization problem paper
- [[llm-taxonomy]] — the four-generation framework establishing LLMs as Generation 4
- [[emergent-abilities-llms]] — the LLM properties that enable M&A applications (ICL, instruction following)
- [[scaling-laws]] — the quantitative basis for LLM capability growth
- [[instruction-tuning]] — the adaptation technique used in fine-tuned M&A LLMs (Bozman et al. 2026)
- [[reinforcement-learning-from-human-feedback]] — the alignment technique behind ChatGPT and GPT-4
- [[wayne-xin-zhao]] — lead author of the canonical LLM survey providing this taxonomy

## Critical challenge: the memorization problem

A fundamental methodological threat to all LLM-based M&A forecasting studies that use pre-training-cutoff data has been identified by Lopez-Lira, Tang & Zhu (2025). Their paper formally proves (Proposition 1) that when an LLM has seen realized economic outcomes during training, genuine forecasting ability and memorized recall are observationally equivalent — indistinguishable from any observed output. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

> ⚠️ Conflict: [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]] claims that GPT-4.0 extracts genuine managerial private information from earnings calls (2013–2023) to forecast M&A deal volume, interpreting MASS predictive power (out-of-sample R2 = 9.4%) as evidence of LLM forecasting ability. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]] demonstrates that the MASS study's entire sample is within GPT-4o's training period and that M&A sentiment scoring is a future-variant task (judgment of M&A relevance and sentiment would differ with knowledge of which deals actually occurred). The measured predictive power is therefore observationally equivalent to memorization of realized M&A outcomes. Unresolved — no published response from Degen et al. as of this ingest.

M&A sentiment scoring and deal-activity prediction are explicitly classified as "future-variant" tasks by Lopez-Lira et al. (2025): an analyst's judgment of whether an earnings call paragraph signals upcoming M&A activity would change if the analyst knew which deals subsequently materialized. This makes pre-cutoff LLM-based M&A forecasting structurally unreliable regardless of prompt engineering or other in-context controls. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

By contrast, factual extraction tasks — entity identification, numerical data extraction, document structure parsing — are typically future-invariant and remain valid LLM applications even on pre-cutoff data. [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]

## Open questions

- How do LLM predictions of M&A activity compare to traditional econometric models in accuracy?
- Can LLMs process virtual data room contents at sufficient scale and accuracy to replace or augment human due diligence teams?
- What are the confidentiality and data security implications of using cloud-based LLMs in M&A due diligence?
- Can a similar sentiment extraction approach predict individual deal targets rather than only aggregate deal volume?
- From a practitioner perspective, LLMs such as ChatGPT are the most ubiquitous AI entry point for M&A teams, enabling practitioners to incorporate AI into everyday tasks without specialist infrastructure — LLMs are described as a gateway technology for broader AI adoption in M&A deal processes. [[2026-05-04-bremen-2024-ai-accelerates-ma]]
- According to the Bain 2024 survey, GenAI (which includes LLMs) is most widely used in due diligence (58% of current users) and target sourcing/screening (50%), but only 10% of current users apply it in integration execution. [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]]
- A key practical constraint: LLMs depend on available training data, and targets are unlikely to share their internal proprietary data with potential acquirers via GenAI tools — limiting LLM utility in late-stage valuation and due diligence. [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]]
- Jang & Stikkel (2024) provide the first empirical benchmark of LLMs for M&A due diligence document classification; GPT-4 (few-shot) achieves F1 = 0.82 and recall = 0.96 on one KIRA topic, outperforming the CRF baseline on F1 and substantially on recall. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- GPT-4's very high recall in DD screening (0.93–0.96 at 2–8 shots) makes it useful as a first-pass filter that narrows the lawyer's review burden from ~3,300 sentences to a manageable subset; a combined LLM + precision-model pipeline is proposed as the optimal architecture. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- The document-length constraint is the central bottleneck for LLMs in due diligence: the KIRA GPT-4 experiment required simplifying the full-document task to a paragraph-level binary classification (16 sentences per paragraph) to stay within context limits. [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- MAUD extends measurable M&A legal-review evidence beyond KIRA: the best multi-task LegalBERT baseline reaches 76.1% micro-F1 and 59.7% macro-F1 on merger-agreement questions, showing useful but incomplete legal-document understanding. [[2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]]
