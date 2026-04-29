# Audit & Examination Readiness Checklist
## UAE AI Compliance for Banking & Fintech

> 70 controls across 10 domains | Covers CBUAE Guidance Note (Feb 2026), CBUAE MMS Rulebook, and UAE AI Charter

**How to use this checklist:**
- **Status options:** ✅ Complete | 🟡 In Progress | ❌ Not Started | N/A Not Applicable
- **Priority:** 🔴 CRITICAL (exam risk if missing) | 🟠 HIGH | 🟡 MEDIUM
- Review quarterly and before any CBUAE examination
- Evidence column lists what an examiner will ask to see

---

## Domain 1: Governance and Accountability (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| G1 | Board has formally approved an AI Risk Policy | Board-signed policy document; Board minutes with approval date | All three | 🔴 | |
| G2 | AI Policy explicitly references UAE AI Charter principles (all eight) | Policy document with Charter section | AI Charter | 🔴 | |
| G3 | AI/Model Governance Committee constituted with documented Terms of Reference | Signed ToR; membership list; reporting line to Board/Risk Committee | GN + MMS | 🔴 | |
| G4 | Governance Committee holds meetings at defined frequency (minimum quarterly for Tier 1 institutions) | Meeting minutes for last 12 months; attendance records | GN + MMS | 🔴 | |
| G5 | Named Responsible AI Officer (RAO) designated at Senior Management level with formal ToR | Appointment letter; ToR; org chart showing reporting line | GN | 🔴 | |
| G6 | Board receives formal AI risk reporting at least annually (quarterly recommended) | Board packs; Board minutes with AI agenda item | GN + MMS | 🟠 | |
| G7 | First / Second / Third Line responsibilities for AI risk defined in RACI or equivalent | Policy / RACI matrix; job descriptions referencing AI accountability | MMS | 🟠 | |

---

## Domain 2: Model Inventory (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| I1 | Comprehensive Model Inventory exists and is actively maintained | Current inventory register with last-updated date | MMS | 🔴 | |
| I2 | Inventory scope covers all model types: statistical, ML, AI, rule-based scoring, vendor/third-party AI | Inventory scope definition; business unit attestation of completeness | MMS | 🔴 | |
| I3 | Each inventory record includes: name/ID, owner, business purpose, input data, output type, risk tier, validation status, monitoring status, last review date | Inventory template; sample records | MMS | 🔴 | |
| I4 | Each model has a named owner at an appropriate level | Inventory records with owner field populated | MMS | 🟠 | |
| I5 | Each model has a formally assigned risk tier (minimum Tier 1, 2, 3) based on documented tiering methodology | Inventory with tier column; tiering methodology document | MMS | 🔴 | |
| I6 | Inventory reflects current validation status per model (validated / overdue / exempt with rationale) | Inventory records; validation tracker cross-reference | MMS | 🟠 | |
| I7 | Business unit heads have provided completeness attestation for models in their area | Signed attestation records by business unit | MMS | 🟠 | |

---

## Domain 3: Model Development and Documentation (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| D1 | Model Concept Document exists for each Tier 1 and Tier 2 model (retrospective is acceptable for existing models) | Concept documents per model; document register | MMS | 🔴 | |
| D2 | Model Development Document exists for each Tier 1 and Tier 2 model | Development documents per model; document register | MMS | 🔴 | |
| D3 | Training data quality assessment is documented in the Development Document | Data quality section in dev docs; source data descriptions; representativeness analysis | MMS + GN | 🔴 | |
| D4 | Prohibited features (protected characteristics: nationality, gender, age, religion, disability, and proxies) formally excluded and documented | Feature list with exclusions noted and approved; legal sign-off | MMS + GN + Charter | 🔴 | |
| D5 | Model selection rationale documented (why this algorithm/approach vs. alternatives considered) | Methodology selection section in dev doc | MMS | 🟠 | |
| D6 | Operational Manual exists for each Tier 1 and Tier 2 model | Operational manuals per model; document register | MMS | 🔴 | |
| D7 | Model Change Log initiated for all production models; changes recorded since deployment | Change logs per model; entries for all known post-deployment changes | MMS | 🟠 | |

---

## Domain 4: Independent Validation (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| V1 | Validation team/function is structurally independent from model development team (four-eyes principle) | Org chart showing separation; Validation ToR; no dual reporting to development lead | MMS | 🔴 | |
| V2 | All Tier 1 models have a current Validation Report (within the defined review cycle) | Validation reports with dates; inventory validation status column | MMS | 🔴 | |
| V3 | All Tier 2 models have a current Validation Report (within the defined review cycle) | Validation reports with dates | MMS | 🔴 | |
| V4 | Validation Reports contain a formal opinion from one of three options: Approve / Approve with Conditions / Reject | Opinion section in each validation report | MMS | 🔴 | |
| V5 | Validation scope covers all required elements: conceptual soundness, data quality, statistical performance, outcome analysis, stress testing, explainability, fairness/bias | Validation methodology checklist; validation report sections | MMS + GN | 🔴 | |
| V6 | All validation findings tracked in a Validation Finding Tracker with owners, severity, and due dates | Finding tracker; evidence of management responses | MMS | 🟠 | |
| V7 | No Tier 1 model is in production with an outstanding Critical or High severity validation finding that is unmitigated | Finding tracker with status column; deployment gate evidence | MMS | 🔴 | |

---

## Domain 5: Model Monitoring (6 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| M1 | A monitoring plan exists for every model currently in production | Monitoring plan documents per model; document register | MMS | 🔴 | |
| M2 | Monitoring metrics defined and include performance drift indicators (PSI, KS, Gini/AUC as appropriate to model type) | Monitoring plan metric definitions with thresholds | MMS | 🔴 | |
| M3 | Alert thresholds defined for each monitoring metric; breach triggers documented escalation | Monitoring plan threshold table; escalation protocol | MMS | 🟠 | |
| M4 | Monitoring results reported to AI Governance Committee on defined cadence (min. quarterly for Tier 1) | Monitoring reports; Committee meeting packs; minutes | MMS + GN | 🔴 | |
| M5 | Monitoring breach escalation protocol documented, tested, and followed when triggered | Protocol document; evidence of any breaches handled per protocol | MMS | 🟠 | |
| M6 | Fairness/bias metrics included as part of ongoing production monitoring (not just pre-deployment validation) | Monitoring plans with fairness section; monitoring reports with fairness data | MMS + GN + Charter | 🔴 | |

---

## Domain 6: Consumer Protection and Disclosure (9 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| C1 | Customer-facing AI disclosure present in product documentation, terms and conditions, website, and/or mobile app | Document/app screenshots; legal-approved disclosure text | GN + Charter | 🔴 | |
| C2 | AI chatbots and virtual assistants identify themselves as AI systems at the start of each customer session | UI screenshots; system configuration; test evidence | GN | 🔴 | |
| C3 | Customers are proactively notified when an AI system made or materially influenced an adverse decision about them | Notification templates; process documentation; sample notifications sent | GN | 🔴 | |
| C4 | Customers can request a plain-language explanation of any AI-influenced decision — and receive one within a defined SLA | Process documentation; explanation templates; SLA; sample explanations delivered | GN + Charter | 🔴 | |
| C5 | Customers can request human review of any high-impact AI decision — a formal workflow exists | Process documentation; request channel; SLA; review outcome logging | GN | 🔴 | |
| C6 | Human review requests are logged and outcomes tracked (number of requests; outcomes; customer satisfaction) | Review log with complete records; reporting to governance | GN | 🟠 | |
| C7 | AI-related complaints are captured as a distinct named category in the complaints management system | Complaints system configuration; complaints category list; complaints data extract | GN | 🔴 | |
| C8 | AI complaints data is reported to the AI Governance Committee on a regular basis | Committee meeting packs with AI complaints section; minutes | GN | 🟠 | |
| C9 | A formal redress mechanism exists for customers harmed by incorrect, biased, or erroneous AI decisions | Process documentation; redress policy; sample remediation records | GN | 🟠 | |

---

## Domain 7: Fairness and Bias (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| F1 | Protected characteristics defined and formally documented as prohibited model features for each model type | Feature exclusion list; approved by Legal/Compliance; in model documentation | GN + MMS + Charter | 🔴 | |
| F2 | Proxy discrimination analysis conducted: testing that variables correlated with protected characteristics do not cause indirect discrimination | Proxy analysis section in validation report; correlation analysis results | GN + MMS + Charter | 🔴 | |
| F3 | Fairness metrics formally defined per model category (e.g., demographic parity, equalised odds, predictive parity as appropriate) | Fairness Testing Framework document; metric definitions per model type | GN + Charter | 🟠 | |
| F4 | Pre-deployment fairness testing results documented and reviewed/approved by Governance Committee before go-live | Fairness test report; Committee approval minutes; deployment gate | GN + MMS | 🔴 | |
| F5 | Ongoing fairness monitoring implemented for all Tier 1 and Tier 2 production models | Monitoring plans with fairness metrics; monitoring reports with fairness results | GN + MMS | 🔴 | |
| F6 | Bias remediation process documented with defined SLAs for escalation to Senior Management | Process documentation; SLA definitions | GN | 🟠 | |
| F7 | Evidence of Senior Management escalation and action on any material bias findings | Escalation records; remediation plans with closure dates | GN | 🟠 | |

---

## Domain 8: Third-Party and Vendor AI (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| T1 | Inventory of all third-party AI systems currently deployed by the institution | Vendor AI inventory as subset of (or cross-reference to) main Model Inventory | GN | 🔴 | |
| T2 | AI-specific risk assessment conducted for each live vendor AI system | Completed risk assessments per vendor AI; risk rating | GN | 🔴 | |
| T3 | Vendor contracts include the LFI's right to audit the vendor AI model (methodology, data, testing results) | Contract excerpts showing audit rights clause | GN | 🔴 | |
| T4 | Vendor contracts require the vendor to provide explainability artifacts sufficient for CBUAE examination | Contract excerpts; or vendor letter of undertaking | GN + Charter | 🔴 | |
| T5 | Vendor contracts require advance notification to LFI of material model changes (retraining, threshold changes, new features) | Contract excerpts showing change notification clause; notice period defined | GN + MMS | 🔴 | |
| T6 | Vendor contracts include provisions allowing the LFI to exit or replace the AI system if governance standards are not met | Contract excerpts showing exit/termination for cause clause | GN | 🟠 | |
| T7 | Vendor AI systems are included in the Model Inventory with appropriate tiering and subject to monitoring requirements | Inventory records for vendor AI; monitoring plan for vendor AI | MMS + GN | 🟠 | |

---

## Domain 9: Data Governance for AI (6 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| DA1 | Training data lineage documented for each Tier 1 and Tier 2 model (source systems, transformation steps, version used in training) | Data lineage documentation in Development Documents | MMS + GN | 🟠 | |
| DA2 | Training data quality assessment documented: volume, time period, representativeness, exclusions, known biases | Quality assessment section in Development Documents | MMS + GN | 🟠 | |
| DA3 | Lawful basis for using personal data in AI model training assessed and documented (consent / contract / legitimate interest) | Privacy legal assessment or DPIA; data processing records | GN + Charter | 🟠 | |
| DA4 | Data retention and deletion policies applied to AI training datasets (aligned with UAE PDPL) | Retention schedule; evidence of deletion process for expired training data | GN + Charter | 🟠 | |
| DA5 | Cross-border data transfers in AI pipelines (training data, inference data, model APIs to foreign servers) assessed and approved | Transfer assessment; data processing agreement or adequacy decision | GN + Charter | 🟠 | |
| DA6 | AI data processing activities recorded in the institution's Record of Processing Activities (ROPA) under UAE PDPL | ROPA entries for each AI system processing personal data | GN + Charter | 🟠 | |

---

## Domain 10: Internal Audit AI Coverage (7 controls)

| # | Control | Evidence Required | Framework | Priority | Status |
|---|---------|------------------|-----------|----------|--------|
| IA1 | AI/Model risk explicitly included in the annual Internal Audit plan with dedicated audit assignments | Annual Internal Audit plan; AI audit assignments | All | 🟠 | |
| IA2 | Model Inventory completeness audit conducted (at least annually) | Internal Audit report on inventory; findings and management response | MMS | 🟠 | |
| IA3 | Model documentation compliance audit conducted (sample of Tier 1 and Tier 2 models) | Internal Audit report on documentation; findings | MMS | 🟠 | |
| IA4 | Validation independence and quality audit conducted | Internal Audit report on validation function | MMS | 🟠 | |
| IA5 | Consumer AI disclosure compliance audit conducted | Internal Audit report on consumer disclosures; mystery shopping or testing | GN | 🟠 | |
| IA6 | Vendor AI contract compliance audit conducted | Internal Audit report on vendor AI contracts; gaps identified | GN | 🟠 | |
| IA7 | Internal Audit AI findings tracked and followed up in Governance Committee with management response and closure evidence | Committee minutes with IA findings agenda; finding closure records | All | 🟠 | |

---

## Summary Dashboard

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
| D9: Data Governance for AI | 6 | 0 | 6 | | |
| D10: Internal Audit AI Coverage | 7 | 0 | 7 | | |
| **TOTAL** | **70** | **40** | **30** | | |

---

## Examiner Focus Areas

Based on typical CBUAE examination methodology, examiners will prioritise the following in an AI-focused review:

1. **Model Inventory** — First document requested. Must be complete, current, and attested.
2. **Tier 1 Documentation Pack** — For a sample of 3–5 high-impact models, all five documents will be requested.
3. **Validation Reports** — Examiners will read the formal opinion and check for outstanding critical findings.
4. **Consumer Disclosure Evidence** — Live testing of websites, apps, and chatbot interactions may be conducted.
5. **Human Review Process** — Process documentation and log of review requests and outcomes.
6. **Governance Minutes** — Board and Committee minutes demonstrating AI risk is actively discussed.
7. **Fairness Testing Evidence** — Results and what remediation actions were taken.

> **Preparation tip:** Prepare an Examination Pack in advance containing the 20 key artefacts listed in README.md Section 6. Examiners appreciate organised, well-indexed documentation.

---

*Last updated: April 2026 | Part of the [UAE AI Compliance Guide](./README.md)*
