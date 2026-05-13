# Quellenguide: "Der Einfluss von KI auf M&A"
## Strukturierte Quellendokumentation für die Seminararbeit

**Seminar:** Bachelorseminar Mergers & Acquisitions (Thema 7), Goethe-Universität Frankfurt  
**Arbeitstitel:** Der Einfluss von KI auf M&A  
**Gliederung:** 5 Kapitel + Grundlagen  
**Stand:** Mai 2026

---

## 1. Einleitung (~2 Seiten)

### Singh (2023): The Transformative Potential of Artificial Intelligence and Its Impact on M&A Transactions

**Quellentyp:** Pflichtlektüre / Peer-reviewed Theorie

**Abschnitt:** 1 (Einleitung) — Querschnittsquelle; primär zu 2.1/3 relevant

**Was steht in der Quelle:**  
Singh untersucht aus rechtsanwaltlicher Perspektive, wie KI den gesamten M&A-Lebenszyklus (Strategie, Target-Identifikation, Due Diligence, Verhandlung, Integration) transformieren kann. Der Beitrag betont, dass über 50% der M&A-Deals fehlschlagen und zeigt konkrete KI-Anwendungen von Target-Screening über Dokumentenanalyse bis zur Integrationsvorbereitung. Zentrale These: KI kann Effizienz stark erhöhen, kann aber menschliches Urteil niemals ersetzen.

**Was wir rausnehmen:**  
- Kernstatistik: >50% M&A-Deals scheitern (Motivator für Forschungsfrage)
- KI-Einsatz über alle M&A-Phasen möglich (Evidence für Breite)
- Besondere Stärke: Legal DD, Dokumentenautomatisierung, Due-Diligence-Risikoerkennung
- Menschliche Grenzen: Verhandlung, kulturelle Integration bleiben Domäne von Menschen

**Schlüsselzitat:**
> "AI has the ability to significantly improve M&A deals by enhancing efficiency and decision-making. However, its limitations must be acknowledged, and human expertise must be matched with AI skills for desired results."

**Was bleibt offen:**
- Welche empirischen Belege gibt es für die behaupteten Effizienzgewinne?
- Wie lässt sich "Erfolg" einer M&A messbar definieren?
- Was sind die Grenzen von KI in hochkomplexen Integrationsprozessen konkret?

---

### Bain & Company (2024): Generative AI in M&A: Where Hope Meets Hype

**Quellentyp:** Praxisbericht / Consulting-Studie (nicht peer-reviewed)

**Abschnitt:** 1 (Einleitung) — Querschnittsquelle; auch 3.1, 3.2 relevant

**Was steht in der Quelle:**  
Bain-Umfrage unter 306+ M&A-Praktiker:innen zeigt aktuellen Adoptionsstand und Erwartungen. GenAI-Einsatz derzeit bei nur 16%, aber 80% erwarten Einsatz innerhalb 3 Jahren. Nutzer konzentrieren sich auf Target-Sourcing/Screening (38–50%) und Due Diligence (58%). 85% Zufriedenheit unter Early Adopters. Top-Risiken: Datenungenauigkeit (59%), Datenschutz (38%), Cybersecurity (36%).

**Was wir rausnehmen:**  
- **Zentrale Adoption-Zahlen:** 16% heute → 80% in 3 Jahren (Motivator für Zeitlichkeit der Forschungsfrage)
- Phasenfokus: Aktuell Target-Finding > Due Diligence >> Integration (zeigt Forschungs-Lücken)
- Praktiker-Perspektive: Effizienzgewinne klar, aber nicht gleichbedeutend mit besseren Deals
- Risk-Hierarchy: Datenqualität ist Top-Concern, nicht Haftung oder XAI

**Schlüsselzitat:**
> "Reviewing more deals faster is not equivalent to making better decisions. Competitive differentiation requires building on existing M&A process strengths."

**Was bleibt offen:**
- Hat sich die Adoption 2025/2026 wie erwartet entwickelt (Post-Prognose)?
- Was ist der aktuelle Status bei Integration (wo Adoption laut Report am niedrigsten)?
- Unterscheiden sich Bedenken zwischen Tech/Finance/anderen Sektoren?

---

### Bremen (2024): AI accelerates M&A into the future

**Quellentyp:** Pflichtlektüre / Praxisbericht (WTW, nicht peer-reviewed)

**Abschnitt:** 1 (Einleitung) — Querschnittsquelle; auch 2.1, 3, 4 relevant

**Was steht in der Quelle:**  
WTW-Artikel (Senior Managing Director John Bremen) argumentiert, dass erfolgreiche Führungskräfte KI bereits zur Prozessoptimierung einsetzen. Deckt alle M&A-Phasen ab: Sell-Side-Vorbereitung, Target-ID, Bewertung, Due Diligence, Synergieprüfung, Deal-Tracking, Integration. Kern: KI automatisiert Datenanalyse und Dokumentenprüfung, freut aber strategische, menschliche Aufgaben. **Verantwortungsvolle Governance** ist zentral: Verstehen von KI-Grenzen, Nutzer-Schulung, ethische Standards, Datenschutz, Bias-Adressierung, Regulierungshaftung.

**Was wir rausnehmen:**  
- KI-Anwendungen systematisch über alle 6+ M&A-Phasen
- Prompt Engineering als operative Kompetenz in Due Diligence
- Governance-Rahmen: 6 Komponenten (Verständnis, Schulung, Ethics, Datenschutz, Bias-Management, Regulierung)
- Positionierung: KI als Produktivitätsverstärker, nicht als Job-Ersatz
- Imperativ: "Nicht erste, aber auch nicht letzte sein" — Window to Build Capabilities Now

**Schlüsselzitat:**
> "Effective leaders know they don't need to go first, but they also shouldn't go last."

**Was bleibt offen:**
- Welche konkrete Trainingsmodule für M&A-Teams?
- Wie lässt sich "ethische Nutzung" in Deal-Kontext operationalisieren?
- Governance-Unterschiede zwischen Jurisdiktionen (Bremen focused mostly on US-context)?

---

## 2. Grundlagen (~5–6 Seiten)

### 2.1 Der M&A-Prozess: Phasen und Informationsasymmetrie

#### Howson (2003): Due Diligence: The Critical Stage in Mergers and Acquisitions

**Quellentyp:** Lehrbuch / Praxishandbuch

**Abschnitt:** 2.1 (M&A-Prozess, klassische DD)

**Was steht in der Quelle:**  
Howson ist das Standardwerk für den klassischen DD-Prozess. Argumentiert, dass DD eine **Projektmanagement**-Aufgabe ist (nicht nur Finanz-/Rechtsprüfung) und mindestens 5 Stränge umfassen muss: (1) Vermögen/Schulden-Verifikation, (2) Risikoidentifikation, (3) vertragliche Schutzmaßnahmen, (4) Synergieidentifikation, (5) Post-Acquisitions-Planung. Schätzt true M&A Failure Rate auf ~75% (nicht nur 50%). Zentral: DD sollte sowohl Risiken als auch Integrationsmöglichkeiten erschließen.

**Was wir rausnehmen:**  
- **DD-Definition:** Nicht nur Risikofixierung, sondern Springboard für PMI-Planung
- **5 DD-Stränge:** Breiter als nur Legal/Financial (15 Disziplinen über 13 Kapitel)
- **Failure-Erklärung:** "Zu sehr auf Finanzkennzahlen fokussiert, zu wenig Planung"
- **Kalibration:** DD-Schwerpunkt sollte zum M&A-Typ passen (Bowyer 5-Kategorien)
- **Implikation für KI:** KI kann einzelne Stränge (Legal DD, Finanzanalyse) optimieren, aber nicht Gesamtprogramm oder Projektmanagement ersetzen

**Schlüsselzitat:**
> "Due diligence is one of the most important but least well understood aspects of the acquisition process. It is not, as many believe, a chore to be left to the accountants and lawyers. To get the best from it, due diligence has to be properly planned and professionally managed."

**Was bleibt offen:**
- Welche der 15 Disziplinen sind derzeit von KI-Tools adressiert? (Lückenanalyse)
- Kann KI die Projektmanagement-Dimension von DD unterstützen (oder nur Inhalte)?
- Wie messen wir Erfolg: Risk-Mitigation? Synergy-Realisierung? Beides?

---

#### Lajoux (2024): The Art of M&A (6th ed.) — Chapters 1 & 6

**Quellentyp:** Lehrbuch / Standardwerk

**Abschnitt:** 2.1 (M&A-Prozess, DD-Definition)

**Was steht in der Quelle:**  
Lajoux definiert M&A als 8-Phasen-Zyklus (Strategie → Bewertung → Finanzierung → Strukturierung → DD → Verhandlung → Closing → Integration). DD ist Phase 5 und wird formal durch NDA/LOI getriggert. Die 6. Kapitel behandelt klassische DD systematisch: finanzielle Statements, Management/Operations, Legal Compliance, Dokumenten/Transaktion. Neu in 6. Auflage: Explizite Cyber-DD, kulturelle DD-Komponente, AI Asset Valuation Checklist, Referenz zu ChatGPT als Deal-Game-Changer.

**Was wir rausnehmen:**  
- **8-Phasen-Modell** mit DD als Phase 5 (strukturiert gegen klassische 7-Phase)
- **DD-Aktivitätsströme:** 4 parallele Workstreams (nicht sekvenziell)
- **Red Flags:** Strukturiert nach 4 Kategorien (Financial, Operational, Liability, Transactional)
- **VDR-Infrastruktur:** Moderne DD findet in virtuellen Datenräumen statt (relevant für KI-Integration)
- **Neu 2024:** Kulturelle DD, Cyber-DD, AI-Asset-Evaluierung explizit genannt
- **Governance:** Securities Act § 11 "Due Diligence Defense" — Nachweis einer **reasonable investigation** erforderlich (relevant für KI-Liability)

**Schlüsselzitat:**
> "Due diligence is the process of verifying that the company is what it claims to be and discovering risk exposures material to the transaction."

**Was bleibt offen:**
- Wie integriert man KI in die 4 Activity Streams konkret?
- Ersetzt KI die Human Direction of DD (Outside Counsel)?
- Genügt KI-Output als Nachweis einer "reasonable investigation" nach § 11?

---

#### Zhang et al. (2025): Does digital transformation affect corporate mergers and acquisitions? From the perspective of information asymmetry

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 2.1 (Informationsasymmetrie als M&A-Treiber)

**Was steht in der Quelle:**  
Chinesische Empirical Study (22.274 Firm-Year Observations, 2008–2022) zeigt, dass digitale Transformation M&A-Aktivität signifikant erhöht — primär durch **Reduktion externer Informationsasymmetrie** zwischen Akquisiteur und Target. Duales Mechanismus-Modell: (1) externe IA-Reduktion fördert M&A, (2) interne IA-Reduktion supprimiert selbstinteressierte, agentur-getriebene M&A. Netto-Effekt positiv für externe IA. Effekt stärker bei nicht-High-Tech und nicht-politisch-vernetzten Firmen.

**Was wir rausnehmen:**  
- **Theoretischer Kern:** Informationsasymmetrie ist der zentrale Mechanismus, durch den Digitalisierung M&A befördert
- **Duale Mechanismen:** Externe IA-Reduktion > Interne IA-Reduktion (netto positiv)
- **Moderatoren:** High-Tech-Status, politische Vernetzung, regionale Internet-Infrastruktur
- **Operationalisierung:** DT gemessen via Keyword-Häufigkeit in Geschäftsberichten (textmining)
- **Kausales Design:** IV-Regressions mit exogenem Shock (Broadband China policy)

**Schlüsselzitat:**
> "Digital transformation primarily reduces external information asymmetry, enabling acquirers to gain a clearer understanding of the true conditions of target firms, thereby facilitating corporate M&As."

**Was bleibt offen:**
- Übertragen sich diese Ergebnisse auf Western M&A Contexts (Studie ist China-fokussiert)?
- Ist KI speziell oder allgemeine Digitalisierung der operative Driver?
- Wie verhalten sich Synergy-Realisierungsraten unter IA-Reduktion?

---

#### Akerlof (1970): The Market for "Lemons"

**Quellentyp:** Klassisches Theorem / Peer-reviewed Theorie (Nobel Prize 2001)

**Abschnitt:** 2.1 (Theoretische Grundlagen: Informationsasymmetrie)

**Was steht in der Quelle:**  
Akerlof zeigt formal, wie Qualitätsunsicherheit und asymmetrische Information zu Marktversagen führen: Wenn Käufer Qualität nicht beobachten können, haben Low-Quality-Verkäufer Anreize, ihre Produkte als Average-Quality auszugeben. Dies senkt die durchschnittliche Marktqualität und schrumpft den Markt. Institutionen (Garantien, Brand, Lizenzen) entstehen als Reaktion. Für M&A direkt anwendbar: Targets haben bessere Information über ihre Qualität als Käufer.

**Was wir rausnehmen:**  
- **Adverse Selection Mechanismus:** Low-Quality-Targets können sich als Average ausgeben
- **Marktversagen:** Information Asymmetry kann zu suboptimalen Transaktionen führen
- **Institutionelle Lösungen:** Due Diligence, Warranties, Earnouts sind Mechanismen zur Bekämpfung
- **KI-Anwendung:** KI kann DD-Tiefe und Qualitätsüberprüfung verstärken

**Schlüsselzitat:**
> "When buyers cannot observe quality before purchase, sellers of low-quality goods have an incentive to pass them off as average-quality goods."

**Was bleibt offen:**
- Kann KI die Information Asymmetry wirklich signifikant reduzieren oder nur partiell?
- Gibt es neue Formen von Information Asymmetry, die durch KI entstehen (z.B. Black-Box-Opazität)?

---

#### Myers & Majluf (1984): Corporate Financing and Investment Decisions When Firms Have Information That Investors Do Not Have

**Quellentyp:** Klassisches Theorem / Peer-reviewed Theorie

**Abschnitt:** 2.1 (Informationsasymmetrie in Finanzierungsentscheidungen)

**Was steht in der Quelle:**  
Myers & Majluf zeigen, wie Manager's private Information über Firmenwert Finanzierungs- und Investitionsentscheidungen prägt. Unter asymmetrischer Information signalisiert Equity-Ausgabe, dass das Management die Aktie für überbewertet hält. Firmen bevorzugen intern generierte Mittel, dann Fremdkapital, sind Equity-Emission unwillig. **Pecking Order Theory.** Relevant für M&A: Käufer können nicht wissen, ob ein Seller die IA nutzt, um zu überverkaufen.

**Was wir rausnehmen:**  
- **Signaling Problem:** Financing-Entscheidungen sind informativ für Außenstehende
- **Pecking Order:** Interne Mittel > Fremdkapital > Equity (relevant für Deal Structure)
- **KI-Anwendung:** Wenn KI die IA reduziert, sinken Signaling-Verzerrungen

**Schlüsselzitat:**
> "Firms may reject positive-NPV investment opportunities if financing them through undervalued equity would harm existing shareholders."

**Was bleibt offen:**
- Helfen KI-Tools dem Käufer, die echte Motivation des Sellers zu erkennen?

---

#### Bergh et al. (2019): Information Asymmetry in Management Research: Past Accomplishments and Future Opportunities

**Quellentyp:** Peer-reviewed Theorie (Systematic Review)

**Abschnitt:** 2.1 (Definitorische Grundlagen: IA-Konzeptualisierungen)

**Was steht in der Quelle:**  
Umfassende Literatur-Review über 223 Management-Articles, die zeigen, wie Information Asymmetry in 5 Konzeptualisierungen verwendet wird: (1) private Information, (2) different Information, (3) hidden Information (adverse selection/moral hazard), (4) lack of perfect information, (5) information impactedness. Organisiert um 3 Antecedent-Bedingungen, 4 theoretische Rollen, 5 Reduktionsmechanismen (gathering/disclosure, precommitment, monitoring, signaling, intermediaries). Anteil der Theorien: Agency (36%), Transaction Cost (14%), Signaling (11%), Resource-Based (9%).

**Was wir rausnehmen:**  
- **5 IA-Konzeptualisierungen:** Verstehen, welche Version in einem M&A-Kontext relevant ist
- **Reduktionsmechanismen:** Due Diligence = Gathering/Disclosure; Earnouts = Precommitment; AI-Tools = strukturelle Mechanismen
- **Antecedent Conditions:** (1) Unobservable Qualities (klassisch M&A-Problem), (2) Structural Barriers (Information Flow), (3) Strategic Barriers (Disclosure-Zurückhaltung)
- **Implikation:** AI kann besonders Antecedent (1) adressieren: Qualitäten sichtbar machen, die sonst unbeobachtbar wären

**Schlüsselzitat:**
> "Information asymmetry is a condition wherein one party in a relationship has more or better information than another."

**Was bleibt offen:**
- Setzt KI neue Formen von IA: z.B. "AI Opacity Information Asymmetry" (Käufer verstehen KI-Output nicht)?
- Können Seller auch KI einsetzen, um IA zu erhöhen (arms race)?

---

#### Haleblian et al. (2009): Taking Stock of What We Know About Mergers and Acquisitions

**Quellentyp:** Peer-reviewed Theorie (Review Article)

**Abschnitt:** 2.1 (M&A-Antecedents und Outcomes)

**Was steht in der Quelle:**  
Breite akademische Review, die M&A-Forschung über Disziplinen (Management, Ökonomie, Finance, Accounting, Soziologie) organisiert. Zeigt, dass frühere Finance-Studien oft neutrale oder negative Akquisiteur-Returns finden. Neuere Forschung fokussiert auf Antecedents, Moderators und Bedingungen, unter denen Akquisitionen dem Käufer zugute kommen.

**Was wir rausnehmen:**  
- **Performance-Puzzle:** Akquisitionen erzielen nicht konsistent positive Returns für Käufer (motiviert Frage nach Moderators)
- **Disziplinäre Integration:** M&A-Theorie bleibt fragmentiert
- **Moderators:** Success hängt von Antecedents und Bedingungen ab (KI könnte Moderator sein)

**Schlüsselzitat:**
> "Acquisition research shows practical importance but lacks sufficient theoretical integration across disciplines."

**Was bleibt offen:**
- Ist KI ein Moderator, der unter bestimmten Bedingungen M&A-Success erhöht?

---

### 2.2 Grundlagen der KI: Einordnung relevanter Verfahren

#### Zhao et al. (2023): A Survey of Large Language Models

**Quellentyp:** Peer-reviewed Theorie (arXiv Survey, ~15.000+ citations)

**Abschnitt:** 2.2 (KI-Grundlagen: LLM-Taxonomie und Capabilities)

**Was steht in der Quelle:**  
Umfassendes ~100-Seiten-Survey über LLMs: 4-Generationen-Taxonomie (Statistical LM → Neural LM → Pre-trained LM → LLM), Pre-Training, Adaptation Tuning (Instruction Tuning, RLHF), Prompting-Strategien, Capability Evaluation. Zentral: **Emergent Abilities** (fähigkeiten, die bei kleinen Modellen nicht vorhanden sind, bei größeren Models plötzlich entstehen), In-Context Learning, Instruction Following, Chain-of-Thought. Scaling Laws: KM Law (Kaplan et al. 2020) und Chinchilla Law (Hoffmann et al. 2022).

**Was wir rausnehmen:**  
- **LLM-Definition:** Transformers mit sehr großen Parametern (tens to hundreds of billions)
- **4-Generationen-Progression:** Statistical → Neural → Pre-trained → Large Language Models (expansion of task-solving capacity)
- **Emergent Abilities:** Explain why GPT-4 (aber nicht GPT-2) kann few-shot M&A-DD-Klassifikation (Jang & Stikkel 2024)
- **Prompting-Strategien:** Zero-shot, Few-shot In-Context Learning, Chain-of-Thought (operativ relevant für M&A-Prompt-Design)
- **Scaling:** Training-Compute trade-offs; Larger ≠ always better if not optimally trained
- **Hallucinations:** GPT-4 and ChatGPT are prone to hallucinations — relevant for XAI-Governance

**Schlüsselzitat:**
> "In the literature, emergent abilities of LLMs are formally defined as 'the abilities that are not present in small models but arise in large models', which is one of the most prominent features that distinguish LLMs from previous PLMs."

**Was bleibt offen:**
- Wie skalieren diese Capabilities auf M&A-spezifische Aufgaben?
- Können wir emergent abilities in M&A-Kontext zuverlässig prognostizieren?

---

#### Arrieta et al. (2020): Explainable Artificial Intelligence (XAI): Concepts, taxonomies, opportunities and challenges toward Responsible AI

**Quellentyp:** Peer-reviewed Theorie (Survey, 6000+ citations)

**Abschnitt:** 2.2 (KI-Grundlagen: XAI und Governance) — auch Abschnitt 4

**Was steht in der Quelle:**  
Meistzitierteste XAI-Survey. Unterscheidet **Interpretability** (passive: Modell ergibt für Menschen Sinn) von **Explainability** (aktiv: deliberate Verfahren zur Klärung). 2 Hauptfamilien: (1) transparent models (interpretable by design: Linear Regression, Decision Trees, Rules, GAMs, Bayes), (2) post-hoc explainability (LIME, SHAP, Attention, Saliency Maps, Layer-wise Relevance Propagation). Zentral: **Responsible AI** benötigt Fairness + Explainability + Accountability gleichzeitig. Finance als High-Stakes-Domäne genannt (neben Medicine, Law).

**Was wir rausnehmen:**  
- **Definitionen:** Interpretability vs. Explainability (wichtig für Klarheit)
- **2 XAI-Familien:** Transparent vs. Post-Hoc (trade-off zwischen Performance und Erklärbarkeit)
- **Responsible AI:** Framework mit 7 Prinzipien (Fairness, Explainability, Accountability, Transparency, Privacy, Ethics, Security)
- **Finance ist High-Stakes-Domain:** Explainability ist nicht optional sondern erforderlich
- **Zielgruppen von XAI:** Domain experts, Affected Users, Regulators, Data Scientists, Managers (different needs)
- **Performance-Interpretability Trade-off:** Deep Networks sind powerful aber opaque

**Schlüsselzitat:**
> "The danger is on creating and using decisions that are not justifiable, legitimate, or that simply do not allow obtaining detailed explanations of their behaviour."

**Was bleibt offen:**
- Welche XAI-Methoden sind praktisch für M&A-ML-Modelle (z.B. LightGBM aus Zhang et al. 2024)?
- Reicht Explainability aus, um Legal/Governance Anforderungen zu erfüllen?

---

## 3. KI im M&A-Prozess (~15–17 Seiten)

### 3.1 KI in der Target-Identifikation und Deal-Sourcing

#### Zhang et al. (2024): AI-Driven M&A Target Selection and Synergy Prediction: A Machine Learning-Based Approach

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.1 (KI in Target-Auswahl) — auch 3.3 Synergy Prediction

**Was steht in der Quelle:**  
Hybrides Machine Learning-Modell (LightGBM + SVM + MLP) trainiert auf 10.000 M&A-Deals, erreicht AUC-ROC 0.937 und AUC-PR 0.912 zur Vorhersage von Synergieerfolgung. Outperformt signifikant traditionelle Methoden (DCF, Comparable Company Analysis, Expert Judgment mit ~0.75 Accuracy). Feature Importance: Revenue Growth Rate (0.182), Market Cap/EBITDA (0.159), Debt-to-Equity (0.143). NLP-Features (TF-IDF aus Company-Descriptions und Press Releases) integriert. Case Studies zeigen Model-Synergy-Schätzungen näher an realisierten Synergien als Expert-Estimates. Claim: 47% höhere PMI-Success-Rate vs. traditionelle Screening-Methoden.

**Was wir rausnehmen:**  
- **Performance-Benchmark:** AUC-ROC 0.937 vs. Accuracy Expert Judgment 0.754 (signifikante Überlegenheit)
- **Feature Ranking:** Revenue Growth > Valuation > Leverage (nicht nur offensichtliche Faktoren)
- **Untergewertete Faktoren in klassischer Analysis:** R&D Intensity, Industry Concentration
- **Hybrid Architecture:** Ensemble (LightGBM + SVM + MLP) outperforms single models
- **Text Features:** NLP auf Firm Descriptions hilft, qualitative Kompatibilität zu erfassen
- **Practical Output:** Synergy Prediction Score (SPS) für Ranking von Candidates
- **Limitationen:** Abhängig von CrunchBase-Datenqualität, kann kulturelle Passung nur begrenzt erfassen, Low Explainability

**Schlüsselzitat:**
> "The model's explainability is acknowledged as a current limitation: feature importance provides partial transparency but stakeholders require clearer justification for target selection decisions."

**Was bleibt offen:**
- Wie misst man die "47% PMI Success Rate"? (Methodologische Definition fehlend)
- Funktioniert das Modell auch bei Private Targets oder nur bei CrunchBase-Unternehmen?
- Wie verhält sich das Modell bei Cross-Border / Cross-Industry Deals?

---

#### Bozman et al. (2026): Better Than a Coin Flip? Screening Mergers and Acquisitions With Artificial Intelligence Models

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.1 (KI in Deal-Screening) — auch 3.3 Overpayment Prevention

**Was steht in der Quelle:**  
Erste Out-of-Sample Empirical Test, ob ML und LLMs die Akquisiteur-Returns bei M&A-Announcements verbessern. Testet auf 615 Deals (Oktober 2021 — Dezember 2024, nach GPT-4's Knowledge Cutoff). **Hauptfinding:** ML-Modelle verbesserng statistisch signifikant die Mean Returns (0.39% unconditional → 1.05% für positive Predictions). LLMs (Baseline) können das nicht (0.28% for positive predictions, nicht signifikant). **Fine-tuning GPT-4o** auf 500 recent deals verbessert LLMs zu 3.00% mean returns (61.7% directional accuracy). **Moderatoren:** AI-Screening ist effektiver für schwach-governanced Firmen (staggered boards) und weniger effektiv für komplexe Deals (cross-industry). **Methodological Strength:** Out-of-Sample Period beginnt nach GPT-4 Knowledge Cutoff (Sept 30, 2021), **ruled out memorization problem**.

**Was wir rausnehmen:**  
- **Performance-Benchmark:** ML signifikant > Baseline LLMs in out-of-sample setting
- **Out-of-Sample Design:** Methodologisch stärker als Degen et al. (2024) weil Post-Cutoff
- **Governance-Channel:** AI useful für hubris/empire-building-Reduktion (schwache Boards profitieren mehr)
- **Complexity-Channel:** Cross-industry deals difficult for AI (task complexity matters)
- **Fine-Tuning Works:** Domain-adapted GPT-4o reaches ~3% mean returns
- **Feature Importance:** Public Target Status, Relative Size, Acquirer Total Assets (interaction terms dominant)
- **Overpayment Detection:** LLMs sehr sensibel auf Preis-Variation (25.22% fewer positive predictions bei 10x price increase)

**Schlüsselzitat:**
> "Screening deals with AI models is more effective for firms with weaker governance, suggesting the potential to counteract managerial biases, and is less effective for complex deals."

**Was bleibt offen:**
- Wie robust ist die Governance-Moderation über verschiedene Governance-Regimes (US/EU/andere)?
- Gibt es Kalender-Effekte oder andere Marktanomalien, die das Out-of-Sample-Signal treiben?
- Wie generalisiert sich das Modell auf Private-Target Deals?

---

#### Degen et al. (2024): Large Language Models and M&A: Can ChatGPT help forecast M&A activity?

**Quellentyp:** Pflichtlektüre / Working Paper (not peer-reviewed, aber hochrelevant)

**Abschnitt:** 3.1 (KI in M&A-Sentiment-Analyse und Prognostik)

**Was steht in der Quelle:**  
Konstruiert M&A Sentiment Score (MASS) durch GPT-4.0-Analyse von Earnings Call Transcripts (S&P Global 1200, 2013–2023, 40.776 Transcripts). MASS predicts aggregate M&A deal volume mit 18-Monats-Lag. In-sample R² adjusted 9.1%, out-of-sample R² 9.4%. Outperforms Baker-Wurgler (4.4%), Huang et al. (-6.5%), UM CSI (3.2%), aber nicht OECD BCI (49.1% — combined MASS+OECD reaches 50.5%). GPT-4.0 hat höchste Korrelation mit Human M&A Expert Consensus Panel. **Critical Limitation: Memorization Problem** — Lopez-Lira et al. (2025) zeigen, dass alle Befunde im Pre-Cutoff-Zeitraum (2013–2023) sind und GPT-4o memorized realized M&A outcomes near-perfectly, making genuine forecasting vs. memorization non-identified.

**Was wir rausnehmen:**  
- **Innovation:** LLM-basierte M&A-Sentiment-Messung aus privaten Manager-Informationen (Earnings Calls)
- **18-Monats-Lag:** Plausibel für Deal Timeline (Target Search + Due Diligence + Closing)
- **Incremental Predictive Power:** MASS adds signal beyond standard sentiment/fundamentals
- **Validation:** GPT-4.0 closest to Human Expert Consensus (over Claude, GPT-4o, Perplexity, Gemini)
- **ABER: MEMORIZATION PROBLEM** — out-of-sample R² 9.4% könnte bloß Memorization sein, nicht genuine forecasting
- **Implication:** Study cannot be cited for "LLMs extract private information" without caveating memorization critique

**Schlüsselzitat:**
> [From Lopez-Lira et al. critical commentary:] "Degen et al. (2024) is a study warranting caution. Their sample (2013–2023) is entirely within GPT-4o's training period, making genuine forecasting ability non-identified from memorization."

**Was bleibt offen:**
- Kann der MASS-Ansatz auf Post-Cutoff-Daten validiert werden? (Replication erforderlich)
- Sind die 18-Monats-Lag-Befunde robust gegen Alternative Lags / andere Macroeconomic Drives?

---

### 3.2 KI in der Due Diligence

#### Jang & Stikkel (2024): Leveraging Natural Language Processing and Large Language Models for Assisting Due Diligence in the Legal Domain

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.2 (KI in Due Diligence — Legal DD mit NLP/LLMs)

**Was steht in der Quelle:**  
Erste Studie zum Einsatz von Pre-Trained Language Models (PLMs) und LLMs speziell für M&A Legal Due Diligence. Problem: KIRA Dataset hat ~3.308 Sätze pro Dokument, aber nur 4.8 relevant (extreme Imbalance >99.8% non-relevant). Tested 3 Architekturen: Single-Sentence, Context-Aware, Hierarchical Sentence Extraction. **Winner: Hierarchical Bi-LSTM** erreicht höhere Recall gegen KIRA-Baseline. GPT-4 im Few-Shot-Setting erreicht F1 0.81–0.82 (recall 0.93–0.96, precision 0.70–0.72) vs. KIRA-Baseline F1 0.78. Proposed: Combined Pipeline (LLM for High-Recall Screening + High-Precision Model for Exact Selection) as practical DD architecture.

**Was wir rausnehmen:**  
- **Extreme Class Imbalance:** DD ist ein "Needle in Haystack" Task (relevante Klauseln sind selten)
- **Architecture Matters:** Hierarchical approach > Single-Sentence BERT (sequential structure important)
- **LegalBERT ≠ BERT:** Legal domain-specific pre-training doesn't guarantee improvement (surprising finding)
- **GPT-4 Practical Utility:** High Recall, serviceable Precision — acts as Lawyer Assistant (not Replacement)
- **Prompt-Sensitivity:** Topic Descriptions critical; Example Set less important
- **Practical Design:** Combined pipeline leverages LLM high-recall with discriminative high-precision

**Schlüsselzitat:**
> "To our knowledge, this is the first study that employs pre-trained language models (PLMs) and LLMs for the due diligence problem."

**Was bleibt offen:**
- Generalisierung zu full KIRA (only 5 of 50 topics tested)?
- Performance on non-English Legal Frameworks (all KIRA is US credit agreements)?
- Can fine-tuned/domain-adapted LLMs further improve?

---

#### Dwivedi & Kamps (2025): Effectiveness of In-Context Learning for Due Diligence

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.2 (KI in Legal DD — Reproducibility and Scaling)

**Was steht in der Quelle:**  
Reproducibility study: erfolgreich repliziert Roegiest et al. (2018) CRF baseline auf KIRA. Zeigt dann, dass Few-Shot LLMs (Title + Description + Examples Prompt) competitive recall erreichen **ohne labeled training data**. Across all 50 KIRA topics: Dolphin-Llama3 recall 0.926, Gemma2 0.873, Llama3.1 0.818, GPT-4o-mini 0.663. Open-source models outperform or match GPT-4o-mini on recall. Praktische Implikation: LLM-basierter Ansatz allows rapid adaptation zu neuen DD-Topics/Jurisdictions (prompt rewrite vs. corpus annotation).

**Was wir rausnehmen:**  
- **Reproducibility:** Confirmed CRF baseline robustness (cross-framework)
- **Open-Source Competitive:** Smaller models (Llama, Gemma) reach ~0.8–0.9 recall (keine GPT-4 Abhängigkeit)
- **Prompt Design Critical:** Topic descriptions >> Example Selection
- **High-Recall Focus:** Correct for legal DD (missing key clause = huge financial risk)
- **Cost Implication:** Open-source models reduce AI DD costs vs. API-based
- **Generalization Gap:** All KIRA is English/US; language/jurisdiction generalization open

**Schlüsselzitat:**
> "It is an attractive idea to closely couple the instructions of the human legal professional and the technology-assisted review models used by them, using identical instructions. Compared to annotating extensive corpora, the efforts involved in drafting precise instructions are minimal."

**Was bleibt offen:**
- How to transition from sentence-level to paragraph-level output (cleaned documents)?
- Performance on non-credit-agreement legal documents (M&A-specific agreements)?

---

#### Wang et al. (2023): MAUD: An Expert-Annotated Legal NLP Dataset for Merger Agreement Understanding

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.2 (KI in Merger Agreement Understanding)

**Was steht in der Quelle:**  
EMNLP 2023 paper introducing MAUD: 39.000+ examples, 47.457 expert annotations from 152 English-language public merger agreements. Task: Given deal-point question + relevant contract excerpt, predict standardized answer labels. Annotation training rigorous (law students trained, experienced lawyers reviewed). LegalBERT best reaches 76.1% micro-F1, 59.7% macro-F1. Hard categories: Conditions to Closing, Deal Protection, Material Adverse Effect clauses. Long legal text remains structural challenge (token length limits).

**Was wir rausnehmen:**  
- **Task-Specific Benchmark:** Merger agreement review as reading comprehension (not just clause detection)
- **Annotation Quality:** Rigorous training + lawyer review (high ground truth)
- **Performance Gap:** 76% micro-F1 shows AI helps but not autonomous (complexity remains)
- **Hard Categories:** Complex deal concepts (MAC, Deal Protection) remain difficult
- **Data Bottleneck:** Expert annotation is expensive (cost as barrier to progress)

**Schlüsselzitat:**
> "The dataset converts merger agreement review into a reading-comprehension task..."

**Was bleibt offen:**
- How do MAUD-trained models generalize to non-public (private deal) agreements?
- What specific deal-point categories does current AI handle reliably?

---

#### Hendrycks et al. (2021): CUAD: An Expert-Annotated NLP Dataset for Legal Contract Review

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.2 (KI in Legal Contract Review — Non-M&A Baseline)

**Was steht in der Quelle:**  
NeurIPS 2021 Datasets & Benchmarks paper. CUAD: 500+ contracts, 13.000+ expert annotations, 41 label categories. Task is to highlight contract portions important for human review (obligations, red-flag clauses). 25 contract types covered. Contract review is "needle in haystack" task (important clauses sparse). DeBERTa reaches 44% Precision @ 80% Recall vs. BERT 8.2%. Annotation cost ~$2 million — illustrates data bottleneck. Training data volume critical for performance.

**Was wir rausnehmen:**  
- **Broader Legal Benchmark:** CUAD not M&A-specific but shows general contract-review challenges
- **Annotation Value:** $2M cost illustrates why expert-labeled legal data is scarce
- **Performance Gap:** 44% P@80R still far from autonomous (requires human review)
- **Data Bottleneck:** Reducing training data by order of magnitude sharply hurts performance
- **M&A Implication:** Similar challenges for M&A-specific legal DD

**Schlüsselzitat:**
> "Contract review is expensive and specialised; many law firms spend approximately 50% of their time reviewing contracts."

**Was bleibt offen:**
- Does CUAD performance translate to M&A-specific contracts (vs. generic commercial)?

---

#### Herbosch & Mertens (2025): The Future of Mergers & Acquisitions? Risk Allocation in AI-Guided Transactions

**Quellentyp:** Working Paper / Peer-reviewed Theorie

**Abschnitt:** 3.2 (KI in Due Diligence — Rechtliche Implikationen) — auch Abschnitt 4

**Was steht in der Quelle:**  
Legal-Academic Comparative Analysis (German, French, English, Belgian, Delaware Law) on liability regimes when AI tools make errors in M&A DD. Central argument: AI systems are inherently imperfect; erroneous output shifts responsibility to humans who selected, trained, deployed the tool (selection choices + supervision practice = legal nexus). Applies existing doctrines (duty of care, mistake doctrine, fiduciary duties, business judgment rule) to AI-guided M&A. **Key Legal Safeguards:** (1) reasonable tool selection, (2) adequate testing, (3) ongoing supervision, (4) meaningful human review, (5) **explainability as critical** (opaque AI = gross negligence risk in Delaware, violation of "Ision-doctrine" in Germany). **Risk Allocation:** Residual risk falls on acquiring shareholders (limited ex-ante tools to limit exposure).

**Was wir rausnehmen:**  
- **Liability Framework:** Tool Provider, Service Provider (Law Firm), Board, Shareholders (each has obligations)
- **Selection & Supervision:** Key legal questions (not whether AI was correct)
- **Explainability as Safeguard:** Unexplainable AI for significant M&A decisions = legal risk
- **Mistake Doctrine:** AI output can undermine contract validity if material error, but practicality limited (reps & warranties shift risk)
- **Business Judgment Rule Asymmetry:** Delaware (deferential) vs. Germany (strict) to boards
- **97% of M&A Pros use AI for DD:** Current adoption (Deloitte 2025), rising from 69% in 2022

**Schlüsselzitat:**
> "AI systems play an increasingly important role in facilitating all aspects of M&A transactions, particularly in the due diligence analysis that precedes such transactions. With that potential come significant risks. The inherently imperfect nature and distinct 'decision-making' of AI systems mean some outputs will be manifestly incorrect and conceptually inexplicable, potentially leading to undesirable transactions."

**Was bleibt offen:**
- Has any M&A transaction actually been challenged on AI-output errors? (Theory, no empirical cases yet)
- How to operationalize "meaningful human review" in high-volume DD?

---

### 3.3 KI in Bewertung und Synergiesch Schätzung

#### [Zhang et al. 2024 — see section 3.1 for full entry; also relevant here]

#### Zhang et al. (2025) — see section 2.1 for full entry; also relevant for synergy mechanism

---

### 3.4 KI in der Post-Merger-Integration

#### Brede et al. (2025): Mind the gap: the effect of cultural distance on mergers and acquisitions — evidence from Glassdoor reviews

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.4 (KI in Post-Merger-Integration — Kulturelle Distanz-Messung)

**Was steht in der Quelle:**  
Uses Culture-BERT (RoBERTa-based LLM fine-tuned on 2000 Glassdoor reviews) applied to ~400.000 Glassdoor employee reviews to measure organizational cultural distance for 243 M&A deals (2008–2021). **Key Findings:** Cultural distance negatively affects acquirer CARs at announcement and post-deal synergy realization (sales growth 2 and 4 years post-deal). **Cultural friction dominates cultural learning:** higher distance predicts lower performance, higher acquisition premiums (systematic overpayment), reduced post-deal innovativeness (patents, NPD). **Market culture differences** are strongest predictor (vs. other CVF dimensions: Clan, Adhocracy, Hierarchy). **First application:** Transformer-based NLP on large Glassdoor corpus to M&A cultural distance + premium effects simultaneously.

**Was wir rausnehmen:**  
- **Novel AI Operationalization:** Culture-BERT enables large-scale measurement of organizational culture (previously only via surveys, limited samples)
- **Empirical Evidence:** Cultural distance matters for M&A outcomes (not just anecdotal)
- **Mechanism:** Market culture differences are most impactful (observable to investors = drives CARs)
- **Integration Implication:** High cultural distance predicts lower synergy realization (supports DD-for-Cultural-Fit)
- **28% Accuracy Improvement:** Culture-BERT 28% more accurate than previous word2vec/survey approaches
- **Limitations:** English-language reviews only, English-speaking markets (US, Canada, Australia, UK)

**Schlüsselzitat:**
> "Using a state-of-the-art large language model, we construct a novel measure of organizational cultural distance based on employee reviews from Glassdoor.com covering 243 M&A deals from 2008 to 2021."

**Was bleibt offen:**
- Can Culture-BERT be adapted to non-English-language reviews?
- How early in DD process can cultural distance signals be used predictively?
- Does knowing cultural distance ex-ante allow targets better integration planning?

---

#### Graebner et al. (2017): The Process of Post-Merger Integration: A Review and Agenda for Future Research

**Quellentyp:** Peer-reviewed Theorie (Review)

**Abschnitt:** 3.4 (PMI als Kontext für KI-Anwendungen)

**Was steht in der Quelle:**  
Systematic Review der fragmentierten PMI-Literatur, organiziert um 3 Dimensionen: Strategic Integration, Sociocultural Integration, Experience & Learning. **Core Argument:** PMI ist nicht nur eine Information-Processing-Aufgabe, sondern ein sozialer Prozess mit zeitlichen Dynamiken, emotionalen Reaktionen, Entscheidungen, Praktiken. Calls for more **processual research** auf Temporalität, Decision-Making, Tools/Practices, Emotionality.

**Was wir rausnehmen:**  
- **PMI ≠ Information Processing:** AI can assist mit Information, aber nicht mit sozialer Integration
- **Three Integration Streams:** Strategic (systems, processes), Sociocultural (people, culture), Learning (experience transfer)
- **Temporal Dynamics:** Integration unfolds non-linearly; early wins/losses matter
- **Implication für KI:** AI likely helpful for Strategic Integration (process coordination), less useful for Sociocultural (culture-building is human work)

**Schlüsselzitat:**
> "PMI research should attend to strategic integration, sociocultural integration, and acquisition experience/learning."

**Was bleibt offen:**
- What specific PMI processes could AI optimize (Project management? Synergy tracking)?
- How to measure cultural integration progress?

---

#### Li et al. (2021): Measuring Corporate Culture Using Machine Learning

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 3.4 (Kulturmessung mittels ML — Methodologische Foundation)

**Was steht in der Quelle:**  
Uses word embeddings on 209.480 Earnings Call Transcripts (62.664 firm-year observations, 2001–2018) to measure corporate culture at scale. Scores 5 cultural values: Innovation, Integrity, Quality, Respect, Teamwork. Finds culture correlates with operational efficiency, risk-taking, earnings management, compensation design, firm value, and **deal making**. Provides methodological foundation for ML-based culture measurement (broader than Brede et al.'s M&A-specific application).

**Was wir rausnehmen:**  
- **Methodological Grounding:** ML can operationalize nebulous constructs (culture) at scale
- **Deal-Making Connection:** Culture explicitly associated with M&A activity
- **Limitations:** Earnings calls reflect **management-facing culture** (not employee-lived culture); different from Glassdoor-based Culture-BERT which uses employee voice

**Schlüsselzitat:**
> "Machine learning can operationalize otherwise nebulous corporate-culture constructs at scale using text data."

**Was bleibt offen:**
- How do earnings-call-derived and employee-review-derived culture measures correlate?

---

## 4. Kritische Reflexion (~3–4 Seiten)

### Lopez-Lira et al. (2025): The Memorization Problem: Can We Trust LLMs' Economic Forecasts?

**Quellentyp:** Peer-reviewed Theorie / Empirical Critique (arXiv, working paper)

**Abschnitt:** 4 (Black-Box Problem, Memorization Problem, Validity of LLM Forecasts)

**Was steht in der Quelle:**  
**Fundamental critique:** LLM-based economic forecasting on pre-training-cutoff data is **non-identified** — genuine forecasting skill and memorization are observationally equivalent. GPT-4o recalls S&P 500 daily closing values (MAPE 0.61%), unemployment rates (MAE 0.03 pp), GDP growth (threshold accuracy 96.27%) for pre-cutoff periods. Post-cutoff accuracy collapses to near-random (29–53%). **Key implication for Degen et al. (2024) study:** MASS (2013–2023) is entirely within GPT-4o's training period. The measured predictive power may reflect **memorization of realized M&A outcomes**, not genuine extraction of managerial private information. **Masking fails:** GPT-4o identifies companies in anonymized earnings transcripts with 100% (AAPL, META, MSFT) or 91.89% (Alphabet) accuracy. **Prompt constraints fail:** Asking to "ignore post-2010 data" yields 97.6% vs. 98.0% accuracy (no difference) — genuine post-cutoff accuracy is 40%.

**Was wir rausnehmen:**  
- **Non-Identification Problem:** Observationally equivalent hypotheses (skill vs. memorization) cannot be separated from pre-cutoff data alone
- **Empirical Evidence of Memorization:** GPT-4o near-perfect recall of public macroeconomic data
- **Robustness to Masking:** Entity neutering doesn't work; models reconstruct from context
- **Prompt Constraints Ineffective:** Instructions to ignore future data don't constrain models from using training knowledge
- **Reliable Method:** Only post-cutoff testing (after model's knowledge cutoff) rules out memorization
- **M&A-Specific Application:** Degen et al. MASS study warranting caution; empirical findings non-identified

**Schlüsselzitat:**
> "LLMs cannot be trusted for economic forecasts during periods covered by their training data. Counterfactual forecasting ability is non-identified when the model has seen the realized values: any observed output is consistent with both genuine skill and memorization."

**Was bleibt offen:**
- Can any pre-cutoff LLM forecast be trusted, or only those with external validation?
- What about newer models with extended context windows / updated training?

---

### Herbosch & Mertens (2025) — [see section 3.2 for full entry; also critical for Abschnitt 4]

---

### Arrieta et al. (2020) — [see section 2.2 for full entry; core XAI framework for Abschnitt 4]

---

### Johnson, Pasquale & Chapman (2019): Artificial Intelligence, Machine Learning, and Bias in Finance: Toward Responsible Innovation

**Quellentyp:** Peer-reviewed Theorie (Legal Academic Essay)

**Abschnitt:** 4 (Algorithmic Bias, Governance, Regulatory Responses)

**Was steht in der Quelle:**  
Legal-policy essay arguing that algorithmic bias in fintech credit markets is **structurally produced** by biased training data, flawed feature selection, and proxy variables — not by developer negligence alone. OCC's 2018 Fintech Charter Decision preempts state consumer-protection laws, removing safeguards for low-income/minority borrowers. **Core argument:** Explainability is not merely a technical preference but a **regulatory necessity** — without algorithmic transparency, existing federal discrimination laws (ECOA, Fair Housing Act) cannot practically be enforced. Proposes coordinated state-federal oversight establishing uniform consumer-protection floor.

**Was wir rausnehmen:**  
- **Bias as Structural:** Moves from human judgment to training data, feature selection, proxy variables
- **Proxy Variables:** Alternative data (social media, shopping, browsing) encode socioeconomic proxies for race/gender
- **Regulatory Gap:** OCC preemption removes state-level safeguards
- **XAI as Regulatory Tool:** Explainability enables ECOA/Fair Housing Act enforcement
- **M&A Implication:** If AI-driven M&A targets systematically exclude certain firm types, disparate impact liability may arise

**Schlüsselzitat:**
> "ADM may only shift the locus of discrimination from the bank manager's desk to the programmer's computer screen or to the data scientists' training sets since data are never brute or raw — they are always collected, analyzed, and used by people, who may have the same conscious calculations, barely conscious emotions, or unconscious biases at play in their own observations."

**Was bleibt offen:**
- Do M&A AI tools systematically exclude/disadvantage certain firm types (women-owned, minority-owned)?
- How to audit M&A AI models for proxy discrimination?

---

### Sele & Chugunova (2024): Human-in-the-Loop Algorithmic Decision Making

**Quellentyp:** Peer-reviewed Theorie

**Abschnitt:** 4 (Human-AI Collaboration, Governance of AI-Driven Decisions)

**Was steht in der Quelle:**  
[Placeholder — specific content not fully extracted from wiki source, but relevant for HITL governance frame]

---

### Logg, Minson & Moore (2019): Algorithm Appreciation: People Prefer Algorithmic to Human Judgment

**Quellentyp:** Peer-reviewed Empirie

**Abschnitt:** 4 (Human Over-Reliance on Algorithms vs. Under-Reliance)

**Was steht in der Quelle:**  
Experimental study across 6 experiments showing lay participants display robust **algorithm appreciation:** they adhere more to identical advice when told it's from an algorithm vs. human. BUT experienced professionals (national-security forecasters) show **inverse pattern** — discount algorithmic advice heavily, rely on own judgment, achieve **lower accuracy** as a result. **Key moderator:** Domain expertise. DD professionals are "expert" archetype (not lay) — likely to **under-weight** AI DD outputs, opposite of automation bias.

**Was wir rausnehmen:**  
- **Dual Pattern:** Lay people over-weight algorithms; Experts under-weight them
- **Accuracy Cost:** Expert under-reliance on algorithms reduces forecast accuracy
- **M&A Implication:** DD professionals may dismiss valuable AI signals (governance risk is not over-reliance but under-reliance)
- **Theory of Machine:** How people represent algorithm internals/processes (opacity increases skepticism for experts)

**Schlüsselzitat:**
> "Paradoxically, experienced professionals, who make forecasts on a regular basis, relied less on algorithmic advice than lay people, which hurt their accuracy."

**Was bleibt offen:**
- How to calibrate expert confidence in AI DD outputs?
- Training interventions to improve expert-AI collaboration?

---

## 5. Fazit (~2 Seiten)

[Guide section reserved for synthesis; content to be drawn from above sources in paper-writing phase]

---

## Quellen-Übersicht nach Abschnitt

| Abschnitt | Quelle | Typ | Primär | Sekundär |
|-----------|--------|-----|--------|----------|
| **1. Einleitung** | Singh (2023) | Pflichtlektüre | ✓ | 2.1, 3 |
| | Bain (2024) | Praxisbericht | ✓ | 3.1, 3.2 |
| | Bremen (2024) | Pflichtlektüre | ✓ | 2.1, 3, 4 |
| **2.1 M&A-Prozess** | Howson (2003) | Lehrbuch | ✓ | |
| | Lajoux (2024) | Lehrbuch | ✓ | |
| | Zhang et al. (2025) | Peer-reviewed | ✓ | |
| | Akerlof (1970) | Klassiker | ✓ | |
| | Myers & Majluf (1984) | Klassiker | ✓ | |
| | Bergh et al. (2019) | Peer-reviewed Review | ✓ | |
| | Haleblian et al. (2009) | Peer-reviewed Review | ✓ | |
| **2.2 KI-Grundlagen** | Zhao et al. (2023) | Peer-reviewed Survey | ✓ | |
| | Arrieta et al. (2020) | Peer-reviewed Survey | ✓ | 4 |
| **3.1 Target-ID** | Zhang et al. (2024) | Peer-reviewed | ✓ | 3.3 |
| | Bozman et al. (2026) | Peer-reviewed | ✓ | |
| | Degen et al. (2024) | Pflichtlektüre | ✓ | 4 |
| **3.2 Due Diligence** | Jang & Stikkel (2024) | Peer-reviewed | ✓ | |
| | Dwivedi & Kamps (2025) | Peer-reviewed | ✓ | |
| | Wang et al. (2023) | Peer-reviewed | ✓ | |
| | Hendrycks et al. (2021) | Peer-reviewed | ✓ | |
| | Herbosch & Mertens (2025) | Working Paper | ✓ | 4 |
| | Bhagwan et al. (2018) | Peer-reviewed Review | ✓ | |
| | Puranam et al. (2006) | Peer-reviewed | ✓ | |
| **3.3 Bewertung/Synergien** | Zhang et al. (2024) | Peer-reviewed | ✓ | 3.1 |
| | Zhang et al. (2025) | Peer-reviewed | ✓ | 2.1 |
| **3.4 PMI** | Brede et al. (2025) | Peer-reviewed | ✓ | |
| | Graebner et al. (2017) | Peer-reviewed Review | ✓ | |
| | Li et al. (2021) | Peer-reviewed | ✓ | |
| **4. Kritische Reflexion** | Lopez-Lira et al. (2025) | Peer-reviewed | ✓ | |
| | Herbosch & Mertens (2025) | Working Paper | ✓ | 3.2 |
| | Arrieta et al. (2020) | Peer-reviewed | ✓ | 2.2 |
| | Johnson et al. (2019) | Peer-reviewed | ✓ | |
| | Logg et al. (2019) | Peer-reviewed | ✓ | |

---

## Hinweise zur Verwendung dieses Guides

1. **Pflichtlektüren (4):** Singh 2023, Bremen 2024, Degen et al. 2024, Bain 2024 — sollten primär behandelt werden
2. **Kritische Validation:** Lopez-Lira et al. (2025) **kritisiert** Degen et al. (2024) — beide zusammen lesen!
3. **Querschnitt-Quellen:** Singh, Bremen treten in mehreren Abschnitten auf — ausführliche erste Einführung, dann Kurzzitate in den folgenden Kapiteln
4. **Lehrbuch-Baseline:** Howson (2003) und Lajoux (2024) sind Standardreferenzen für klassische DD — im Grundlagenteil ausführlich darstellen
5. **Empirischer Support:** Bozman et al. (2026) ist stärker als Degen et al. (2024) wegen Post-Cutoff-Design — für positive KI-Wirkungsnachweis präferieren
6. **Governance-Rahmen:** Herbosch & Mertens (2025) ist einzige Quelle zu Liability/Legal Risk — zentral für kritische Reflexion
7. **Bias & Explainability:** Arrieta (2020) + Johnson et al. (2019) kombinieren technisches (XAI) und regulatorisches (Bias) Risiko

---

**Redaktion:** Claude Sonnet 4.6  
**Datum:** Mai 2026
