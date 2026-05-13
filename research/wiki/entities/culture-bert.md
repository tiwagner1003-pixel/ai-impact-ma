---
title: Culture-BERT
type: entity
created: 2026-05-04
updated: 2026-05-04
sources: [2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]
aliases: [CultureBERT]
entity_kind: model
---

# Culture-BERT

**A RoBERTa-based large language model fine-tuned on 2,000 manually labeled Glassdoor employee reviews to classify text along the four dimensions of the Competing Values Framework (CVF); developed by Koch and Pasch (2022).**

## Overview

Culture-BERT was developed by Koch and Pasch (2022) and builds on the RoBERTa large language model (Liu et al. 2019). It was specifically fine-tuned for the task of measuring organizational culture from textual data, with training labels drawn from 2,000 Glassdoor reviews manually assigned to the four CVF dimensions: Clan, Adhocracy, Market, and Hierarchy. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

The model outputs four probability scores (one per CVF dimension, each ranging from 0 to 1) for any given text input, indicating the extent to which that text reflects each cultural dimension. The authors of Brede et al. (2025) apply Culture-BERT to the merged pro and con text sections of Glassdoor reviews, limiting token length to 300 (median review length: 128 tokens) to account for performance degradation in RoBERTa at longer inputs. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

Culture-BERT has been shown to achieve up to 28% higher accuracy in inferring organizational culture compared to earlier word2vec and LDA-based methods, and outperforms both LDA (Blei et al. 2001) and word2vec (Mikolov et al. 2013) on natural language processing benchmarks due to the transformer attention mechanism's ability to model context, irony, and negation. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

In Brede et al. (2025), Culture-BERT was applied at scale to approximately 400,000 Glassdoor reviews from 437 firms, producing the firm-level CVF scores that serve as the basis for the organizational cultural distance measure across 243 M&A deals (2008–2021). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

## Key facts

- Underlying architecture: RoBERTa (Liu et al. 2019). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Fine-tuning corpus: 2,000 manually labeled Glassdoor reviews (four CVF dimensions). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Output: Four probability scores per review — Clan, Adhocracy, Market, Hierarchy. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Accuracy advantage: up to 28% higher than word2vec-based methods per Koch and Pasch (2022). [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Applied in Brede et al. (2025) to ~400,000 Glassdoor reviews, 437 firms, 243 M&A deals. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- Advantages over LDA/word2vec: handles ironic expressions, negations, and contextual colloquialisms; uses attention to model whole-sentence meaning. [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]

## Related

- [[competing-values-framework]] — the cultural taxonomy Culture-BERT classifies
- [[pre-trained-language-models]] — parent model class (RoBERTa)
- [[glassdoor]] — primary data source for training and application
- [[cultural-fit-assessment]] — downstream use case in M&A
- [[marius-brede]] — applied Culture-BERT in the 2025 M&A study

## Open questions

- Is Culture-BERT publicly available (HuggingFace, GitHub)?
- How does Culture-BERT perform on non-English or non-Glassdoor text sources?
- Would Culture-BERT transfer to other unstructured text types (annual reports, earnings calls) for organizational culture measurement?
