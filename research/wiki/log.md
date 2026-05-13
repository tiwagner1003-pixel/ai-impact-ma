# Wiki Log

Append-only chronological record of every wiki operation. Entry prefix is
`## [YYYY-MM-DD HH:MM] <op> | <title>` so the log stays `grep`-parseable:

```
grep "^## \[" research/wiki/log.md | tail -10
```

Valid `<op>` values: `ingest`, `query`, `lint`, `resolve`, `refactor`.

## [2026-05-03 00:00] ingest | Bachelorseminar SS 2026: M&A Prozess und organisatorische Integration — Vorbesprechung
- Source: [[2026-05-03-bachelorseminar-ma-ss2026-intro]]
- New: [[bachelorseminar-ma-ss2026]], [[goethe-universitat-frankfurt]], [[lars-schweizer]], [[ai-in-ma]], [[due-diligence]], [[esg-in-ma]], [[mergers-and-acquisitions]], [[post-merger-integration]], [[synergy-calculation]], [[index]]
- Updated: (none — first ingest)
- Contradictions flagged: none

## [2026-05-03 12:00] ingest | Bachelorseminar M&A SS 2026 — Syllabus mit Literaturliste
- Source: [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]]
- New: [[fti-andersch]], [[merger-waves]], [[ma-success-measurement]], [[llms-in-ma]]
- Updated: [[ai-in-ma]], [[bachelorseminar-ma-ss2026]], [[lars-schweizer]], [[goethe-universitat-frankfurt]], [[mergers-and-acquisitions]], [[synergy-calculation]], [[post-merger-integration]], [[esg-in-ma]], [[due-diligence]], [[index]]
- Contradictions flagged: 1 — see note below

Note on contradiction: The intro slides [[2026-05-03-bachelorseminar-ma-ss2026-intro]] listed Thema 3 as "Due Diligence und Takeover-Taktiken." The authoritative syllabus [[2026-05-03-bachelorseminar-ma-ss2026-syllabus]] shows Thema 3 is "Takeover-Taktiken und Abwehrtechniken" (due diligence is part of Thema 2). The bachelorseminar entity page has been updated to the authoritative syllabus titles. No conflict callout inserted because the syllabus is unambiguously the authoritative document; the intro slides used shorthand labels.

## [2026-05-03 14:00] ingest | Wissenschaftliches Arbeiten: Eine Einführung (SS 2026)
- Source: [[2026-05-03-einfuehrung-wiss-arbeiten]]
- New: [[marco-hochhaus]], [[scientific-writing]], [[citation-style-harvard]], [[literature-research]], [[snowball-method]]
- Updated: [[ai-in-ma]], [[bachelorseminar-ma-ss2026]], [[goethe-universitat-frankfurt]], [[index]]
- Contradictions flagged: none

## [2026-05-03 16:00] ingest | Large Language Models and M&A: Can ChatGPT help forecast M&A activity?
- Source: [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]
- New: [[dominik-degen]], [[jens-kengelbach]], [[soenke-sievers]], [[sp-global-1200]], [[earnings-conference-calls]], [[prompt-engineering]], [[sentiment-analysis]]
- Pre-existing (created in prior partial ingest, now fully populated): [[boston-consulting-group]], [[paderborn-university]], [[chatgpt]], [[gpt-4]], [[mass-index]], [[baker-wurgler-sentiment-index]], [[oecd-business-confidence-index]], [[ma-sentiment-analysis]]
- Updated: [[llms-in-ma]], [[ai-in-ma]], [[merger-waves]], [[index]]
- Contradictions flagged: none

## [2026-05-03 18:00] ingest | AI-Driven M&A Target Selection and Synergy Prediction: A Machine Learning-Based Approach
- Source: [[2026-05-03-zhang-et-al-2024-ai-ma-target-selection]]
- New: [[haodong-zhang]], [[yanli-pu]], [[shuaiqi-zheng]], [[lin-li]], [[wjimt]], [[crunchbase]], [[lightgbm]], [[ml-target-selection]], [[synergy-prediction]], [[gradient-boosting]], [[feature-engineering]]
- Updated: [[ai-in-ma]], [[synergy-calculation]], [[llms-in-ma]], [[index]]
- Contradictions flagged: none
- Note: Syllabus cites this paper as "Zheng & Lin Li (2024)" but full author list is Zhang, Pu, Zheng, Li (Zhang is first author). Flagged on [[shuaiqi-zheng]] and in source page notes. Seminar paper bibliography should use "Zhang et al. (2024)" or list all authors per Harvard style.

## [2026-05-04 00:00] ingest | The Transformative Potential of Artificial Intelligence and its Impact on M&A Transactions
- Source: [[2026-05-04-singh-2023-ai-transformative-potential-ma]]
- New: [[kavya-sanjay-singh]], [[national-law-university-delhi]], [[jus-corpus-law-journal]], [[satya-nadella]], [[ginni-rometty]], [[westlaw]], [[world-economic-forum]], [[deep-learning]], [[lean-methodology-in-ma]]
- Updated: [[ai-in-ma]], [[due-diligence]], [[post-merger-integration]], [[mergers-and-acquisitions]], [[llms-in-ma]], [[index]]
- Contradictions flagged: none
- Note: Singh (2023) is a legal survey paper with no original empirical data. The "Singh (2022)" label in the syllabus follows the Bluebook volume-year convention; the actual publication date is 16 August 2023. Source page includes a citation note explaining both labels.

## [2026-05-04 14:30] ingest | AI accelerates M&A into the future (Bremen 2024, WTW)
- Source: [[2026-05-04-bremen-2024-ai-accelerates-ma]]
- New: [[john-m-bremen]], [[willis-towers-watson]], [[steven-rosenberg]], [[evercore-isi]], [[david-shrier]], [[generative-ai-in-ma]], [[ai-governance-in-ma]]
- Updated: [[ai-in-ma]], [[due-diligence]], [[post-merger-integration]], [[llms-in-ma]], [[prompt-engineering]], [[boston-consulting-group]], [[index]]
- Contradictions flagged: none
- Note: Bremen (2024) is a practitioner thought-leadership article (originally Forbes, 31 May 2024; republished WTW, 26 June 2024), not peer-reviewed. The BCG 16%→80% adoption projection is cited without a specific survey title or methodology — this should not be used as a primary empirical citation in the seminar paper without finding the underlying BCG report. The Evercore ISI / David Shrier report on AI job impact is similarly uncited in full. Both are flagged on their respective entity pages and in the source page Notes.

## [2026-05-04 15:00] ingest | Generative AI in M&A: Where Hope Meets Hype (Bain & Company, January 2024)
- Source: [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]]
- New: [[bain-and-company]], [[ben-siegal]], [[brooke-houston]], [[bain-ma-practitioners-2024-outlook-survey]]
- Updated: [[generative-ai-in-ma]], [[ai-in-ma]], [[due-diligence]], [[llms-in-ma]], [[boston-consulting-group]], [[index]]
- Contradictions flagged: 1 — [[2026-05-04-bremen-2024-ai-accelerates-ma]] attributes the 16%/80% GenAI adoption figures to a "BCG survey"; [[2026-05-04-bain-2024-genai-ma-hope-meets-hype]] presents the same figures as originating from Bain's own M&A Practitioners' 2024 Outlook Survey (N≈306). Conflict callout inserted on [[generative-ai-in-ma]] and [[boston-consulting-group]]. Use Bain article as primary citation; the underlying BCG survey (if any) has not been verified.
- Note: This source is the direct empirical source for the 16%/80% figures widely cited in practitioner commentary. The source provides a three-question GenAI adoption framework and phase-by-phase adoption breakdown (Figure 1) and benefit/risk hierarchy (Figures 2–3). Not peer-reviewed.

## [2026-05-04 17:00] ingest | Does digital transformation affect corporate mergers and acquisitions? From the perspective of information asymmetry
- Source: [[2026-05-04-zhang-et-al-2025-digital-transformation-ma-information-asymmetry]]
- New: [[information-asymmetry]], [[digital-transformation]], [[xinhe-zhang]], [[shujing-yue]], [[jiayi-tao]], [[xiaobing-lai]], [[southeast-university]], [[csmar-database]], [[economic-analysis-and-policy]]
- Updated: [[ai-in-ma]], [[mergers-and-acquisitions]], [[due-diligence]], [[index]]
- Contradictions flagged: none
- Note: Zhang et al. (2025) is the first peer-reviewed source in this wiki to provide an explicit theoretical mechanism (information asymmetry reduction) linking digital/AI tools to M&A activity. Resolves the open question on [[ai-in-ma]] about established theoretical frameworks. Paper is published in *Economic Analysis and Policy* (Elsevier, Vol. 86, 2025, pp. 764–778, DOI: 10.1016/j.eap.2025.03.049). Planned for use in Grundlagenteil 2.2 of the Thema 7 seminar paper.

## [2026-05-04 19:00] ingest | Explainable Artificial Intelligence (XAI): Concepts, taxonomies, opportunities and challenges toward Responsible AI
- Source: [[2026-05-04-arrieta-et-al-2020-xai-concepts-taxonomies]]
- New: [[xai-explainable-ai]], [[black-box-problem]], [[post-hoc-explainability]], [[responsible-ai]], [[alejandro-barredo-arrieta]], [[natalia-diaz-rodriguez]], [[javier-del-ser]], [[information-fusion]]
- Updated: [[deep-learning]], [[ai-governance-in-ma]], [[ai-in-ma]], [[index]]
- Contradictions flagged: none
- Note: Arrieta et al. (2020) is the foundational academic reference for the Kritische Reflexion section of the Thema 7 seminar paper. It provides the theoretical basis for the claim that black-box ML model opacity is a structural (not merely perceptual) barrier to AI adoption in high-stakes financial decisions, and supplies the XAI toolbox (transparent-by-design models vs. post-hoc LIME/SHAP) that practitioners can use to address it. The Responsible AI framework (fairness + explainability + accountability) directly complements the practitioner governance framework documented in [[2026-05-04-bremen-2024-ai-accelerates-ma]]. Published in *Information Fusion*, Vol. 58 (2020), pp. 82–115 (Elsevier, DOI: 10.1016/j.inffus.2019.12.012); 6,000+ citations as of early 2026.

## [2026-05-04 21:00] ingest | Leveraging NLP and LLMs for Assisting Due Diligence in the Legal Domain
- Source: [[2026-05-04-jang-stikkel-2024-nlp-llms-due-diligence]]
- New: [[myeongjun-erik-jang]], [[gabor-stikkel]], [[clifford-chance]], [[kira-dataset]], [[legalbert]], [[hierarchical-sentence-extraction]], [[pre-trained-language-models]]
- Updated: [[due-diligence]], [[llms-in-ma]], [[gpt-4]], [[index]]
- Contradictions flagged: none
- Note: Jang & Stikkel (2024) is the primary empirical source for Abschnitt 3.2 (KI in der Due Diligence) of the Thema 7 seminar paper. Published in NAACL 2024 Industry Track (pp. 155–164); industry collaboration between University of Oxford (CS) and Clifford Chance (Data Science Lab). Key quantitative findings: hierarchical Bi-LSTM > KIRA CRF baseline on recall (4 of 5 topics); LegalBERT does not beat BERT on DD; GPT-4 (8 shots) achieves F1 0.82 / recall 0.96. Cite as Jang & Stikkel (2024) per Harvard author-date. Source available at: https://aclanthology.org/2024.naacl-industry.14/

## [2026-05-04 22:00] ingest | The Memorization Problem: Can We Trust LLMs' Economic Forecasts?
- Source: [[2026-05-04-lopez-lira-et-al-2025-memorization-problem-llms]]
- New: [[memorization-problem-llms]], [[lookahead-bias]], [[alejandro-lopez-lira]], [[yuehua-tang]], [[mingyin-zhu]], [[university-of-florida]]
- Updated: [[llms-in-ma]], [[ma-sentiment-analysis]], [[gpt-4]], [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]], [[index]]
- Contradictions flagged: 1 — Lopez-Lira et al. (2025) directly challenges Degen et al. (2024): the MASS study's entire 2013–2023 sample is within GPT-4o's training period; M&A sentiment scoring is a future-variant task; the measured predictive power is observationally equivalent to memorization of realized M&A outcomes rather than genuine extraction of managerial private information. Conflict callouts inserted on [[ma-sentiment-analysis]], [[llms-in-ma]], [[memorization-problem-llms]], and [[2026-05-03-degen-et-al-2024-llms-ma-forecasting]]. Unresolved — user should determine how prominently to present the challenge in Abschnitt 4 of the seminar paper.

## [2026-05-04 23:30] ingest | Mind the gap: the effect of cultural distance on M&A — evidence from Glassdoor reviews
- Source: [[2026-05-04-brede-et-al-2025-cultural-distance-ma-glassdoor]]
- New: [[marius-brede]], [[hannes-gerstel]], [[arnt-wohrmann]], [[andreas-bausch]], [[review-of-managerial-science]], [[culture-bert]], [[glassdoor]], [[competing-values-framework]], [[cultural-fit-assessment]]
- Updated: [[post-merger-integration]], [[index]]
- Contradictions flagged: none

## [2026-05-04 23:59] ingest | The Future of Mergers & Acquisitions? Risk Allocation in AI-Guided Transactions
- Source: [[2026-05-04-herbosch-mertens-2025-risk-allocation-ai-ma]]
- New: [[maarten-herbosch]], [[floris-mertens]], [[ku-leuven]], [[ghent-university]], [[eu-ai-act]], [[business-judgment-rule]], [[ai-liability-ma]]
- Updated: [[ai-governance-in-ma]], [[responsible-ai]], [[index]]
- Contradictions flagged: none
- Note: SSRN working paper (not yet peer-reviewed). The 97% Deloitte due diligence adoption figure and ~80% M&A professional AI adoption forecast are cited from the paper's introduction (Deloitte 2025 M&A Trends Survey and Bain & Company 2024 respectively); the Deloitte 2025 survey has not been separately ingested. Paper belongs in Abschnitt 4 (Kritische Reflexion) of the Thema 7 seminar paper; provides the most legally rigorous five-jurisdiction treatment of AI governance obligations and liability exposure in M&A available in the prescribed reading list. No conflicts with existing wiki content; the explainability-as-legal-safeguard claim reinforces and extends prior entries in [[ai-governance-in-ma]] and [[responsible-ai]] from a comparative law perspective.

## [2026-05-04 14:00] ingest | Better Than a Coin Flip? Screening Mergers and Acquisitions With Artificial Intelligence Models
- Source: [[2026-05-04-bozman-et-al-2026-ai-deal-screening]]
- New: [[adam-bozman]], [[douglas-fairhurst]], [[daniel-greene]], [[washington-state-university]], [[clemson-university]]
- Updated: [[ml-target-selection]], [[ai-in-ma]], [[memorization-problem-llms]], [[gradient-boosting]], [[gpt-4]], [[index]]
- Contradictions flagged: none
- Note: SSRN Working Paper 5421737 (first draft April 2024, this draft March 2026, not yet peer-reviewed). JEL G30, G34. Primary empirical anchor for Abschnitt 3.1 (KI in der Target-Identifikation und Deal-Sourcing) of the Thema 7 seminar paper. The paper's out-of-sample design (October 2021 – December 2024, after GPT-4's September 2021 training cutoff) is the most credible LLM-in-M&A methodology in this wiki and directly addresses the memorization critique from Lopez-Lira et al. (2025). ML models outperform baseline LLMs; fine-tuned GPT-4o partially closes the gap. Governance moderation result (AI more useful for weak-governance firms) is novel and policy-relevant. No conflicts with existing wiki content — Bozman et al. results are complementary to and consistent with Zhang et al. (2024) and Degen et al. (2024), addressing a different prediction task (announcement returns vs. synergy prediction vs. aggregate M&A volume).

## [2026-05-05 12:00] ingest | A Survey of Large Language Models (Zhao et al. 2023)
- Source: [[2026-05-05-zhao-et-al-2023-survey-large-language-models]]
- New: [[wayne-xin-zhao]], [[renmin-university-of-china]], [[llm-taxonomy]], [[scaling-laws]], [[emergent-abilities-llms]], [[instruction-tuning]], [[reinforcement-learning-from-human-feedback]]
- Updated: [[chatgpt]], [[gpt-4]], [[pre-trained-language-models]], [[deep-learning]], [[prompt-engineering]], [[llms-in-ma]], [[index]]
- Contradictions flagged: none
- Note: arXiv preprint (arXiv:2303.18223v13, not peer-reviewed in a journal). ~15,000+ citations; treated as the de facto foundational LLM reference. Anchors Section 2.2 ("KI-Verfahren: Einordnung und Relevanz für M&A") of the Thema 7 seminar paper by supplying the canonical four-generation LM taxonomy and definitions of emergent abilities, scaling laws, and the pre-training + adaptation tuning + prompting paradigm. The taxonomy directly explains why GPT-4-class models (used in Degen et al. 2024, Jang & Stikkel 2024, Bozman et al. 2026) can perform M&A tasks that earlier models could not: only the LLM generation (Generation 4) exhibits emergent abilities (ICL, instruction following) enabling few-shot document classification and zero-shot sentiment scoring.

## [2026-05-05 16:33] ingest | M&A Grundlagenteil sources: information asymmetry, performance, PMI, and culture
- Sources: [[2026-05-05-akerlof-1970-market-for-lemons]], [[2026-05-05-myers-majluf-1984-corporate-financing-investment-decisions]], [[2026-05-05-king-et-al-2004-post-acquisition-performance-meta-analysis]], [[2026-05-05-haleblian-et-al-2009-ma-review]], [[2026-05-05-graebner-et-al-2017-post-merger-integration-review]], [[2026-05-05-li-et-al-2021-corporate-culture-ml]]
- New: [[george-akerlof]], [[stewart-myers]], [[nicholas-majluf]], [[david-r-king]], [[jerayr-haleblian]], [[melissa-graebner]], [[kai-li]], [[quarterly-journal-of-economics]], [[journal-of-financial-economics]], [[strategic-management-journal]], [[journal-of-management]], [[academy-of-management-annals]], [[review-of-financial-studies]], [[sdc-securities-data-company]], [[sp-global]], [[market-for-lemons]], [[pecking-order-theory]], [[acquisition-performance]], [[corporate-culture]], [[machine-learning]]
- Updated: [[information-asymmetry]], [[mergers-and-acquisitions]], [[post-merger-integration]], [[ma-success-measurement]], [[index]]
- Contradictions flagged: none
- Note: All six PDFs were judged relevant and moved from `research/input/inbox/` to `research/input/papers/` with normalized filenames. Akerlof (1970) and Myers & Majluf (1984) strengthen the information-asymmetry foundation; Haleblian et al. (2009), King et al. (2004), and Graebner et al. (2017) strengthen the M&A-process and performance foundation; Li et al. (2021) is relevant as a supporting source for ML-based corporate-culture measurement, but should remain secondary to the M&A-specific Brede et al. (2025) evidence.

## [2026-05-06 13:57] ingest | M&A uncertainty foundation sources
- Sources: [[2026-05-06-bhagwat-dam-harford-2016-uncertainty-merger-activity]], [[2026-05-06-bonaime-gulen-ion-2018-policy-uncertainty-ma]]
- New: [[uncertainty-in-ma]], [[vineet-bhagwat]], [[robert-dam]], [[jarrad-harford]], [[alice-bonaime]], [[huseyin-gulen]], [[mihai-ion]]
- Updated: [[mergers-and-acquisitions]], [[merger-waves]], [[ma-success-measurement]], [[acquisition-performance]], [[journal-of-financial-economics]], [[review-of-financial-studies]], [[index]]
- Contradictions flagged: none
- Note: Both PDFs were judged important and moved from `research/input/inbox/` to `research/input/papers/` with normalized filenames. Bhagwat, Dam & Harford (2016) provides the core interim-risk mechanism; Bonaime, Gulen & Ion (2018) provides the policy-uncertainty / real-options mechanism and deal-term implications. Together they strengthen the proposed "AI and uncertainty in M&A decision-making" research direction as a general M&A foundation before adding AI-specific sources.

## [2026-05-06 14:45] ingest | AI limits in M&A legal review and post-merger integration planning
- Sources: [[2026-05-06-wang-et-al-2023-maud-merger-agreement-understanding]], [[2026-05-06-malmqvist-2025-ai-assisted-pmi-planning]]
- New: [[maud-dataset]], [[the-atticus-project]], [[steven-wang]], [[lars-malmqvist]], [[the-tech-collective]], [[merger-agreement-understanding]], [[ai-assisted-pmi-planning]], [[dependency-analysis]]
- Updated: [[due-diligence]], [[post-merger-integration]], [[llms-in-ma]], [[ai-in-ma]], [[kira-dataset]], [[index]]
- Contradictions flagged: none
- Note: Both PDFs were judged relevant and moved from `research/input/inbox/` to `research/input/papers/` with normalized filenames. Wang et al. (2023, EMNLP) is a strong peer-reviewed benchmark source for measurable AI performance and errors in merger agreement understanding. Malmqvist (2025, arXiv preprint) is directly relevant to AI-assisted PMI planning and the human-judgment angle, but should be framed as exploratory evidence because of the tiny student sample and simulated setting.

## [2026-05-07 12:00] ingest | Artificial Intelligence, Machine Learning, and Bias in Finance: Toward Responsible Innovation
- Source: [[2026-05-07-johnson-pasquale-chapman-2019-ai-ml-bias-finance]]
- New: [[kristin-johnson]], [[frank-pasquale]], [[jennifer-chapman]], [[fordham-law-review]], [[office-of-the-comptroller-of-the-currency]], [[consumer-financial-protection-bureau]], [[new-york-dfs]], [[algorithmic-bias]], [[automated-decision-making]], [[disparate-impact]], [[fintech-regulation]]
- Updated: [[black-box-problem]], [[ai-governance-in-ma]], [[responsible-ai]], [[xai-explainable-ai]], [[index]]
- Contradictions flagged: none

## [2026-05-07 10:00] ingest | Artificial Intelligence on Merger and Acquisition Processes: Observation from The Target Identification and Due Diligence Perspective

- Source: [[2026-05-07-rashid-et-al-2025-ai-ma-target-identification-due-diligence]]
- New: [[mohammad-mamunur-rashid]], [[nazim-ullah]], [[international-islamic-university-chittagong]], [[ijirme]], [[cyndx]], [[predictive-analytics-in-ma]]
- Updated: [[due-diligence]], [[ml-target-selection]], [[ai-in-ma]], [[machine-learning]], [[index]]
- Contradictions flagged: none
- Note: IJIRME is a lower-tier journal. The paper is a conceptual literature review (secondary data only) with no original empirical analysis. The practitioner-reported efficiency figures (6 weeks → 8 days, −42% cost, 40× more targets) are cited without traceable primary provenance; they should be treated as illustrative benchmarks, not peer-reviewed findings. Use as a supporting reference for the broad AI-in-M&A framing; prefer Bozman et al. (2026), Jang & Stikkel (2024), or Zhang et al. (2024) for quantitative claims. Source is relevant for Abschnitt 3.1 (target identification) and 3.2 (due diligence) of the Thema 7 seminar paper, particularly for narratively connecting the two phases and for the efficiency-gain framing.

## [2026-05-07 12:21] ingest | Howson full scan — Due Diligence: The Critical Stage in Mergers and Acquisitions
- Source: [[2026-05-07-howson-2003-due-diligence-critical-stage]]
- New: none
- Updated: [[2026-05-07-howson-2003-due-diligence-critical-stage]], [[classical-due-diligence-process]], [[due-diligence]], [[index]]
- Contradictions flagged: none
- Note: Moved the full scanned PDF from `research/input/inbox/` to `research/input/papers/howson-2003-due-diligence-critical-stage-full.pdf`. The PDF has 296 page-image pages and no embedded text; local OCR was not available, so this is a selective visual re-ingest rather than full text mining. Update aligns Howson with the new DD-focused research question from Notion and adds adviser-governance/process-quality points for the classical-vs-AI DD comparison.

## [2026-05-07 14:00] ingest | Due Diligence: The Critical Stage in Mergers and Acquisitions (Howson 2003)

- Source: [[2026-05-07-howson-2003-due-diligence-critical-stage]]
- New: [[peter-howson]], [[amr-international]], [[gower-publishing]], [[routledge]], [[kpmg]], [[classical-due-diligence-process]]
- Updated: [[due-diligence]], [[index]]
- Contradictions flagged: none
- Note: Only a cover preview PDF is in research/input/ (cover, ToC, Ch. 1 introduction, preface, list of tables/figures). Full text of Chapters 2–16 not available. Source page is explicitly marked as preview-only; claims inferred from the ToC are flagged with (inferred from ToC/cover). The Howson five-strand DD model and 16-discipline taxonomy are established as the "classical DD process" baseline for the Thema 7 seminar paper, against which AI-assisted DD is compared. The KPMG 1999 acquisition success study (83% correlation; synergy evaluation +28%) is noted as a secondary citation requiring verification if the original becomes available.

## [2026-05-07 15:30] ingest | Information Asymmetry in Management Research: Past Accomplishments and Future Opportunities
- Source: [[2026-05-07-bergh-et-al-2019-information-asymmetry-management-research]]
- New: [[donald-bergh]], [[david-ketchen]], [[ilaria-orlandi]], [[pursey-heugens]], [[brian-boyd]], [[agency-theory]], [[signaling-theory]], [[transaction-cost-economics]], [[adverse-selection]], [[moral-hazard]], [[information-impactedness]]
- Updated: [[information-asymmetry]], [[due-diligence]], [[journal-of-management]], [[index]]
- Contradictions flagged: none
- Note: Bergh et al. (2019, Journal of Management, Vol. 45, No. 1, pp. 122–158) is the most comprehensive management-research review of information asymmetry and should serve as the primary theoretical framework source for the Grundlagenteil of the Thema 7 seminar paper. The paper provides (a) a canonical five-conceptualization taxonomy (private information, different information, hidden information, lack of perfect information, impactedness), (b) a three-antecedent model (unobservable qualities, structural barriers, strategic/behavioral barriers), (c) a four-theoretical-role framework (assumption, mechanism, construct, boundary condition), and (d) eight resolution/exploitation strategies. The information-asymmetry concept page has been substantially enriched with these conceptual layers. Six new concept stub pages created (agency-theory, signaling-theory, transaction-cost-economics, adverse-selection, moral-hazard, information-impactedness) to anchor the theoretical vocabulary for future sources. The due-diligence concept page gains a theoretically grounded claim connecting DD to the Bergh et al. resolution taxonomy (gathering/disclosure + monitoring + intermediaries = most composite resolution). No conflicts with existing wiki content — this source deepens and formalizes what prior sources treated as given.

## [2026-05-07 17:00] ingest | Artificial Intelligence applications in due diligence processes for large-scale merger and acquisition transaction evaluation

- Source: [[2026-05-07-ugoji-et-al-2025-ai-due-diligence-ma-transaction-evaluation]]
- New: [[angela-ugoji]], [[iyedolapo-ajewole]], [[olaadura-peters]], [[culbert-kalle]], [[case-western-reserve-university]], [[wjarr]], [[thomson-reuters-sdc-platinum]], [[adaboost]], [[support-vector-machine]], [[ai-due-diligence-platforms]], [[cross-border-ma]]
- Updated: [[due-diligence]], [[machine-learning]], [[ai-in-ma]], [[esg-in-ma]], [[information-asymmetry]], [[index]]
- Contradictions flagged: none

## [2026-05-07 18:00] ingest | The Art of M&A: A Merger, Acquisition, and Buyout Guide (Fifth Edition) — Lajoux 2019
- Source: [[2026-05-07-lajoux-2019-art-of-ma-fifth-edition]]
- New: [[alexandra-reed-lajoux]], [[capital-expert-services]], [[mcgraw-hill]], [[jim-jeffries]], [[ma-leadership-council]]
- Updated: [[mergers-and-acquisitions]], [[due-diligence]], [[index]]
- Contradictions flagged: none
- Note: Only cover, half-title, and blank page are available in the PDF preview. Source page is an explicit stub; all substantive claims derive from prior knowledge / publisher description and are marked as such. No direct quotations should be used in the seminar paper without access to the full text. Lajoux (2019) is registered as the secondary reference for Kap. 2.1 (broader M&A lifecycle context); Howson (2003) remains the primary classical DD reference. The book's scope (full lifecycle, Q&A format) and the Howson book's scope (DD only, practitioner manual) are complementary and non-conflicting.

## [2026-05-07 13:49] ingest | Due diligence quality, legal AI benchmarks, ICL, and human-in-the-loop risks
- Sources: [[2026-05-07-bhagwan-et-al-2018-systematic-review-dd-ma]], [[2026-05-07-puranam-et-al-2006-dd-signal-detection]], [[2026-05-07-hendrycks-et-al-2021-cuad-contract-review]], [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]], [[2026-05-07-sele-chugunova-2024-human-in-loop-adm]]
- New: [[v-bhagwan]], [[sara-grobbelaar]], [[william-bam]], [[south-african-journal-of-industrial-engineering]], [[stellenbosch-university]], [[phanish-puranam]], [[benjamin-powell]], [[harbir-singh]], [[strategic-organization]], [[london-business-school]], [[university-of-pennsylvania]], [[dan-hendrycks]], [[collin-burns]], [[anya-chen]], [[spencer-ball]], [[uc-berkeley]], [[contract-understanding-atticus-dataset]], [[madhukar-dwivedi]], [[jaap-kamps]], [[university-of-amsterdam]], [[information-retrieval-research]], [[daniela-sele]], [[marina-chugunova]], [[plos-one]], [[eth-zurich]], [[max-planck-institute-for-innovation-and-competition]], [[due-diligence-quality]], [[due-diligence-signal-detection]], [[legal-contract-review]], [[in-context-learning-for-due-diligence]], [[human-in-the-loop]], [[automation-bias]]
- Updated: [[due-diligence]], [[classical-due-diligence-process]], [[kira-dataset]], [[the-atticus-project]], [[hierarchical-sentence-extraction]], [[algorithmic-bias]], [[ai-governance-in-ma]], [[index]]
- Contradictions flagged: none
- Note: Five inbox PDFs were content-checked for relevance to the unchanged research question ("Inwiefern verbessert KI Qualität und Geschwindigkeit der Due Diligence, und welche Risiken entstehen durch algorithmische Verzerrung?") and moved into `research/input/papers/` with normalized filenames. Bhagwan et al. (2018) and Puranam et al. (2006) strengthen the classical/process-quality foundation; Hendrycks et al. (2021) and Dwivedi & Kamps (2025) strengthen the measurable legal-DD automation evidence; Sele & Chugunova (2024) strengthens the risk section by showing that human-in-the-loop designs can increase algorithm uptake without guaranteeing better accuracy. The Dwivedi & Kamps PDF is image/rendered; key metadata and claims were verified by visual page inspection rather than full embedded-text extraction.

## [2026-05-07 19:30] ingest | The Art of M&A (6th ed., 2024) — Lajoux, Chapters 1 and 6

- Source: [[2026-05-07-lajoux-2024-art-of-ma-sixth-edition-ch1-ch6]]
- New: (none — all entities and concepts already existed)
- Updated: [[alexandra-reed-lajoux]], [[classical-due-diligence-process]], [[due-diligence]], [[mergers-and-acquisitions]], [[index]]
- Contradictions flagged: none
- Note: Sixth and final edition supersedes the 2019 fifth-edition preview ([[2026-05-07-lajoux-2019-art-of-ma-fifth-edition]]) as the primary Lajoux wiki reference. The 2019 stub page is retained but marked as superseded. Chapter 1 provides the canonical eight-phase circular M&A lifecycle (Strategy → Valuation → Financing → Structuring → Due Diligence → Negotiation → Closing → Integration), now the authoritative process diagram for Kap. 2.1 of the seminar paper. Chapter 6 is the most detailed practitioner source for classical DD currently in the wiki: it adds legal anchoring (Securities Act 1933 due diligence defense, Exchange Act Rule 10(b)5), VDR infrastructure detail, cybersecurity DD (cloud, GDPR, shadow IT), cultural DD linked to PMI planning, a four-category red-flag taxonomy, the 2023 US safe-harbor for DD-discovered legal violations, and the bring-down condition extending DD through closing — none of which are covered in Howson (2003). The alexandra-reed-lajoux entity page is updated to reflect six editions (1989–2024) and the author's emerita status on the Board of M&A Standards. No conflicts with existing wiki content; Lajoux (2024) Ch.6 and Howson (2003) are complementary on the classical DD baseline (legal anchoring vs. project-management framework).

## [2026-05-07 18:00] ingest | Effectiveness of In-Context Learning for Due Diligence (Dwivedi & Kamps 2025, IRRJ)

- Source: [[2026-05-07-dwivedi-kamps-2025-icl-due-diligence]]
- New: [[entities/adam-roegiest]], [[entities/gpt-4o-mini]], [[entities/deepseek-r1]], [[entities/llama3-1]], [[entities/gemma2]], [[entities/dolphin-llama3]], [[entities/ollama]], [[concepts/conditional-random-fields]], [[concepts/high-recall-information-retrieval]], [[concepts/few-shot-learning]], [[concepts/zero-shot-learning]]
- Updated: [[entities/kira-dataset]], [[entities/madhukar-dwivedi]], [[entities/jaap-kamps]], [[concepts/in-context-learning-for-due-diligence]], [[concepts/due-diligence]], [[concepts/legal-contract-review]], [[concepts/prompt-engineering]], [[index]]
- Contradictions flagged: none
- Note: Source page was a stub from a prior partial ingest; fully rewritten with quantitative results from all tables. The existing source-page slug is unchanged. Open question on kira-dataset ("has any group covered all 50 topics?") is now resolved by this paper.

## [2026-05-07 19:00] ingest | Due Diligence: The Critical Stage in Mergers and Acquisitions (Howson 2003)

- Source: [[2026-05-07-howson-2003-due-diligence-critical-stage]]
- New: [[vendor-due-diligence]], [[cadbury-report]]
- Updated: [[2026-05-07-howson-2003-due-diligence-critical-stage]], [[classical-due-diligence-process]], [[due-diligence-quality]], [[index]]
- Contradictions flagged: none
- Note: Source page previously existed as a stub built from preview material; fully upgraded with OCR-extracted key facts covering all 16 chapters, the two DD-area tables (15 areas total), the five-strand programme model, Bowyer's five M&A types, VDD credibility risk, and the Cadbury Report governance anchor. Precision correction added to classical-due-diligence-process: "16 Disziplinen" is a simplification — the book has 16 chapters but only 13 are discipline-specific; the two tables list 15 DD areas. New concept page created for vendor-due-diligence (VDD); new entity stub created for cadbury-report.

## [2026-05-07 18:36] cleanup | Remove out-of-scope and low-confidence wiki pages

- Removed source pages: `Bhagwat/Dam/Harford 2016 uncertainty`, `Bonaime/Gulen/Ion 2018 policy uncertainty`, `Malmqvist 2025 PMI planning`, `Lajoux 2019 preview stub`, `Rashid et al. 2025`, `Ugoji et al. 2025`.
- Removed only dependent concept/entity pages that were created solely from those pages or from the superseded preview.
- Updated: [[index]], [[due-diligence]], [[ai-in-ma]], [[machine-learning]], [[esg-in-ma]], and related entity pages.
- Rationale: Conservative cleanup for the current DD-focused research question; retained all pages with plausible relevance to M&A, due diligence, AI, bias, XAI, governance, citation/formalia, or the prescribed seminar readings.
- Verification: no broken wiki links outside this append-only log after cleanup.
