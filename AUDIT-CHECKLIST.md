# Audit & Examination Readiness Checklist
## UAE AI Compliance for Banking & Fintech

> **Version: 1.1 | Last Reviewed: April 2026**
> 70 controls across 10 domains | Covers CBUAE Guidance Note (Feb 2026), CBUAE MMS Rulebook, and UAE AI Charter

**How to use this checklist:**
- **Status options:** ✅ Complete | 🟡 In Progress | ❌ Not Started | N/A Not Applicable
- **Priority:** 🔴 CRITICAL (examination finding risk if missing) | 🟠 HIGH (significant finding) | 🟡 MEDIUM (noted finding)
- Review quarterly and before any CBUAE examination
- Evidence column lists what an examiner will specifically ask to see

> **v1.1 changes:** DA2 (training data quality), DA3 (lawful basis for training data), and DA5 (cross-border transfers) reclassified from HIGH to CRITICAL. V3 (Tier 2 validation) clarified to reflect proportionate depth. Control G5 priority upgraded. Summary dashboard updated.

---

## Domain 1: Governance and Accountability (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| G1 | Board has formally approved an AI Risk Policy | Board-signed policy document; Board minutes with approval date | All three | 🔴 | |
| G2 | AI Policy explicitly references UAE AI Charter principles (all eight) | Policy document with Charter section | AI Charter | 🔴 | |
| G3 | AI/Model Governance Committee constituted with documented Terms of Reference | Signed ToR; membership list; reporting line to Board/Risk Committee | GN + MMS | 🔴 | |
| G4 | Governance Committee holds meetings at defined frequency (minimum quarterly for Tier 1 institutions) | Meeting minutes for last 12 months; attendance records | GN + MMS | 🔴 | |
| G5 | Named Responsible AI Officer (RAO) designated at Senior Management level with formal ToR and org chart positioning | Appointment letter; ToR; org chart showing reporting line and seniority | GN | 🔴 | |
| G6 | Board receives formal AI risk reporting at least annually (quarterly recommended) | Board packs; Board minutes with AI agenda item | GN + MMS | 🟠 | |
| G7 | First / Second / Third Line responsibilities for AI risk defined in RACI or equivalent | Policy / RACI matrix; job descriptions referencing AI accountability | MMS | 🟠 | |

---

## Domain 2: Model Inventory (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| I1 | Comprehensive Model Inventory exists and is actively maintained | Current inventory register with last-updated date | MMS | 🔴 | |
| I2 | Inventory scope covers all model types: statistical, ML, AI, rule-based scoring, vendor/third-party AI | Inventory scope definition; business unit attestation of completeness | MMS | 🔴 | |
| I3 | Each inventory record includes: name/ID, owner, business purpose, input data, output type, risk tier, high-impact classification, validation status, monitoring status, last review date | Inventory template; sample records showing all fields populated | MMS + GN | 🔴 | |
| I4 | Each model has a named owner at an appropriate seniority level | Inventory records with owner field populated and owner confirmed | MMS | 🟠 | |
| I5 | Each model has a formally assigned risk tier (minimum Tier 1, 2, 3) based on documented tiering methodology (5-question framework or equivalent) | Inventory with tier column; tiering methodology document; RAO approval for T1/T2 | MMS | 🔴 | |
| I6 | Inventory reflects current validation status per model (validated / overdue / exempt with documented rationale) | Inventory records; validation tracker cross-reference | MMS | 🟠 | |
| I7 | Business unit heads have provided completeness attestation for models in their area | Signed attestation records by business unit; date of last attestation | MMS | 🟠 | |

---

## Domain 3: Model Development and Documentation (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| D1 | Model Concept Document exists for each Tier 1 and Tier 2 model (retrospective reconstruction acceptable for existing models) | Concept documents per model; document register | MMS | 🔴 | |
| D2 | Model Development Document exists for each Tier 1 and Tier 2 model | Development documents per model; document register | MMS | 🔴 | |
| D3 | Training data quality assessment is documented: volume, time period, representativeness, known exclusions and their impact, known biases | Data quality section in dev docs; source data descriptions; representativeness analysis; evidence exclusions were considered | MMS + GN | 🔴 | |
| D4 | Prohibited features (protected characteristics: nationality, gender, age, religion, disability, and their proxies) formally excluded and documented with legal sign-off | Feature list with exclusions noted and approved; legal/compliance sign-off | MMS + GN + Charter | 🔴 | |
| D5 | Model selection rationale documented (why this algorithm/approach vs. alternatives considered) | Methodology selection section in dev doc with alternatives assessed | MMS | 🟠 | |
| D6 | Operational Manual exists for each Tier 1 and Tier 2 model | Operational manuals per model; document register | MMS | 🔴 | |
| D7 | Model Change Log initiated for all production models; material changes recorded since deployment | Change logs per model; entries for all known post-deployment changes; no unexplained gaps | MMS | 🟠 | |

---

## Domain 4: Independent Validation (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| V1 | Validation team/function is structurally independent from model development team (four-eyes principle) | Org chart showing structural separation; Validation ToR; no dual reporting to development lead | MMS | 🔴 | |
| V2 | All Tier 1 models have a current, full-scope Validation Report (within the defined annual review cycle) | Validation reports with dates; inventory validation status column; all required sections present | MMS | 🔴 | |
| V3 | All Tier 2 models have a current Validation Report at proportionate depth (as defined in Model Risk Policy) | Validation reports with dates; Model Risk Policy section defining T2 validation scope; scope matches policy | MMS | 🔴 | |
| V4 | Validation Reports contain a formal opinion from one of three options: Approve / Approve with Conditions / Reject | Opinion section in each validation report; not implied or informal | MMS | 🔴 | |
| V5 | Validation scope covers all required elements: conceptual soundness, data quality, statistical performance, outcome analysis, stress testing, explainability, fairness/bias | Validation methodology checklist; each element present in validation report | MMS + GN | 🔴 | |
| V6 | All validation findings tracked in a Validation Finding Tracker with owners, severity rating, and due dates | Finding tracker; evidence of management responses; no findings older than due date without documented extension | MMS | 🟠 | |
| V7 | No Tier 1 model is in production with an outstanding Critical or High severity validation finding that is unmitigated (no approved remediation plan in place) | Finding tracker with status column; deployment gate evidence; confirmation no unmitigated critical findings exist | MMS | 🔴 | |

> **Note on V3 — Tier 2 proportionate validation:** The MMS permits Tier 2 validation to be lighter-touch than Tier 1 — for example, a structured review of key risk areas rather than a full independent validation. However, "proportionate" must be defined in the Model Risk Management Policy with explicit criteria for what is included and excluded. An examiner will not accept "proportionate" as a justification without the policy definition. The validation report for Tier 2 must still reach a formal opinion.

---

## Domain 5: Model Monitoring (6 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| M1 | A monitoring plan exists for every model currently in production | Monitoring plan documents per model; document register covering all production models | MMS | 🔴 | |
| M2 | Monitoring metrics defined and include performance drift indicators (PSI, KS, Gini/AUC as appropriate to model type) | Monitoring plan metric definitions with threshold values | MMS | 🔴 | |
| M3 | Alert thresholds defined for each monitoring metric; threshold breach triggers documented escalation pathway | Monitoring plan threshold table; escalation protocol with named escalation path | MMS | 🟠 | |
| M4 | Monitoring results reported to AI Governance Committee on defined cadence (minimum quarterly for Tier 1) | Monitoring reports; Committee meeting packs; minutes confirming discussion | MMS + GN | 🔴 | |
| M5 | Monitoring breach escalation protocol documented, tested, and demonstrably followed when triggered | Protocol document; evidence of any past breaches handled per protocol; test evidence if no real breaches yet | MMS | 🟠 | |
| M6 | Fairness/bias metrics included as part of ongoing production monitoring for all Tier 1 and Tier 2 models (not only pre-deployment) | Monitoring plans with fairness metrics section; monitoring reports with fairness data; not blank | MMS + GN + Charter | 🔴 | |

---

## Domain 6: Consumer Protection and Disclosure (9 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| C1 | Customer-facing AI disclosure present in product documentation, terms and conditions, website, and/or mobile app | Document/app screenshots; legal-approved disclosure text; coverage across all relevant channels | GN + Charter | 🔴 | |
| C2 | AI chatbots and virtual assistants identify themselves as AI systems at the start of each customer session | UI screenshots; system configuration; live test evidence | GN | 🔴 | |
| C3 | Customers are proactively notified when an AI system made or materially influenced an adverse decision about them | Notification templates; process documentation; sample notifications sent to real customers | GN | 🔴 | |
| C4 | Customers can request a plain-language explanation of any AI-influenced decision — and receive one within a defined SLA | Process documentation; explanation templates per model type; SLA definition; sample explanations actually delivered | GN + Charter | 🔴 | |
| C5 | Customers can request human review of any high-impact AI decision — a formal workflow exists with defined SLA and logging | Process documentation; request channel; SLA; review outcome logging; evidence of at least one test run | GN | 🔴 | |
| C6 | Human review requests are logged with full records (request date, model involved, outcome, SLA met/missed) | Review log with complete records; periodic reporting to governance committee | GN | 🟠 | |
| C7 | AI-related complaints are captured as a distinct named category in the complaints management system (not subsumed under general complaints) | Complaints system configuration screenshot; complaints category list showing AI as named category | GN | 🔴 | |
| C8 | AI complaints data (volume, themes, outcomes, trends) reported to AI Governance Committee on regular basis | Committee meeting packs with AI complaints data section; minutes confirming discussion | GN | 🟠 | |
| C9 | A formal redress mechanism exists for customers harmed by incorrect, biased, or erroneous AI decisions — accessible, documented, and tested | Redress policy; process documentation; sample remediation records; accessibility evidence | GN | 🟠 | |

---

## Domain 7: Fairness and Bias (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| F1 | Protected characteristics defined and formally documented as prohibited model features for each model type — approved by Legal/Compliance | Feature exclusion list per model type; Legal/Compliance sign-off on record | GN + MMS + Charter | 🔴 | |
| F2 | Proxy discrimination analysis conducted: quantitative testing that variables correlated with protected characteristics do not cause indirect discrimination | Proxy analysis section in validation report; correlation matrix; results reviewed and documented | GN + MMS + Charter | 🔴 | |
| F3 | Fairness metrics formally defined per model category (demographic parity, equalised odds, predictive parity — as appropriate to model type and use case) | Fairness Testing Framework document; metric selection rationale per model type | GN + Charter | 🟠 | |
| F4 | Pre-deployment fairness testing results documented, reviewed, and approved by Governance Committee as part of deployment gate | Fairness test report; Committee approval minutes; evidence of deployment gate process | GN + MMS | 🔴 | |
| F5 | Ongoing fairness monitoring implemented for all Tier 1 and Tier 2 production models with defined metrics and thresholds | Monitoring plans with fairness metrics; monitoring reports with actual fairness data — not empty fields | GN + MMS | 🔴 | |
| F6 | Bias remediation process documented with defined SLAs for escalation to Senior Management on material findings | Process documentation; SLA definitions; escalation owner named | GN | 🟠 | |
| F7 | Evidence of Senior Management escalation and documented action on any material bias findings identified since AI deployment | Escalation records; remediation plans with named owners and closure dates; if no material findings, documented confirmation | GN | 🟠 | |

---

## Domain 8: Third-Party and Vendor AI (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| T1 | Inventory of all third-party AI systems currently deployed by the institution (distinct field or cross-reference in main Model Inventory) | Vendor AI inventory as subset of or linked to main Model Inventory | GN | 🔴 | |
| T2 | AI-specific risk assessment conducted for each live vendor AI system | Completed risk assessments per vendor AI; risk rating documented | GN | 🔴 | |
| T3 | Vendor contracts include the LFI's right to audit the vendor AI model (methodology, data used, testing results, validation) | Contract excerpts showing audit rights clause with sufficient scope | GN | 🔴 | |
| T4 | Vendor contracts require the vendor to provide explainability artifacts sufficient for CBUAE examination on request | Contract excerpts or vendor letter of undertaking with explicit explainability commitment | GN + Charter | 🔴 | |
| T5 | Vendor contracts require advance notification to LFI of material model changes (retraining, threshold changes, new features, model version changes) | Contract excerpts showing change notification clause; notice period defined (minimum 30 days recommended) | GN + MMS | 🔴 | |
| T6 | Vendor contracts include provisions allowing LFI to exit or replace AI system if governance standards are not met (termination for cause) | Contract excerpts showing exit/termination for cause clause; not only standard termination | GN | 🟠 | |
| T7 | Vendor AI systems included in Model Inventory with appropriate tier assignment and subject to monitoring requirements | Inventory records for vendor AI with tier; monitoring plan; evidence monitoring is actually running | MMS + GN | 🟠 | |

---

## Domain 9: Data Governance for AI (6 controls)

> **v1.1 update:** DA2, DA3, and DA5 reclassified to 🔴 CRITICAL based on their direct impact on validation outcomes and examination findings. See notes in each control.

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| DA1 | Training data lineage documented for each Tier 1 and Tier 2 model (source systems, transformation steps, version used in training, extraction date) | Data lineage documentation in Development Documents; traceable to source | MMS + GN | 🟠 | |
| DA2 | Training data quality assessment documented: volume, time period, representativeness of the target population, exclusions and their impact, known data biases and how they were addressed | Quality assessment in Development Documents; representativeness analysis; explicit statement of known limitations | MMS + GN | 🔴 | |
| DA3 | Lawful basis for using personal data in AI model training assessed and documented under UAE PDPL (consent, contract, legitimate interest, or legal obligation) | Privacy legal assessment or DPIA; confirmed lawful basis per model; documented before training commenced | GN + Charter | 🔴 | |
| DA4 | Data retention and deletion policies applied to AI training datasets — aligned with UAE PDPL and not retained beyond lawful purpose | Retention schedule; evidence that deletion/anonymisation has been applied to expired training data | GN + Charter | 🟠 | |
| DA5 | Cross-border data transfers in AI pipelines assessed and approved: training data to foreign cloud storage; inference data to foreign model APIs; model weights stored offshore | Transfer impact assessment per pipeline; data processing agreement or equivalent; explicit approval record | GN + Charter | 🔴 | |
| DA6 | AI data processing activities recorded in the institution's Record of Processing Activities (ROPA) under UAE PDPL | ROPA entries for each AI system processing personal data; ROPA is current and reviewed | GN + Charter | 🟠 | |

> **Note on DA2 (CRITICAL):** Training data quality directly determines the validity of the model's outputs and is a core component of independent validation. An examiner finding that no training data quality assessment exists will likely render the entire validation report suspect. This is not a back-office data management issue — it is a model governance critical control.

> **Note on DA3 (CRITICAL):** Using personal data to train AI models without a documented lawful basis is a PDPL breach with potential enforcement consequences independent of AI governance. CBUAE examiners increasingly coordinate with data protection assessments. Absence of a documented lawful basis for training data is a critical gap.

> **Note on DA5 (CRITICAL):** The majority of UAE banks and fintechs use foreign cloud providers (AWS, Azure, GCP) for model training and inference. If no cross-border transfer assessment has been conducted, the institution has an undocumented exposure under both the PDPL and CBUAE data governance expectations. This affects every cloud-based AI deployment.

---

## Domain 10: Internal Audit AI Coverage (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| IA1 | AI/Model risk explicitly included in the annual Internal Audit plan with dedicated audit assignments (not subsumed under general technology audits) | Annual Internal Audit plan; AI audit assignments with scope | All | 🟠 | |
| IA2 | Model Inventory completeness audit conducted (at least annually) | Internal Audit report on inventory; findings and management response | MMS | 🟠 | |
| IA3 | Model documentation compliance audit conducted (sample of Tier 1 and Tier 2 models — minimum 20% coverage) | Internal Audit report on documentation; sampling methodology; findings | MMS | 🟠 | |
| IA4 | Tiering consistency audit conducted — are models correctly tiered using the documented framework? | Internal Audit report on tiering decisions; any mis-tiered models identified and corrected | MMS + GN | 🟠 | |
| IA5 | Validation independence and quality audit conducted | Internal Audit report on validation function; independence confirmed | MMS | 🟠 | |
| IA6 | Consumer AI disclosure compliance audit conducted (including live channel testing) | Internal Audit report on consumer disclosures; mystery shopping / channel testing evidence | GN | 🟠 | |
| IA7 | Vendor AI contract compliance audit conducted | Internal Audit report on vendor AI contracts; gaps identified and remediated | GN | 🟠 | |

> **Note on Domain 10:** All internal audit controls remain 🟠 HIGH rather than 🔴 CRITICAL because Internal Audit coverage is a third-line assurance activity — its absence does not directly harm customers or breach the frameworks, but it does indicate the institution has no independent oversight of its own AI controls. A CBUAE examiner finding no IA coverage of AI will treat it as a significant governance weakness. Institutions with a formal D-SIB designation should consider upgrading IA1 to CRITICAL given CBUAE's heightened expectations for systemic institutions.

---

## Summary Dashboard (v1.1)

| Domain | Total Controls | 🔴 CRITICAL | 🟠 HIGH | Completed | % Done |
|--------|---------------|-------------|---------|-----------|--------|
| D1: Governance & Accountability | 7 | 5 | 2 | | |
| D2: Model Inventory | 7 | 4 | 3 | | |
| D3: Model Development & Docs | 7 | 5 | 2 | | |
| D4: Independent Validation | 7 | 6 | 1 | | |
| D5: Model Monitoring | 6 | 4 | 2 | | |
| D6: Consumer Protection & Disclosure | 9 | 7 | 2 | | |
| D7: Fairness & Bias | 7 | 4 | 3 | | |
| D8: Third-Party & Vendor AI | 7 | 5 | 2 | | |
| D9: Data Governance for AI *(updated v1.1)* | 6 | **3** | **3** | | |
| D10: Internal Audit AI Coverage | 7 | 0 | 7 | | |
| **TOTAL** | **70** | **43** | **27** | | |

> **v1.1 change to Domain 9:** DA2, DA3, DA5 upgraded from HIGH to CRITICAL. Total CRITICAL controls increased from 40 to 43.

---

## Examiner Focus Areas

Based on CBUAE examination methodology, examiners will prioritise:

1. **Model Inventory** — First document requested. Must be complete, current, attested, and include high-impact classification for each model.
2. **High-Impact AI Classification** — Examiners will specifically test whether all consumer-facing AI with significant impact has been correctly identified and classified.
3. **Tier 1 Documentation Pack** — For a sample of 3–5 high-impact models, all five documents will be requested and reviewed for substance, not just existence.
4. **Validation Reports** — Examiners will read the formal opinion, check all required sections are present, and look for outstanding critical findings.
5. **Consumer Disclosure Evidence** — Live testing of websites, apps, and chatbot interactions is likely; not just documentation review.
6. **Human Review Process** — Process documentation and the actual log of review requests and outcomes.
7. **Governance Minutes** — Board and Governance Committee minutes demonstrating AI risk is actively discussed — not just noted.
8. **Fairness Testing Evidence** — Pre-deployment results and what ongoing monitoring shows.
9. **Training Data Quality** — Specifically for Tier 1 models: was data quality formally assessed and documented?
10. **Cross-Border Data Flows** — For cloud-based AI: has the transfer been assessed and approved?

> **Preparation tip:** Prepare an Examination Pack in advance containing the 21 key artefacts listed in README.md Section 7. For each Tier 1 model, prepare a model-specific pack with all five documents plus the high-impact classification record, validation report, fairness test report, and latest monitoring report. Examiners will request these within the first day.

---

*Version 1.1 | Last updated: April 2026 | Part of the [UAE AI Compliance Guide](./README.md) | See [CHANGELOG.md](./CHANGELOG.md)*
