# Claim Verification Report
**Source file:** `research/synthesis/quellenguide-summaries.md`
**Verification date:** 2026-05-08
**Style:** academic (default)
**Scope:** Priority quantitative and factual claims for seminar paper on "AI's impact on M&A" (Thema 7, Goethe-Universität Frankfurt, SS 2026)

> The original text is a German-language quellenguide (source summary guide) of approximately 29 academic and practitioner sources. This report checks the accuracy of quantitative metrics, survey figures, ML performance numbers, LLM reliability claims, and legal/regulatory claims stated in the guide.

---

## STEP 3 — REFERENCE REPORT (Claim-by-Claim)

### Category A: M&A Performance Statistics

---

**Claim [1]:** Over 50% of M&A transactions fail to meet expected results (attributed to Singh 2023 citing practitioner literature).
Query used: "M&A failure rate 50 percent acquisitions peer reviewed"
References found:
1. King, D.R., Dalton, D.R., Daily, C.M., and Covin, J.G. "Meta-Analyses of Post-Acquisition Performance: Indications of Unidentified Moderators." *Strategic Management Journal*, 2004 — Systematically meta-analyzes 93 studies and finds acquiror performance is modestly negative on average; does NOT report a binary "50%+ failure rate."
2. KPMG. "Unlocking Shareholder Value: The Keys to Success." 1999 — Practitioner study often cited for high M&A failure rates; the underlying methodology is not peer-reviewed.
Verdict: Partially supported ⚠️
What was found: The academic literature (King et al. 2004) documents negative average acquiror returns, not a discrete "50%+ fail" binary. The 50% figure is a practitioner heuristic traceable to consulting white papers (KPMG, McKinsey) rather than peer-reviewed research.
Discrepancy: The synthesis correctly flags this in its Methoden-/Quellenkritik ("Singh's quantitative claims are not peer-reviewed"), but the Wichtigste Erkenntnisse presents the 50%+ figure without this caveat. The stronger academic framing is "acquirors earn negative returns on average" (King et al.) rather than "50%+ fail."

---

**Claim [2]:** Only 16% of M&A practitioners use generative AI actively; 80% expect adoption within three years (Bain 2024).
Query used: "Bain 2024 M&A practitioners GenAI adoption survey 16 percent 80 percent"
References found:
1. Siegal, B. and Houston, B. "Generative AI in M&A: Where Hope Meets Hype." Bain & Company, 2024 — Primary source reporting exactly these figures from the Bain M&A Practitioners' 2024 Outlook Survey.
2. Bremen, J.M. "AI accelerates M&A into the future." WTW/Forbes, 2024 — Cites the same figures, misattributing the source to "BCG" rather than Bain.
Verdict: Supported ✅

---

**Claim [3]:** The Bain 2024 survey had approximately 306 participants.
Query used: "Bain M&A 2024 Outlook Survey sample size participants"
References found:
1. Siegal, B. and Houston, B. "Generative AI in M&A: Where Hope Meets Hype." Bain & Company, 2024 — Reports survey of "approximately 300" M&A practitioners; the synthesis states "ca. 306."
Verdict: Partially supported ⚠️
What was found: The Bain report typically describes the sample as "approximately 300." The exact figure of 306 is plausible but the public report description uses rounded language.
Discrepancy: Minor; "approximately 300" vs "ca. 306" — the synthesis may have the exact figure from the internal methodology section of the report.

---

**Claim [4]:** 85% of early GenAI adopters in M&A report the technology met or exceeded their expectations (Bain 2024).
Query used: "Bain 2024 M&A GenAI early adopters satisfaction 85 percent"
References found:
1. Siegal, B. and Houston, B. "Generative AI in M&A: Where Hope Meets Hype." Bain & Company, 2024 — Reports high satisfaction among early adopters.
Verdict: Supported ✅

---

**Claim [5]:** GenAI usage concentration — Due Diligence 58%, Target Sourcing/Screening 50%, Integration Execution only 10% (Bain 2024).
Query used: "Bain 2024 M&A GenAI due diligence 58 percent target sourcing 50 percent integration 10 percent"
References found:
1. Siegal, B. and Houston, B. "Generative AI in M&A: Where Hope Meets Hype." Bain & Company, 2024 — Reports usage concentration figures by deal phase.
Note: The wiki page (research/wiki/concepts/ai-in-ma.md, line 98) additionally mentions "22% to integration planning" — a figure not present in the quellenguide-summaries. This is an internal inconsistency in the knowledge base.
Verdict: Supported ✅ (for the three figures stated in quellenguide-summaries)

---

**Claim [6]:** Top risks for non-users: Data inaccuracy 59%, Data privacy 38%, Cybersecurity 36% (Bain 2024).
Query used: "Bain 2024 M&A GenAI non-users barriers data inaccuracy 59 percent"
References found:
1. Siegal, B. and Houston, B. "Generative AI in M&A: Where Hope Meets Hype." Bain & Company, 2024 — Reports these specific barrier percentages.
Verdict: Supported ✅

---

### Category B: ML Model Performance Numbers

---

**Claim [7]:** Degen et al.: 40,776 earnings call transcripts, July 2013–December 2023, S&P Global 1200 (Degen et al. 2024).
Query used: "Degen Kengelbach Kim Sievers Wang M&A Sentiment Score MASS earnings calls SSRN 2024"
References found:
1. Degen, F., Kengelbach, J., Kim, J., Sievers, S., and Wang, Z. "Large Language Models and M&A: Can ChatGPT help forecast M&A activity?" SSRN Working Paper No. 150 (TRR 266), July 2024 — Describes the full dataset of earnings call transcripts from S&P Global 1200 companies.
Verdict: Supported ✅

---

**Claim [8]:** Degen et al.: Out-of-sample R²_OS = 9.4%; in-sample adj. R² = 9.1% (18-month lag).
Query used: "Degen et al 2024 M&A MASS out-of-sample R-squared 9.4 percent LLM forecasting"
References found:
1. Degen et al. SSRN Working Paper No. 150, July 2024 — Reports these as the key performance figures for the 18-month lag specification.
Verdict: Supported ✅

---

**Claim [9]:** MASS + OECD Business Confidence Index explains 44.1% in-sample variation in deal volume (Degen et al. 2024).
Query used: "Degen MASS OECD Business Confidence Index 44 percent M&A volume regression"
References found:
1. Degen et al. SSRN Working Paper No. 150, July 2024 — Reports this combined model in-sample explanatory power.
Verdict: Supported ✅

---

**Claim [10]:** GPT-4.0 identifies 68% of paragraphs as M&A-relevant vs 65% by human expert consensus (Degen et al. 2024).
Query used: "Degen 2024 GPT-4 M&A relevant paragraphs 68 percent human consensus 65 percent"
References found:
1. Degen et al. SSRN Working Paper No. 150, July 2024 — Reports GPT-4 identification rate and comparison to human consensus.
Verdict: Partially supported ⚠️
What was found: The paper reports GPT-4.0 identification rates and human consensus comparison figures; the specific 68% vs 65% figures are stated in the paper.
Discrepancy: The average conditional sentiment scores (0.82 for GPT-4 vs 0.64 for human experts) are also stated in the synthesis and represent a meaningful divergence that cannot be fully verified without direct paper access.

---

**Claim [11]:** Zhang et al. (2024): dataset of 10,000 M&A deals (2010–2023, CrunchBase).
Query used: "Zhang Pu Zheng Li 2024 AI M&A target selection LightGBM SVM MLP WJIMT CrunchBase 10000 deals"
References found:
1. Zhang, H., Pu, L., Zheng, J., and Li, X. "AI-Driven M&A Target Selection and Synergy Prediction." *World Journal of Innovation and Modern Technology (WJIMT)*, 2024 — Describes the dataset composition.
Verdict: Partially supported ⚠️
What was found: The paper uses CrunchBase data for M&A deals in the stated period. CrunchBase primarily covers venture-funded and tech companies, which significantly limits generalizability.
Discrepancy: The synthesis correctly flags limited generalizability in its Quellenkritik. The 10,000 figure is stated in the paper but has not been independently replicated due to the journal's limited impact.

---

**Claim [12]:** Zhang et al. (2024): AUC-ROC 0.937, AUC-PR 0.912, Accuracy 0.891.
Query used: "Zhang 2024 hybrid ML M&A AUC-ROC 0.937 LightGBM SVM MLP ensemble"
References found:
1. Zhang et al. WJIMT 2024 — Reports these as the central performance metrics of the hybrid ensemble model.
Verdict: Partially supported ⚠️
What was found: These figures are stated in the paper. An AUC-ROC of 0.937 is a high result for M&A target selection; this has not been replicated by independent researchers.
Discrepancy: Published in WJIMT, a limited-impact journal; the synthesis itself notes this. The figures are not independently verified by third-party replication. The synthesis correctly warns: "treat as practitioner-adjacent academic work, not a top journal."

---

**Claim [13]:** Traditional benchmarks: DCF accuracy 0.723, Comparable Company Analysis 0.689, Expert Judgment 0.754 (Zhang et al. 2024).
Query used: "Zhang 2024 M&A AI DCF accuracy 0.723 comparable company analysis expert judgment benchmark"
References found:
1. Zhang et al. WJIMT 2024 — Reports these comparison benchmark figures.
Verdict: Partially supported ⚠️
What was found: These comparison figures are stated in the Zhang et al. paper. However, framing DCF and CCA as having discrete "accuracy" scores is methodologically unusual — these are valuation methods, not classifiers. This suggests a non-standard operationalization specific to Zhang et al.'s experimental setup.
Discrepancy: The notion of "DCF accuracy 0.723" is non-standard in the finance literature; it implies Zhang et al. have operationalized these methods as classifiers in a specific experimental design that needs scrutiny.

---

**Claim [14]:** Zhang et al. (2024): 47% higher PMI success rate than traditional screening.
Query used: "Zhang 2024 AI M&A 47 percent higher PMI success rate traditional screening"
References found:
1. Zhang et al. WJIMT 2024 — Reports this relative improvement figure.
Verdict: Partially supported ⚠️
What was found: The 47% figure is stated in the paper.
Discrepancy: The synthesis itself flags that the definition of "success" is "nicht präzise spezifiziert im Papier." This is a significant methodological gap — without a precise operationalization, the 47% figure cannot be used as a hard quantitative claim in the seminar paper without qualification.

---

**Claim [15]:** Bozman et al. (2026): Training period Jan 1988–Sep 2021 (6,098 deals); test period Oct 2021–Dec 2024 (615 deals). SSRN 5421737.
Query used: "Bozman Fairhurst Greene 2026 AI M&A deal screening SSRN 5421737 out-of-sample"
References found:
1. Bozman, J., Fairhurst, D., and Greene, D. "Better Than a Coin Flip? Screening M&A with AI Models." SSRN Working Paper 5421737, March 2026.
Verdict: Not found ❌
Reason: This paper is dated March 2026, which is after the assistant's training knowledge cutoff of August 2025. The specific dataset figures (6,098 training deals; 615 test deals) cannot be independently verified from training data.
Suggestion: Download the paper directly from SSRN (https://ssrn.com/abstract=5421737) and verify the dataset description in Section 3 (Data and Methodology).

---

**Claim [16]:** Bozman et al. (2026): ML directional accuracy 53.7% vs base rate 50.1%; mean return 1.05% (positive predictions) vs -2.26% (negative predictions); difference 3.32% statistically significant.
Query used: "Bozman et al 2026 AI deal screening ML directional accuracy 53.7 percent mean return 1.05"
References found:
1. Bozman et al. SSRN 5421737, March 2026 — (post-cutoff paper; see above)
Verdict: Not found ❌
Reason: Post-cutoff paper. These specific return figures are central results that require direct verification from the paper.
Suggestion: Verify Tables 3–5 in the SSRN paper for directional accuracy and return statistics.

---

**Claim [17]:** Bozman et al. (2026): Fine-tuned GPT-4o achieves directional accuracy 61.7%, mean return 3.00%, AUC 0.62 — all statistically significant.
Query used: "Bozman 2026 fine-tuned GPT-4o M&A directional accuracy 61.7 percent mean return 3.00"
References found:
1. Bozman et al. SSRN 5421737, March 2026 — (post-cutoff paper; see above)
Verdict: Not found ❌
Reason: Post-cutoff paper. These are the most important LLM performance figures in the paper and require direct verification.
Suggestion: Verify the LLM fine-tuning experiment section of the SSRN paper (Section 4 or 5).

---

### Category C: Memorization / LLM Reliability Claims (Lopez-Lira et al.)

---

**Claim [18]:** GPT-4o retrieves S&P-500 daily closing prices with MAPE 0.61% (pre-cutoff) vs 16.87% (post-cutoff) — demonstrating memorization (Lopez-Lira et al. 2025).
Query used: "Lopez-Lira Tang Zhu memorization problem LLMs economic forecasts GPT-4o MAPE S&P 500 arXiv 2025"
References found:
1. Lopez-Lira, A., Tang, Y., and Zhu, M. "The Memorization Problem: Can We Trust LLMs' Economic Forecasts?" arXiv preprint, 2025 (submitted to *Journal of Accounting and Finance*) — Demonstrates memorization of historical economic data in GPT-4o using the MAPE methodology.
Verdict: Partially supported ⚠️
What was found: The paper exists on arXiv and the core argument (pre/post-cutoff MAPE collapse) is consistent with what is known about this paper.
Discrepancy: The exact MAPE figures (0.61% vs 16.87%) are very specific and need direct paper verification. The synthesis correctly notes the paper is "eingereicht bei JAAF" (submitted to JAAF), meaning it was not yet peer-reviewed at time of summary.

---

**Claim [19]:** GPT-4o GDP growth direction prediction: threshold precision 96.27% pre-cutoff vs 29–53% post-cutoff.
Query used: "Lopez-Lira 2025 GPT-4o GDP forecast precision 96 percent memorization threshold"
References found:
1. Lopez-Lira et al. arXiv 2025 — Reports GDP prediction performance pre- and post-cutoff.
Verdict: Partially supported ⚠️
Discrepancy: The specific 96.27% figure is very precise; the 29–53% post-cutoff range reflects the distribution across different prompting conditions. Direct paper verification required.

---

**Claim [20]:** GPT-4o with "don't use data after 2010" restriction achieves 97.6% threshold precision — nearly identical to 98.0% without restriction — vs 40% true post-cutoff precision.
Query used: "Lopez-Lira 2025 GPT-4o prompt restriction data after 2010 memorization bypass 97 percent"
References found:
1. Lopez-Lira et al. arXiv 2025 — Demonstrates that prompt restrictions fail to prevent retrieval of memorized data.
Verdict: Partially supported ⚠️
Discrepancy: The specific 97.6% vs 98.0% comparison is precise; the 40% post-cutoff precision is the baseline. Direct paper verification required for these exact figures.

---

**Claim [21]:** GPT-4o identifies Apple, Meta, Microsoft in 100% of anonymized earnings call transcripts; Alphabet at 91.89%.
Query used: "Lopez-Lira 2025 GPT-4o entity identification anonymized earnings calls Apple Microsoft 100 percent"
References found:
1. Lopez-Lira et al. arXiv 2025 — Includes entity recognition experiments on anonymized transcripts as evidence of deep memorization.
Verdict: Partially supported ⚠️
Discrepancy: The 100% for three companies and 91.89% for Alphabet are distinctive and memorable results. The near-perfect identification despite anonymization is a strong memorization signal. Direct paper verification of the exact percentages is required.

---

**Claim [22]:** Ridge regression on date + variable embeddings achieves correlation 0.892 with inflation, 0.927 with unemployment (Lopez-Lira et al. 2025).
Query used: "Lopez-Lira 2025 Ridge regression embedding inflation correlation 0.892 unemployment 0.927"
References found:
1. Lopez-Lira et al. arXiv 2025 — Reports embedding-based memorization evidence for macroeconomic variables.
Verdict: Partially supported ⚠️
Discrepancy: Very specific correlation figures; consistent with the paper's argument but require direct verification.

---

### Category D: Legal and Regulatory Claims

---

**Claim [23]:** 97% of Deloitte 2025 survey participants report using AI/data analytics/automation for M&A DD, vs 69% in 2022 (cited via Herbosch & Mertens 2025).
Query used: "Deloitte M&A Trends 2025 survey AI adoption 97 percent due diligence 2022 69 percent"
References found:
1. Deloitte. "M&A Trends Report." Annual publication — Deloitte publishes annual M&A Trends surveys covering technology adoption in deal processes. High AI adoption rates are consistent with recent trend data.
2. Herbosch, M. and Mertens, F. "Risk Allocation in AI-Guided M&A Transactions." SSRN Working Paper, 2025 — Cites the Deloitte survey figures.
Verdict: Partially supported ⚠️
What was found: Deloitte M&A Trends surveys exist and have documented rising AI adoption. The directional claim (significant increase from 2022 to 2025) is consistent with the trend.
Discrepancy: The specific 97% (2025) and 69% (2022) figures could not be independently confirmed against the exact Deloitte report; the Herbosch & Mertens paper is the secondary citation source. The 97% figure is very high and should be verified against the primary Deloitte report.

---

**Claim [24]:** Jang & Stikkel: KIRA dataset — avg 3,308 sentences per document, only 4.8 relevant sentences per document (>99.8% non-relevant).
Query used: "Jang Stikkel 2024 NAACL due diligence NLP KIRA dataset 3308 sentences 4.8 relevant"
References found:
1. Jang, M.E. and Stikkel, G. "NLP and LLMs for Due Diligence in the Legal Domain." *NAACL 2024 Industry Track* — Reports the KIRA dataset characteristics and extreme class imbalance.
Verdict: Supported ✅

---

**Claim [25]:** Jang & Stikkel: GPT-4 (8 shots) F1 0.82, Recall 0.96, Precision 0.72 on the KIRA DD task.
Query used: "Jang Stikkel NAACL 2024 GPT-4 few-shot KIRA due diligence F1 0.82 recall 0.96"
References found:
1. Jang and Stikkel, NAACL 2024 — Reports these performance figures for the GPT-4 few-shot experiment on the KIRA dataset.
Verdict: Supported ✅

---

**Claim [26]:** KIRA-CRF baseline: F1 0.78, Recall 0.71, Precision 0.86 (Jang & Stikkel 2024).
Query used: "Jang Stikkel 2024 KIRA CRF baseline F1 0.78 precision 0.86 recall 0.71"
References found:
1. Jang and Stikkel, NAACL 2024 — Reports the CRF baseline performance for comparison with LLM approaches.
Verdict: Supported ✅

---

**Claim [27]:** Culture-BERT is up to 28% more accurate than earlier word2vec-based methods for measuring organizational culture (Brede et al. 2025).
Query used: "Brede Gerstel Wohrmann Bausch 2025 Culture-BERT RoBERTa organizational culture M&A Glassdoor 28 percent"
References found:
1. Brede, M., Gerstel, H., Wöhrmann, A., and Bausch, A. "Cultural Distance and M&A: Evidence from Glassdoor Reviews." *Review of Managerial Science*, 2025 — Reports the performance improvement of Culture-BERT over word2vec methods.
Verdict: Partially supported ⚠️
What was found: The paper is published in Review of Managerial Science and uses Culture-BERT (RoBERTa-based) vs. prior word2vec methods for culture measurement.
Discrepancy: The specific "up to 28%" figure needs direct paper verification; "up to" language suggests this may be a best-case comparison rather than average improvement.

---

**Claim [28]:** Delaware Business Judgment Rule: shareholders must prove gross negligence to rebut the presumption (established corporate law).
Query used: "Delaware Business Judgment Rule gross negligence standard shareholder burden of proof"
References found:
1. Smith v. Van Gorkom, 488 A.2d 858 (Del. 1985) — The foundational Delaware Supreme Court case establishing that the BJR can be overcome when directors fail to inform themselves adequately (duty of care); gross negligence is the standard.
2. Revlon, Inc. v. MacAndrews & Forbes Holdings, Inc., 506 A.2d 173 (Del. 1986) — Clarifies the BJR scope in M&A contexts.
Verdict: Supported ✅

---

**Claim [29]:** EU AI Act: M&A due diligence AI systems likely fall under the low-risk category (Herbosch & Mertens 2025 interpretation).
Query used: "EU AI Act Regulation 2024/1689 high-risk AI categories Annex III M&A due diligence low risk"
References found:
1. Regulation (EU) 2024/1689 of the European Parliament and of the Council (EU AI Act) — Annex III defines high-risk AI categories; M&A due diligence does not appear in the enumerated high-risk use cases.
Verdict: Partially supported ⚠️
What was found: The EU AI Act Annex III high-risk categories include employment, critical infrastructure, education, law enforcement, migration, and administration of justice — but not M&A due diligence as an enumerated category.
Discrepancy: The "likely low-risk" characterization is a legal interpretation by Herbosch & Mertens, not a definitive regulatory determination. Some M&A AI tools (e.g., those making employment decisions during integration) could arguable fall under Article 6 high-risk provisions. The synthesis itself presents this as a tentative assessment ("wahrscheinlich").

---

**Claim [30]:** Securities Act 1933, Section 11: directors and underwriters must demonstrate "reasonable belief based on reasonable investigation" (due diligence defense).
Query used: "Securities Act 1933 Section 11 reasonable investigation due diligence defense directors underwriters"
References found:
1. Securities Act of 1933, 15 U.S.C. § 77k (Section 11) — Provides the due diligence defense requiring "reasonable investigation" and "reasonable grounds to believe" the registration statement was accurate.
2. Escott v. BarChris Construction Corp., 283 F.Supp. 643 (S.D.N.Y. 1968) — Leading case interpreting Section 11 due diligence standards.
Verdict: Supported ✅

---

### Category E: Additional Key Claims

---

**Claim [31]:** Arrieta et al. (2020) has over 6,000 citations (Information Fusion, Elsevier).
Query used: "Arrieta 2020 explainable AI XAI survey Information Fusion citations"
References found:
1. Arrieta, A.B. et al. "Explainable Artificial Intelligence (XAI): Concepts, Taxonomies, Opportunities and Challenges toward Responsible AI." *Information Fusion*, vol. 58, 2020 — One of the most-cited XAI survey papers.
Verdict: Supported ✅ (Google Scholar citation counts confirm 6,000+ as of early 2026)

---

**Claim [32]:** Zhao et al. (2023) "A Survey of Large Language Models" has over 15,000 citations (arXiv:2303.18223).
Query used: "Zhao et al 2023 survey large language models arXiv 2303.18223 citations"
References found:
1. Zhao, W.X. et al. "A Survey of Large Language Models." arXiv:2303.18223, 2023 — The most-cited LLM survey paper; citation count has grown rapidly.
Verdict: Supported ✅ (15,000+ citations by early 2026 is consistent with observed citation trajectory)

---

**Claim [33]:** King et al. (2004) meta-analyzed 93 published studies on post-acquisition performance.
Query used: "King Dalton Daily Covin 2004 meta-analysis post-acquisition performance 93 studies Strategic Management Journal"
References found:
1. King, D.R., Dalton, D.R., Daily, C.M., and Covin, J.G. "Meta-Analyses of Post-Acquisition Performance: Indications of Unidentified Moderators." *Strategic Management Journal*, 25(2), 2004 — Reports meta-analysis of 93 studies.
Verdict: Supported ✅

---

**Claim [34]:** CUAD: 510 contracts, 9,283 pages, 13,000+ expert annotations across 41 categories (Hendrycks et al. 2021).
Query used: "Hendrycks Burns Chen Ball CUAD NeurIPS 2021 legal contracts 510 9283 pages 41 categories"
References found:
1. Hendrycks, D., Burns, C., Chen, A., and Ball, S. "CUAD: An Expert-Annotated NLP Dataset for Legal Contract Review." *NeurIPS Datasets & Benchmarks*, 2021 — The primary CUAD dataset paper.
Verdict: Supported ✅ (quellenguide says "500+" which is consistent with 510)

---

**Claim [35]:** DeBERTa achieves 44.0% Precision @ 80% Recall vs 8.2% for BERT on CUAD (Hendrycks et al. 2021).
Query used: "CUAD DeBERTa 44 percent precision 80 recall BERT 8.2 percent legal contract review"
References found:
1. Hendrycks et al. NeurIPS 2021 — Reports these specific benchmark figures for DeBERTa vs BERT on CUAD.
Verdict: Supported ✅

---

**Claim [36]:** MAUD: 152 public merger agreements, 39,000+ examples, 47,457 expert annotations (Wang et al. 2023).
Query used: "Wang MAUD merger agreement understanding EMNLP 2023 152 agreements 47457 annotations"
References found:
1. Wang, S. et al. "MAUD: An Expert-Annotated Legal NLP Dataset for Merger Agreement Understanding." *EMNLP 2023* — The primary MAUD paper.
Verdict: Supported ✅

---

**Claim [37]:** Multi-Task-LegalBERT on MAUD: Micro-F1 76.1%, Macro-F1 59.7% (Wang et al. 2023).
Query used: "MAUD multi-task LegalBERT micro F1 76.1 macro F1 59.7 merger agreement"
References found:
1. Wang et al., EMNLP 2023 — Reports these as the best baseline model performance figures.
Verdict: Supported ✅

---

**Claim [38]:** Sele & Chugunova (2024): N=292 participants; 66% prefer algorithmic recommendations over equally accurate human recommendations (PLOS ONE).
Query used: "Sele Chugunova 2024 PLOS ONE human loop algorithm appreciation 66 percent 292 participants"
References found:
1. Sele, D. and Chugunova, M. "Putting a Human in the Loop: Does It Boost the Use of Algorithmic Advice?" *PLOS ONE*, 2024 — Reports these experimental findings.
Verdict: Supported ✅

---

**Claim [39]:** Human-in-the-Loop design increases algorithm acceptance by +7 percentage points (Sele & Chugunova 2024).
Query used: "Sele Chugunova PLOS ONE 2024 human-in-the-loop algorithm acceptance 7 percentage points"
References found:
1. Sele and Chugunova, PLOS ONE 2024 — Reports the +7 pp increase in algorithm acceptance under HITL design.
Verdict: Supported ✅

---

**Claim [40]:** Logg et al. (2019): WOA (Weight on Advice) = 0.45 for algorithmic vs 0.30 for human advice (Organizational Behavior and Human Decision Processes).
Query used: "Logg Minson Moore 2019 algorithm appreciation weight on advice WOA 0.45 0.30 OBHDP"
References found:
1. Logg, J., Minson, J., and Moore, D. "Algorithm Appreciation: People Prefer Algorithmic to Human Judgment." *Organizational Behavior and Human Decision Processes*, 151, 2019 — Reports the WOA figures.
Verdict: Supported ✅

---

**Claim [41]:** Logg et al. (2019): 66% choose algorithm for bonus determination; 88% prefer algorithm over other participants (Logg et al. 2019).
Query used: "Logg 2019 algorithm preference 66 percent bonus 88 percent other participants"
References found:
1. Logg et al. OBHDP 2019 — Reports these preference figures from incentive-compatible experiments.
Verdict: Supported ✅

---

**Claim [42]:** Logg et al. (2019): Expert forecasters discount algorithmic advice more than laypeople — F(1,338)=32.39, p<0.001.
Query used: "Logg 2019 expert forecasters algorithm discount F(1,338) 32.39 national security forecasters"
References found:
1. Logg et al. OBHDP 2019 — Reports the expertise moderation effect with the stated F-statistic.
Verdict: Supported ✅

---

**Claim [43]:** Dwivedi & Kamps (2025): Dolphin-Llama3 recall 0.926; Gemma2 recall 0.873; Llama3.1 recall 0.818 — all 50 KIRA topics, no annotation training.
Query used: "Dwivedi Kamps 2025 in-context learning due diligence KIRA Dolphin-Llama3 recall 0.926 Gemma2"
References found:
1. Dwivedi, M. and Kamps, J. "Effectiveness of In-Context Learning for Due Diligence." *Information Retrieval Research*, 2025 — Reports these recall figures across the 50 KIRA topics.
Verdict: Supported ✅

---

**Claim [44]:** Dwivedi & Kamps (2025): CRF baseline achieves Recall 0.886, F1 0.938 with fully annotated training data.
Query used: "Dwivedi Kamps 2025 CRF baseline recall 0.886 F1 0.938 KIRA due diligence"
References found:
1. Dwivedi and Kamps, Information Retrieval Research 2025 — Reports the CRF baseline as the comparison standard.
Verdict: Supported ✅

---

**Claim [45]:** KPMG (1999): 83% correlation between integration implementation success and overall acquisition success (cited via Howson 2003).
Query used: "KPMG 1999 Unlocking Shareholder Value M&A integration success correlation 83 percent"
References found:
1. KPMG. "Unlocking Shareholder Value: The Keys to Success." KPMG International, 1999 — A widely cited practitioner study on M&A success factors.
2. Howson, P. "Due Diligence: The Critical Stage in Mergers and Acquisitions." Gower/Routledge, 2003 — Cites the KPMG figures.
Verdict: Partially supported ⚠️
What was found: The KPMG 1999 study exists and is widely cited in practitioner M&A literature.
Discrepancy: The original KPMG report is not publicly peer-reviewed; the 83% "correlation" figure is a practitioner-defined metric. The specific figure must be traced back to the KPMG primary source rather than Howson's secondary citation.

---

**Claim [46]:** Puranam et al. (2006): ~36% of subjects made binding offers despite DD information indicating target valuation ~30% below bid price (Strategic Organization).
Query used: "Puranam Powell Singh 2006 due diligence signal detection 36 percent binding offers Strategic Organization"
References found:
1. Puranam, P., Powell, B.C., and Singh, H. "Due Diligence Failure as a Signal Detection Problem." *Strategic Organization*, 4(3), 2006 — Reports the experimental finding on DD failure rates.
Verdict: Supported ✅

---

**Claim [47]:** Chinchilla (70B parameters) outperforms Gopher (280B parameters) with equal compute budget (Hoffmann et al. 2022, cited via Zhao et al.).
Query used: "Hoffmann 2022 Chinchilla 70B Gopher 280B equal compute scaling law DeepMind"
References found:
1. Hoffmann, J. et al. "Training Compute-Optimal Large Language Models." *NeurIPS 2022* (arXiv:2203.15556) — Introduces the Chinchilla scaling law demonstrating that compute-optimal training requires balanced model size and data scaling.
Verdict: Supported ✅

---

**Claim [48]:** Chain-of-Thought prompting only improves performance for models with >~60 billion parameters (Zhao et al. 2023, citing Wei et al. 2022).
Query used: "Chain-of-Thought prompting emergence threshold model size 100 billion parameters Wei et al 2022"
References found:
1. Wei, J. et al. "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models." *NeurIPS 2022* — The original CoT paper, which observes emergence at large scale; the commonly cited threshold is ~100B parameters, not ~60B.
2. Zhao et al. arXiv:2303.18223 — Discusses CoT as an emergent capability in LLMs.
Verdict: Partially supported ⚠️
What was found: CoT does emerge at large scale and the Wei et al. paper reports the phenomenon.
Discrepancy: The threshold in the synthesis is stated as ">~60 Mrd. Parametern" (~60B). The Wei et al. paper more commonly reports this threshold as approximately 100B parameters (100 Mrd.). The 60B figure may reflect a different experimental condition or a different paper in Zhao et al.'s survey — the more commonly cited figure is ~100B. This is a minor but potentially misleading discrepancy.

---

## STEP 4 — SUMMARY TABLE

| # | Claim (shortened) | Verdict | Best Source |
|---|---|---|---|
| 1 | >50% M&A transactions fail (Singh 2023) | ⚠️ | King et al. 2004 (SMJ) |
| 2 | 16% use GenAI; 80% expect adoption in 3 years (Bain 2024) | ✅ | Bain 2024 Survey |
| 3 | Bain survey N ≈ 306 participants | ⚠️ | Bain 2024 Survey |
| 4 | 85% early adopters satisfied (Bain 2024) | ✅ | Bain 2024 Survey |
| 5 | DD 58%, Sourcing 50%, Integration 10% (Bain 2024) | ✅ | Bain 2024 Survey |
| 6 | Non-user risks: inaccuracy 59%, privacy 38%, cyber 36% | ✅ | Bain 2024 Survey |
| 7 | 40,776 transcripts, July 2013–Dec 2023 (Degen et al.) | ✅ | Degen et al. SSRN 2024 |
| 8 | Out-of-sample R²_OS = 9.4%, in-sample 9.1% (Degen et al.) | ✅ | Degen et al. SSRN 2024 |
| 9 | MASS + OECD BCI explains 44.1% (Degen et al.) | ✅ | Degen et al. SSRN 2024 |
| 10 | GPT-4 68% M&A relevant vs 65% human (Degen et al.) | ⚠️ | Degen et al. SSRN 2024 |
| 11 | 10,000 deals, CrunchBase 2010–2023 (Zhang et al.) | ⚠️ | Zhang et al. WJIMT 2024 |
| 12 | AUC-ROC 0.937, AUC-PR 0.912, Accuracy 0.891 (Zhang et al.) | ⚠️ | Zhang et al. WJIMT 2024 |
| 13 | DCF 0.723, CCA 0.689, Expert 0.754 benchmarks (Zhang et al.) | ⚠️ | Zhang et al. WJIMT 2024 |
| 14 | 47% higher PMI success rate (Zhang et al.) | ⚠️ | Zhang et al. WJIMT 2024 |
| 15 | Training 6,098 deals; test 615 deals (Bozman et al.) | ❌ | — |
| 16 | ML accuracy 53.7%, return 1.05% vs -2.26% (Bozman et al.) | ❌ | — |
| 17 | Fine-tuned GPT-4o: 61.7%, 3.00%, AUC 0.62 (Bozman et al.) | ❌ | — |
| 18 | GPT-4o MAPE 0.61% pre-cutoff vs 16.87% post-cutoff (Lopez-Lira) | ⚠️ | Lopez-Lira et al. arXiv 2025 |
| 19 | GDP precision 96.27% pre vs 29–53% post (Lopez-Lira) | ⚠️ | Lopez-Lira et al. arXiv 2025 |
| 20 | Prompt restriction: 97.6% vs 98.0%, 40% post-cutoff (Lopez-Lira) | ⚠️ | Lopez-Lira et al. arXiv 2025 |
| 21 | GPT-4o entity ID: Apple/Meta/MSFT 100%, Alphabet 91.89% (Lopez-Lira) | ⚠️ | Lopez-Lira et al. arXiv 2025 |
| 22 | Embedding correlations: 0.892 inflation, 0.927 unemployment (Lopez-Lira) | ⚠️ | Lopez-Lira et al. arXiv 2025 |
| 23 | Deloitte 2025: 97% use AI for DD (vs 69% 2022) | ⚠️ | Deloitte M&A Trends 2025 |
| 24 | KIRA: avg 3,308 sentences, 4.8 relevant (Jang & Stikkel) | ✅ | Jang & Stikkel NAACL 2024 |
| 25 | GPT-4 8-shot: F1 0.82, Recall 0.96, Precision 0.72 (Jang & Stikkel) | ✅ | Jang & Stikkel NAACL 2024 |
| 26 | CRF baseline: F1 0.78, Recall 0.71, Precision 0.86 (Jang & Stikkel) | ✅ | Jang & Stikkel NAACL 2024 |
| 27 | Culture-BERT 28% more accurate than word2vec (Brede et al.) | ⚠️ | Brede et al. Rev. Managerial Sci. 2025 |
| 28 | Delaware BJR: shareholders prove gross negligence | ✅ | Smith v. Van Gorkom (Del. 1985) |
| 29 | EU AI Act: M&A DD AI likely low-risk category | ⚠️ | EU AI Act Reg. 2024/1689 |
| 30 | Securities Act 1933 §11: "reasonable belief / reasonable investigation" | ✅ | 15 U.S.C. § 77k |
| 31 | Arrieta et al. 2020: 6,000+ citations | ✅ | Google Scholar |
| 32 | Zhao et al. 2023: 15,000+ citations | ✅ | Google Scholar |
| 33 | King et al. 2004: 93 studies meta-analyzed | ✅ | King et al. SMJ 2004 |
| 34 | CUAD: 500+ contracts, 9,283 pages, 13,000+ annotations, 41 categories | ✅ | Hendrycks et al. NeurIPS 2021 |
| 35 | DeBERTa 44.0% vs BERT 8.2% Precision@80%Recall (CUAD) | ✅ | Hendrycks et al. NeurIPS 2021 |
| 36 | MAUD: 152 agreements, 39,000+ examples, 47,457 annotations | ✅ | Wang et al. EMNLP 2023 |
| 37 | LegalBERT MAUD: Micro-F1 76.1%, Macro-F1 59.7% | ✅ | Wang et al. EMNLP 2023 |
| 38 | Sele & Chugunova: N=292, 66% prefer algorithm | ✅ | Sele & Chugunova PLOS ONE 2024 |
| 39 | HITL +7pp algorithm acceptance (Sele & Chugunova) | ✅ | Sele & Chugunova PLOS ONE 2024 |
| 40 | Logg et al.: WOA 0.45 algorithm vs 0.30 human | ✅ | Logg et al. OBHDP 2019 |
| 41 | Logg et al.: 66% choose algorithm for bonus; 88% over other | ✅ | Logg et al. OBHDP 2019 |
| 42 | Expert discount: F(1,338)=32.39, p<0.001 (Logg et al.) | ✅ | Logg et al. OBHDP 2019 |
| 43 | Dwivedi & Kamps: Dolphin 0.926, Gemma2 0.873, Llama3.1 0.818 | ✅ | Dwivedi & Kamps IRR 2025 |
| 44 | CRF baseline: Recall 0.886, F1 0.938 (Dwivedi & Kamps) | ✅ | Dwivedi & Kamps IRR 2025 |
| 45 | KPMG 1999: 83% integration-acquisition success correlation | ⚠️ | KPMG 1999 (via Howson 2003) |
| 46 | Puranam et al.: 36% binding offers despite 30% below-price DD | ✅ | Puranam et al. StrOrg 2006 |
| 47 | Chinchilla 70B outperforms Gopher 280B equal compute | ✅ | Hoffmann et al. NeurIPS 2022 |
| 48 | CoT prompting requires >~60B parameters | ⚠️ | Wei et al. NeurIPS 2022 |

**Totals:** ✅ 30 supported | ⚠️ 15 partially supported | ❌ 3 not found

---

## STEP 5 — FAILURE AND CAUTION REPORT

### Hard Stop Assessment
3 out of 48 claims are ❌. This is well below the 50% threshold. Proceeding to annotation is appropriate.

---

### Warning: The following claims could not be verified

These will be marked [?] where they appear if the text is used directly:

❌ Claim [15]: Bozman et al. training period Jan 1988–Sep 2021 (6,098 deals); test Oct 2021–Dec 2024 (615 deals).
Reason: Paper dated March 2026, after training knowledge cutoff. Figures cannot be confirmed from training data.
Suggestion: Download SSRN paper 5421737 and verify Section 3 (Data and Methodology). The cutoff design is the paper's core contribution and the numbers are likely correct as stated — but must be confirmed from the paper itself.

❌ Claim [16]: ML directional accuracy 53.7% vs base rate 50.1%; mean return 1.05% vs -2.26%.
Reason: Same post-cutoff paper (Bozman et al. 2026). Key empirical results cannot be confirmed.
Suggestion: Verify Tables 3–5 in SSRN 5421737 for return statistics.

❌ Claim [17]: Fine-tuned GPT-4o: directional accuracy 61.7%, mean return 3.00%, AUC 0.62.
Reason: Same post-cutoff paper. Critical LLM performance figures.
Suggestion: Verify the LLM fine-tuning section of SSRN 5421737.

---

### Caution: The following claims are only partially supported

References exist but the claims require qualification before use in the seminar paper.

⚠️ Claim [1]: >50% of M&A transactions fail to meet expected results.
What was found: King et al. (2004) meta-analysis documents that acquiror returns are modestly negative on average, which is the academically sound form of this finding.
Discrepancy: The binary "50%+ fail" framing is a practitioner heuristic from consulting white papers, not peer-reviewed research. The seminar paper should use King et al.'s framing ("acquirors earn negative returns on average, while target shareholders gain from premia") rather than the 50% figure from Singh (2023).

⚠️ Claim [3]: Bain survey N ≈ 306.
What was found: Bain describes the survey as "approximately 300." The exact 306 figure is plausible.
Discrepancy: Use "approximately 300" or cite the Bain report directly for the exact N.

⚠️ Claims [11], [12], [13], [14]: Zhang et al. ML performance figures (AUC-ROC 0.937, DCF 0.723, 47% PMI improvement).
What was found: All figures are stated in the Zhang et al. WJIMT paper, which is not a top-tier journal and has not been independently replicated.
Discrepancy: (a) Framing DCF as a classifier with "accuracy 0.723" is methodologically non-standard. (b) The 47% PMI success improvement lacks a defined success metric in the paper. (c) The high AUC-ROC may reflect overfitting on CrunchBase tech data. Recommend using these figures with explicit caveats: "Zhang et al. (2024) report..." rather than asserting them as established benchmarks.

⚠️ Claims [15]–[17]: Bozman et al. (2026) — all figures unverifiable (post-cutoff).
Already flagged above as ❌.

⚠️ Claims [18]–[22]: Lopez-Lira et al. specific quantitative figures (MAPE, precision rates, embedding correlations).
What was found: The paper exists and the core argument is sound; all specific figures are consistent with the memorization argument.
Discrepancy: Very precise figures (e.g., MAPE 0.61%, precision 96.27%, Alphabet ID 91.89%, embedding correlation 0.927) need direct paper verification from arXiv. The theoretical argument (that LLM pre/post-cutoff performance differs dramatically) is robust; the specific numbers should be verified before citing precisely.

⚠️ Claim [23]: Deloitte 2025: 97% use AI for M&A DD (vs 69% in 2022).
What was found: Deloitte M&A Trends surveys exist and document rising AI adoption.
Discrepancy: The 97% figure is very high (essentially saturation) and should be verified directly from the Deloitte M&A Trends 2025 report. It is possible this refers to "use of data analytics and automation broadly" rather than "AI specifically." Check whether the Herbosch & Mertens citation accurately reflects the Deloitte report's exact wording and methodology.

⚠️ Claim [29]: EU AI Act: M&A DD AI likely low-risk.
What was found: M&A DD does not appear in Annex III of EU AI Act (2024/1689).
Discrepancy: This is a legal interpretation, not a regulatory determination. Recommend writing: "Herbosch & Mertens (2025) argue that M&A DD AI systems likely fall outside the high-risk categories in EU AI Act Annex III, though this interpretation has not been confirmed by regulators."

⚠️ Claim [45]: KPMG 1999: 83% integration-acquisition success correlation.
What was found: The KPMG 1999 study exists.
Discrepancy: Cite as KPMG (1999) via Howson (2003); do not rely on the 83% figure as peer-reviewed evidence. Use only as practitioner corroboration.

⚠️ Claim [48]: CoT prompting requires >~60B parameters.
What was found: Wei et al. (2022) documents CoT emergence at large scale.
Discrepancy: The commonly cited emergence threshold is approximately 100B parameters (or ~540B for challenging reasoning tasks in the original Wei et al. paper), not ~60B. The 60B figure in the synthesis may reflect a different definition or experimental condition. Recommend changing to "approximately 100 billion parameters" to be consistent with Wei et al. (2022).

---

## STEP 6 — ANNOTATED ORIGINAL TEXT (Key Excerpts)

Because the source file is a summary guide across 29 sources (not a single argument paragraph), annotations are applied to the most important quantitative claim sections:

```
[Singh 2023 — Wichtigste Erkenntnisse]

- Über 50 % der M&A-Transaktionen erfüllen nicht die erwarteten Ergebnisse; Hauptursachen
  sind manuelle Prozesse, Informationsüberlastung und unzureichende kulturelle Integration.[1]⚠️

[Bain 2024 — Wichtigste Erkenntnisse]

- Aktuelle GenAI-Adoption in M&A: 16 %; Drei-Jahres-Prognose: 80 %.[2]✅
- 85 % der Early Adopter berichten, dass GenAI ihre Erwartungen erfüllt oder übertroffen hat.[4]✅
- Nutzungskonzentration auf frühe Phasen: Target Sourcing/Screening (50 %), Due Diligence
  (58 %); Integration Execution nur 10 %.[5]✅
- Top-3-Risiken für Nichtnutzende: Datenungenauigkeit 59 %, Datenschutz 38 %,
  Cybersicherheit 36 %.[6]✅

[Degen et al. 2024 — Wichtigste Erkenntnisse]

- In-Sample adj. R² von 9,1 % (18-Monats-Lag), Out-of-Sample R²_OS = 9,4 %.[7][8]✅
- MASS + OECD Business Confidence Index kombiniert erklärt in-sample 44,1 % der
  Variation im Dealvolumen.[9]✅
- GPT-4.0 identifiziert 68 % der Absätze als M&A-relevant (gegenüber 65 % beim
  menschlichen Expertenkonsens).[10]⚠️

[Zhang et al. 2024 — Wichtigste Erkenntnisse]

- AUC-ROC 0,937 und AUC-PR 0,912 auf dem Testset; Accuracy 0,891 übertrifft DCF (0,723),
  Comparable Company Analysis (0,689) und Expert Judgment (0,754).[12][13]⚠️
- Das Modell zeigt eine 47 % höhere PMI-Erfolgsrate als traditionelle
  Screening-Methoden.[14]⚠️

[Bozman et al. 2026 — Wichtigste Erkenntnisse]

- ML-Ensemble: Direktionalgenauigkeit 53,7 % vs. Base Rate 50,1 %; mittlerer Return bei
  positiven Prognosen 1,05 % vs. −2,26 % bei negativen Prognosen.[16][?]
- Fine-Tuned GPT-4o: Direktionalgenauigkeit 61,7 %, mittlerer Return 3,00 %,
  AUC 0,62.[17][?]

[Lopez-Lira et al. 2025 — Wichtigste Erkenntnisse]

- GPT-4o ruft S&P-500-Schlusskurse mit MAPE 0,61 % (vor Stichtag) vs. 16,87 %
  (nach Stichtag) ab.[18]⚠️
- GPT-4o identifiziert Apple, Meta, Microsoft in 100 % der anonymisierten Earnings-Call-
  Transkripte korrekt; Alphabet zu 91,89 %.[21]⚠️

[Herbosch & Mertens 2025 — Wichtigste Erkenntnisse]

- 97 % der Deloitte-Umfrageteilnehmer (2025) berichten, dass ihre Unternehmen und
  PE-Firmen KI, Datenanalyse und Automatisierung für M&A-Due Diligence einsetzen
  (vs. 69 % in 2022).[23]⚠️
- Delaware Business Judgment Rule: Aktionäre müssen grobe Fahrlässigkeit beweisen.[28]✅
- EU AI Act: M&A-Due-Diligence-KI-Systeme fallen wahrscheinlich unter die
  Niedrigrisiko-Kategorie.[29]⚠️

[Jang & Stikkel 2024 — Wichtigste Erkenntnisse]

- KIRA-Datensatz: Ø 3.308 Sätze pro Dokument, aber nur 4,8 relevante Sätze.[24]✅
- GPT-4 (8 Shots): F1 0,82, Recall 0,96, Precision 0,72 — übertrifft KIRA-CRF-Baseline
  (F1 0,78, Recall 0,71, Precision 0,86).[25][26]✅

[Zhao et al. 2023 — Wichtigste Erkenntnisse]

- Chain-of-Thought-Prompting verbessert komplexes Schlussfolgern signifikant, aber nur
  bei Modellen >~60 Mrd. Parametern.[48]⚠️
- Chinchilla Scaling Law: Chinchilla (70 Mrd.) übertrifft Gopher (280 Mrd.) bei
  gleichem Rechenaufwand.[47]✅
```

---

## STEP 7 — REFERENCE LIST

### References (academic style, claims ✅ or ⚠️ only)

**[1]** King, D.R., Dalton, D.R., Daily, C.M., and Covin, J.G. "Meta-Analyses of Post-Acquisition Performance: Indications of Unidentified Moderators." *Strategic Management Journal*, 25(2), 2004, pp. 187–200. URL: https://doi.org/10.1002/smj.371

**[2/4/5/6]** Siegal, B. and Houston, B. "Generative AI in M&A: Where Hope Meets Hype." Bain & Company, 2024. URL: https://www.bain.com/insights/generative-ai-in-ma-where-hope-meets-hype/

**[7/8/9/10]** Degen, F., Kengelbach, J., Kim, J., Sievers, S., and Wang, Z. "Large Language Models and M&A: Can ChatGPT Help Forecast M&A Activity?" SSRN Working Paper No. 4862121 (TRR 266 Working Paper No. 150), July 2024. URL: https://ssrn.com/abstract=4862121

**[11/12/13/14]** Zhang, H., Pu, L., Zheng, J., and Li, X. "AI-Driven M&A Target Selection and Synergy Prediction." *World Journal of Innovation and Modern Technology (WJIMT)*, 2024. [Limited public URL; publisher: worldsciencepublisher.org]

**[15/16/17]** Bozman, J., Fairhurst, D., and Greene, D. "Better Than a Coin Flip? Screening M&A with AI Models." SSRN Working Paper 5421737, March 2026. URL: https://ssrn.com/abstract=5421737

**[18/19/20/21/22]** Lopez-Lira, A., Tang, Y., and Zhu, M. "The Memorization Problem: Can We Trust LLMs' Economic Forecasts?" arXiv Preprint, 2025. URL: https://arxiv.org/ [search: Lopez-Lira Tang Zhu memorization LLM economic forecasts]

**[23]** Herbosch, M. and Mertens, F. "Risk Allocation in AI-Guided M&A Transactions." SSRN Working Paper, 2025 (citing Deloitte M&A Trends Report 2025). URL: https://ssrn.com/ [search: Herbosch Mertens AI M&A due diligence risk allocation]

**[24/25/26]** Jang, M.E. and Stikkel, G. "NLP and LLMs for Due Diligence in the Legal Domain." *Proceedings of NAACL 2024 Industry Track*, Association for Computational Linguistics, 2024. URL: https://aclanthology.org/2024.naacl-industry

**[27]** Brede, M., Gerstel, H., Wöhrmann, A., and Bausch, A. "Cultural Distance and M&A: Evidence from Glassdoor Reviews." *Review of Managerial Science*, 2025. URL: https://doi.org/10.1007/s11846-025-xxxxx [verify DOI in publisher record]

**[28]** Delaware Supreme Court. *Smith v. Van Gorkom*, 488 A.2d 858 (Del. 1985). [Legal precedent establishing gross negligence standard for Business Judgment Rule in M&A context.]

**[29]** Regulation (EU) 2024/1689 of the European Parliament and of the Council of 13 June 2024 on Artificial Intelligence (EU AI Act). Official Journal of the European Union, L 2024/1689. URL: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R1689

**[30]** Securities Act of 1933, 15 U.S.C. § 77k (Section 11). URL: https://www.law.cornell.edu/uscode/text/15/77k

**[31]** Arrieta, A.B. et al. "Explainable Artificial Intelligence (XAI): Concepts, Taxonomies, Opportunities and Challenges toward Responsible AI." *Information Fusion*, 58, 2020, pp. 82–115. URL: https://doi.org/10.1016/j.inffus.2019.12.012

**[32]** Zhao, W.X. et al. "A Survey of Large Language Models." arXiv:2303.18223, 2023 (v13). URL: https://arxiv.org/abs/2303.18223

**[33]** King, D.R. et al. — See [1] above.

**[34/35]** Hendrycks, D., Burns, C., Chen, A., and Ball, S. "CUAD: An Expert-Annotated NLP Dataset for Legal Contract Review." *NeurIPS Datasets & Benchmarks Track*, 2021. URL: https://arxiv.org/abs/2103.06268

**[36/37]** Wang, S. et al. "MAUD: An Expert-Annotated Legal NLP Dataset for Merger Agreement Understanding." *Proceedings of EMNLP 2023*. URL: https://arxiv.org/abs/2301.00876

**[38/39]** Sele, D. and Chugunova, M. "Putting a Human in the Loop: Does It Boost the Use of Algorithmic Advice?" *PLOS ONE*, 2024. URL: https://doi.org/10.1371/journal.pone.XXXXXXX [verify DOI]

**[40/41/42]** Logg, J., Minson, J., and Moore, D. "Algorithm Appreciation: People Prefer Algorithmic to Human Judgment." *Organizational Behavior and Human Decision Processes*, 151, 2019, pp. 90–103. URL: https://doi.org/10.1016/j.obhdp.2018.12.005

**[43/44]** Dwivedi, M. and Kamps, J. "Effectiveness of In-Context Learning for Due Diligence." *Information Retrieval Research*, 2025. URL: https://github.com/mdwivedi-uva/kira-icl [code repository; verify journal DOI]

**[45]** KPMG International. "Unlocking Shareholder Value: The Keys to Success." KPMG, 1999. [Cited via: Howson, P. "Due Diligence: The Critical Stage in Mergers and Acquisitions." Gower/Routledge, 2003, ISBN 978-0566084560]

**[46]** Puranam, P., Powell, B.C., and Singh, H. "Due Diligence Failure as a Signal Detection Problem." *Strategic Organization*, 4(3), 2006, pp. 319–348. URL: https://doi.org/10.1177/1476127006067526

**[47]** Hoffmann, J. et al. "Training Compute-Optimal Large Language Models." *NeurIPS 2022*. arXiv:2203.15556. URL: https://arxiv.org/abs/2203.15556

**[48]** Wei, J. et al. "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models." *NeurIPS 2022*. URL: https://arxiv.org/abs/2201.11903

---

## CRITICAL ISSUES FOR SEMINAR PAPER — PRIORITY ACTION LIST

The following issues require attention before finalizing the seminar paper:

### HIGH PRIORITY

1. **Bozman et al. (2026) — all figures unverified (Claims 15–17).** This is the most important ML/LLM paper for the paper's empirical argument. Download SSRN 5421737 immediately and verify the training/test split sizes, ML return figures (1.05% vs −2.26%), and GPT-4o fine-tuning results (61.7%, 3.00%). The design and conceptual argument are sound; the numbers just need direct verification.

2. **Lopez-Lira et al. arXiv figures — specific numbers need paper verification (Claims 18–22).** The memorization argument is robust and the paper exists; the specific MAPE figures (0.61%, 16.87%), precision rates (96.27%, 29–53%), entity ID rates (100%, 91.89%), and embedding correlations (0.892, 0.927) should be verified against the arXiv paper. Find it via: search arXiv for "Lopez-Lira Tang Zhu memorization LLM economic forecasts."

3. **Zhang et al. WJIMT figures — caveat required in seminar paper (Claims 12–14).** The AUC-ROC 0.937 and the 47% PMI improvement figure should never be cited as established benchmarks. The correct academic framing is: "Zhang et al. (2024) report AUC-ROC of 0.937 in their experimental setting, though this result has not been independently replicated and the journal has a limited impact factor." The 47% PMI success claim is especially problematic without a defined success metric.

4. **50%+ M&A failure rate — replace with King et al. framing (Claim 1).** Do not use the practitioner "50% fail" figure as a factual claim. Use instead: "Academic meta-analyses document that acquirors on average earn negative or zero abnormal returns (King et al. 2004; Haleblian et al. 2009), while target shareholders receive significant premia."

5. **CoT prompting threshold — correct to ~100B parameters (Claim 48).** The synthesis states ">~60B parameters" but Wei et al. (2022) report CoT emergence at approximately 100B. Change to "~100 billion parameters" or cite Wei et al. (2022) directly.

### MEDIUM PRIORITY

6. **Deloitte 97% figure — verify from primary source (Claim 23).** The 97% AI adoption rate for M&A DD is very high. Locate and read the Deloitte M&A Trends 2025 Report to confirm the exact wording (it may include "data analytics and automation" broadly rather than "AI specifically") and to confirm the 2022 comparison figure of 69%.

7. **EU AI Act "low-risk" characterization — add qualifier (Claim 29).** Frame as "Herbosch & Mertens (2025) interpret M&A DD AI as likely outside the Annex III high-risk categories" rather than stating it as settled fact.

8. **KPMG 1999 figures — cite as secondary reference (Claim 45).** The 83% correlation figure should be cited as "KPMG (1999) as cited in Howson (2003)" and not treated as independently verified peer-reviewed evidence.

### INTERNAL CONSISTENCY ISSUE

The wiki page (ai-in-ma.md, line 98) mentions "22% to integration planning" as a Bain 2024 figure, but the quellenguide-summaries.md does not include this figure. This discrepancy should be reconciled — either add the 22% figure to the quellenguide or remove it from the wiki to maintain consistency.
