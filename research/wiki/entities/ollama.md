---
title: Ollama
type: entity
created: 2026-05-07
updated: 2026-05-07
sources: [2026-05-07-dwivedi-kamps-2025-icl-due-diligence]
aliases: [Ollama platform, ollama-local-runner]
entity_kind: tool
---

# Ollama

**An open-source local large language model runner that enables privacy-preserving, cost-effective inference of open-source models on local hardware without cloud API access.**

## Overview

Ollama is an open-source platform for running LLMs locally (Ollama, 2024). In Dwivedi & Kamps (2025), it was used to run all open-source models (Dolphin-Llama3, Llama3.1, Gemma2, and DeepSeek-R1:8B) for the due diligence passage retrieval experiments. Models were selected based on their performance within the Ollama framework as of July 2024. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

The use of Ollama serves two purposes in the study: (1) data privacy — legal M&A documents should not be sent to external APIs; (2) adaptability to "projects with limited computational resources," enabling inference on non-GPU servers with modest hardware. This makes Ollama-based deployment a realistic path for organizations that cannot or will not send confidential deal documents to cloud services. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Key facts

- Used to run Dolphin-Llama3, Llama3.1, Gemma2, and DeepSeek-R1:8B in the Dwivedi & Kamps (2025) experiments. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Selected for local execution capabilities, data privacy, and adaptability to limited compute. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- Experiments were run on the Dutch National Supercomputer Snellius with SURF/University of Amsterdam HPC Board support. [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]

## Related

- [[dolphin-llama3]] — open-source model run via Ollama
- [[llama3-1]] — open-source model run via Ollama
- [[gemma2]] — open-source model run via Ollama
- [[deepseek-r1]] — open-source model run via Ollama
- [[in-context-learning-for-due-diligence]] — the task it enabled
- [[ai-governance-in-ma]] — data-privacy dimension of local inference in confidential deal workflows

## Open questions

- How does local Ollama inference latency compare to OpenAI API latency for real-time M&A due diligence workflows?
- Which Ollama-supported models are most suitable for production-grade confidential legal document classification?
