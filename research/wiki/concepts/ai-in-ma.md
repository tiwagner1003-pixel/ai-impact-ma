---
title: AI in M&A (Einfluss von KI auf M&A)
type: concept
created: 2026-05-03
updated: 2026-05-07
sources: [2026-05-03-bachelorseminar-ma-ss2026-intro, 2026-05-03-bachelorseminar-ma-ss2026-syllabus, 2026-05-03-einfuehrung-wiss-arbeiten, 2026-05-03-degen-et-al-2024-llms-ma-forecasting, 2026-05-03-zhang-et-al-2024-ai-ma-target-selection, 2026-05-04-bozman-et-al-2026-ai-deal-screening, 2026-05-04-singh-2023-ai-transformative-potential-ma, 2026-05-04-bremen-2024-ai-accelerates-ma, 2026-05-04-bain-2024-genai-ma-hope-meets-hype, 2026-05-04-zhang-et-al-2025-digital-transformation-ma-information-asymmetry, 2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies, 2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]
aliases: [Einfluss von KI auf M&A, Einfluss von AI auf M&A, Thema 7, AI influence on M&A, Artificial Intelligence in Mergers and Acquisitions, Der Einfluss von KI auf M&A]
---

# AI in M&A (Einfluss von KI auf M&A)

**The study of how artificial intelligence technologies influence the full M&A transaction lifecycle — from target identification and due diligence through valuation and post-merger integration.**

## Summary

"Einfluss von AI auf M&A" is Thema 7 of the Goethe-Universitat Frankfurt Bachelor seminar SS 2026. It is positioned in the seminar framework as a horizontal cross-cutting topic, meaning it applies across the entire deal process (not limited to one phase) — parallel to ESG (Thema 6) and spanning the process layer that includes due diligence, takeover tactics, synergy calculation, and post-merger integration. [[2026-05-03-bachelorseminar-ma-ss2026-intro]]

The topic is implicitly broad: because the seminar framework diagram places Thema 7 as a band running beneath the entire process layer, the paper is expected to analyze AI's influence across multiple M&A phases (e.g., AI-assisted target screening, NLP in due diligence, predictive synergy modeling, AI in PMI change management) rather than focusing on a single step. [[2026-05-03-bachelorseminar-ma-ss2026-intro]]

This is the user's assigned seminar paper topic. The paper must be submitted by 2 June 2026, and the group presents on 9 June 2026, 10:00–11:00.

## Variations / sub-concepts

- AI-assisted target identification and deal sourcing
- AI in due diligence (document review, NLP, anomaly detection)
- AI-driven valuation and synergy estimation
- AI in post-merger integration (cultural fit assessment, change management)
- [[llms-in-ma]] — LLMs specifically for deal forecasting, document review, and target profiling
- [[generative-ai-in-ma]] — generative AI (including LLMs) applied to M&A deal processes
- [[xai-explainable-ai]] — explainability as an adoption prerequisite for AI in high-stakes deal decisions
- [[black-box-problem]] — the structural opacity barrier to AI adoption in M&A

## Key claims across sources

- Thema 7 is explicitly framed as a cross-cutting influence topic spanning the full M&A process, not a standalone phase. [[2026-05-03-bachelorseminar-ma-ss2026-intro]]
- The seminar framework positions AI influence as structurally equivalent to ESG influence in its scope across the deal lifecycle. [[2026-05-03-bachelorseminar-ma-ss2026-intro]]
- The official German title of the topic is "Der Einfluss von KI auf M&A" (the intro slides used the Anglicism "AI" rather than the German "KI"). [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- The four prescribed starting readings for Thema 7 are: Bremen (2024, WTW), Degen et al. (2024, LLMs and M&A forecasting), Singh (2022, legal/transformative perspective), and Zheng & Lin Li (2024, ML-based target selection and synergy prediction). [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- Zheng & Lin Li (2024) specifically addresses AI-driven target selection and synergy prediction using machine learning — connecting Thema 7 directly to the Thema 4 (synergy calculation) literature. [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- Degen et al. (2024) tests whether LLMs (ChatGPT) can forecast M&A activity, introducing an NLP/LLM methodology into the deal prediction literature. [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- Degen et al. (2024) is a working paper (TRR 266 Working Paper No. 150, SSRN 4862121, July 2024), not yet peer-reviewed; four of the five authors are BCG practitioners, one is a Paderborn University academic. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- ChatGPT (GPT-4.0) applied to earnings call transcripts achieves statistically significant prediction of aggregate M&A deal volume 18 months ahead, with out-of-sample R2 of 9.4%, demonstrating LLMs can extract managerial private information relevant to M&A forecasting. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- Among LLMs tested for M&A sentiment classification, GPT-4.0 aligns most closely with human M&A expert consensus; Claude (Anthropic) diverges most, with the highest average sentiment score and the lowest M&A identification rate. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- A hybrid ML model (LightGBM + SVM + MLP) trained on 10,000 historical M&A deals achieves AUC-ROC 0.937 and outperforms DCF analysis (Accuracy 0.723), Comparable Company Analysis (0.689), and expert judgment (0.754) at predicting synergy success — providing the first concrete benchmark comparison between AI and traditional M&A methods. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Incorporating text-based NLP features (TF-IDF from company descriptions and press releases) into ML models partially captures qualitative compatibility signals that structured financial data alone misses. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Model interpretability / explainability is a key barrier to practitioner adoption of AI tools in M&A — even high-performing models face skepticism without transparent reasoning for target selection recommendations. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- AI has six distinct application areas in M&A transactions: (1) contract review and due diligence, (2) data analysis and predictive analytics, (3) target identification, (4) market intelligence, (5) automated compliance and regulatory analysis, and (6) expedient post-merger integration. [[2026-05-04-singh-2023-ai-transformative-potential-ma]]
- Over 50% of M&A transactions fail to produce expected results; traditional manual processes have not evolved for decades and are a primary motivation for AI adoption. [[2026-05-04-singh-2023-ai-transformative-potential-ma]]
- AI's role in the negotiation stage of M&A is constrained because human relationships are complicated and dynamic — tactical judgments and interpersonal relationships remain vital and cannot be replaced by AI. [[2026-05-04-singh-2023-ai-transformative-potential-ma]]
- Deep learning models — as trainable, multi-layered neural networks — are specifically suited to handling the unstructured, high-dimensional transaction data characteristic of M&A deals. [[2026-05-04-singh-2023-ai-transformative-potential-ma]]
- At a World Economic Forum panel, both Ginni Rometty (IBM) and Satya Nadella (Microsoft) characterised AI as complementing rather than replacing human capabilities — a framing that anchors AI's role in M&A as augmentative. [[2026-05-04-singh-2023-ai-transformative-potential-ma]]

## Academic writing constraints for Thema 7

Because the paper topic is itself about AI, the academic-writing rules create a notable constraint: AI tools used in writing the paper must be documented in a KI-Verzeichnis, and AI-generated claims cannot substitute for peer-reviewed citations — even when writing about AI capabilities. [[2026-05-03-einfuehrung-wiss-arbeiten]]

AI is explicitly "keine wissenschaftliche Quelle im klassischen Sinne" and the chair warns that AI frequently fabricates bibliographic references ("erfindet oft Literaturangaben"). For a Thema 7 paper this means all claims about AI capabilities in M&A must trace back to verifiable academic or practitioner publications, not to LLM outputs. [[2026-05-03-einfuehrung-wiss-arbeiten]]

## Related

- [[mergers-and-acquisitions]] — the domain AI is being applied to
- [[due-diligence]] — a key phase where AI tools are being deployed
- [[post-merger-integration]] — a key phase where AI has emerging applications
- [[synergy-calculation]] — a phase where AI-driven models are relevant
- [[esg-in-ma]] — parallel cross-cutting topic (Thema 6) in the same seminar
- [[bachelorseminar-ma-ss2026]] — the seminar this topic belongs to
- [[llms-in-ma]] — LLMs as a specific AI technology subcategory within this topic
- [[ml-target-selection]] — classical ML (non-LLM) applied to target screening and synergy prediction
- [[synergy-prediction]] — AI-driven prediction of deal synergy magnitude
- [[feature-engineering]] — the data preparation technique enabling ML models in M&A
- [[gradient-boosting]] — the ML family (LightGBM, XGBoost) most used in M&A tabular models
- [[ma-success-measurement]] — AI adoption may improve measurable M&A outcomes
- [[deep-learning]] — multi-layered neural network AI technique applicable to unstructured M&A data
- [[lean-methodology-in-ma]] — complementary process framework to AI for M&A efficiency improvement
- [[generative-ai-in-ma]] — specific sub-category covering LLMs and GenAI tools in M&A
- [[ai-governance-in-ma]] — governance and risk framework for responsible AI deployment in M&A
- [[willis-towers-watson]] — practitioner firm authoring the Bremen (2024) prescribed reading
- [[information-asymmetry]] — the theoretical mechanism through which digital/AI tools create M&A value
- [[digital-transformation]] — the broader digitalization process of which AI is a component; empirically shown to promote M&A
- [[xai-explainable-ai]] — explainability as the structural adoption prerequisite for AI in high-stakes M&A decisions
- [[black-box-problem]] — the opacity barrier that limits ML model adoption by M&A practitioners and regulators
- [[responsible-ai]] — the overarching framework governing AI deployment in finance and other high-stakes domains
- [[adam-bozman]] — co-author of Bozman et al. (2026) AI deal-screening study
- [[douglas-fairhurst]] — co-author of Bozman et al. (2026) AI deal-screening study
- [[daniel-greene]] — co-author of Bozman et al. (2026) AI deal-screening study
- [[memorization-problem-llms]] — key methodological constraint addressed by the Bozman et al. out-of-sample design
- [[merger-agreement-understanding]] — measurable AI task for interpreting M&A legal deal terms
- [[maud-dataset]] — benchmark evidence for AI performance and error rates in merger-agreement review

## Open questions

- Which specific AI technologies are most relevant: machine learning, NLP, large language models, computer vision, or predictive analytics?
- Does the paper scope include AI as a driver of M&A activity (companies acquiring AI firms) as well as AI as a tool within the M&A process?
- What empirical evidence exists on M&A outcome improvements attributable to AI adoption in deal processes?
- Are there established theoretical frameworks connecting AI capabilities to M&A value creation (e.g., dynamic capabilities, information asymmetry reduction)?
- Are the four prescribed readings mandatory citations, or starting points to be supplemented?
- According to the Bain M&A Practitioners' 2024 Outlook Survey (N≈306), generative AI adoption in M&A deal processes stood at 16% prevalence in early 2024; 80% of respondents expected to use GenAI within three years. [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]] (Note: Bremen 2024 attributes these figures to a "BCG survey" — see conflict callout on [[generative-ai-in-ma]].)
- GenAI usage is concentrated in the early deal phases: 50% of current users apply it to target sourcing/screening, 58% to due diligence, but only 22% to integration planning and 10% to integration execution. [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]]
- 85% of current GenAI users in M&A reported the technology met or exceeded expectations. [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]]
- Efficiency gains from AI in M&A do not automatically translate into better deals; it is what practitioners do with freed-up time that determines value. [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]]
- AI is being deployed across all M&A deal stages: sell-side asset preparation, buy-side target identification, due diligence, and post-merger integration management. [[2026-05-04-bremen-2024-ai-accelerates-ma]]
- Practitioners use AI prompt engineering to detect patterns, flag discrepancies, and focus diligence on key risk areas — making prompt engineering a practitioner skill, not only an academic research tool. [[2026-05-04-bremen-2024-ai-accelerates-ma]]
- AI in M&A is expected to produce job-role shifts (toward higher-value human activities: relationship management, negotiation, strategic decision making) rather than wholesale job elimination; an Evercore ISI / David Shrier report concludes almost every job will be impacted partially. [[2026-05-04-bremen-2024-ai-accelerates-ma]]
- Responsible AI governance in M&A requires a dedicated framework covering confidentiality protection, bias mitigation, ethical usage standards, user education, and jurisdiction-specific regulatory compliance. [[2026-05-04-bremen-2024-ai-accelerates-ma]]
- ~~Are there established theoretical frameworks connecting AI capabilities to M&A value creation?~~ Resolved: Information Asymmetry Theory (Akerlof 1970, Myers-Majluf 1984) provides a well-grounded theoretical mechanism — digital/AI tools reduce external information asymmetry between acquirer and target, lowering barriers to deal initiation and improving valuation accuracy. [[2026-05-04-zhang-et-al-2025-digital-transformation-ma-information-asymmetry]]
- The black-box opacity of high-performing ML models (DNNs, tree ensembles) is a structural adoption barrier in high-stakes financial decisions: decisions that cannot be explained cannot be justified to boards, audited by regulators, or legally defended — this is the core argument for XAI in M&A contexts. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Finance is explicitly identified alongside medicine, law, and defence as a high-stakes domain where XAI is most critical for enabling responsible AI deployment. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Responsible AI — requiring fairness, explainability, accountability, transparency, privacy, ethics, and security simultaneously — is the normative framework for large-scale AI deployment in organizations; XAI is its enabling technical pillar. [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- Corporate digital transformation (a broad measure including AI) significantly promotes M&A activity (deal likelihood, volume, and scale) among Chinese listed companies (2008–2022); the primary causal mechanism is reduction of external information asymmetry between acquirer and target, not transaction cost reduction. [[2026-05-04-zhang-et-al-2025-digital-transformation-ma-information-asymmetry]]
- The effect of digital transformation on M&A is stronger for non-high-tech firms and politically unconnected firms — both groups that lack pre-existing information advantage — indicating that AI/digital tools are a particularly important equaliser for informationally disadvantaged acquirers. [[2026-05-04-zhang-et-al-2025-digital-transformation-ma-information-asymmetry]]
- ~~What is the publication status of Degen et al. (2024)?~~ Resolved: working paper, TRR 266 WP No. 150, SSRN 4862121, July 2024. [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- ~~What empirical evidence exists on M&A outcome improvements attributable to AI adoption?~~ Partially resolved: Zhang et al. (2024) shows a 47% higher PMI success rate and significantly better synergy prediction accuracy vs. traditional benchmarks, though the "success" definition needs scrutiny. [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- Does the paper scope include AI as a driver of M&A activity (companies acquiring AI firms) as well as AI as a process tool?
- ~~Are there established theoretical frameworks connecting AI capabilities to M&A value creation?~~ Resolved above — Information Asymmetry Theory. [[2026-05-04-zhang-et-al-2025-digital-transformation-ma-information-asymmetry]]
- ~~How do classical ML approaches and LLM approaches complement each other across the M&A lifecycle?~~ Partially resolved: Bozman et al. (2026) provide a direct head-to-head comparison under identical training/testing conditions and find ML models outperform baseline LLMs for acquirer-return forecasting; fine-tuning GPT-4o partially closes the gap (3.00% mean return vs. 1.05% for baseline ML). [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- Bozman et al. (2026) show that ML deal screening works significantly better for firms with weaker governance (staggered boards), providing the first empirical evidence that AI counteracts managerial biases (hubris, empire-building) in M&A deal selection. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- AI deal screening is less effective for complex M&A transactions (cross-industry deals), consistent with the broader AI literature on performance degradation under increasing task complexity. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- The out-of-sample testing design in Bozman et al. (2026) — using GPT-4's exogenous September 2021 knowledge cutoff to define the test window — is the most credible available design for LLM-based M&A prediction studies and directly addresses the memorization critique. [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- MAUD provides direct quantitative evidence on AI errors in M&A legal document understanding: even the best reported multi-task baseline remains imperfect at 76.1% micro-F1 / 59.7% macro-F1, especially on complex clauses. [[2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]]
- Does the information-asymmetry framework from Zhang et al. (2025) — developed for Chinese A-share companies — generalise to Western M&A contexts with different disclosure regimes and governance structures?
- What is the journal quality of WJIMT (Zhang et al.'s venue) — is it appropriate as a primary citation in a Goethe seminar paper?
