# Implementation Roadmap: UAE AI Compliance for Banking & Fintech

> **Version: 1.1 | Last Reviewed: April 2026**
> Phased plan covering CBUAE Guidance Note on Responsible AI, CBUAE Model Management Standards, and UAE AI Charter

---

## Timeline Calibration by Institution Size

> ⚠️ **Read this before using the roadmap.** The timelines in this document are calibrated for a **proportionate institution** — a regulated fintech or small-to-mid bank with fewer than 20 AI models in the inventory. They are **not realistic** for large institutions.

| Institution Type | Typical AI Model Count | Realistic Full Compliance Timeline | Phase 1 | Phase 2 | Phase 3 |
|-----------------|----------------------|-----------------------------------|---------|---------|---------|
| **Regulated Fintech** | 1–5 models | 12–15 months | Months 1–3 | Months 4–9 | Months 10–15 |
| **Small Bank / Finance Co.** | 5–20 models | 15–18 months | Months 1–3 | Months 4–10 | Months 11–18 |
| **Mid-size Bank** | 20–50 models | 18–24 months | Months 1–3 | Months 4–12 | Months 13–24 |
| **D-SIB / Large Bank** | 50–150+ models | 24–36 months | Months 1–4 | Months 5–18 | Months 19–36 |

> **Validation bottleneck:** A single complex ML model validation takes 4–8 weeks. A large bank with 20 Tier 1 models requires 10–20 months of validation capacity at full throughput — before documentation remediation and queue management. Build your validation capacity plan first; it will determine your critical path.

> **Board meeting cycle:** The "Board Policy approved by Month 3" milestone assumes a board meeting falls within that window. Most UAE bank boards meet quarterly. If Month 1 starts just after a board meeting, your first opportunity may be Month 4. Plan accordingly — a Board Risk Committee can often provide interim approval.

---

## Phase Overview

| Phase | Indicative Timeline | Goal | Key Output |
|-------|----------|------|-----------|
| **Phase 1 — Foundation** | Months 1–3 | Minimum viable governance; stop examination gaps | Governance structure live; Model Inventory v1; High-Impact AI triage complete |
| **Phase 2 — Operationalisation** | Months 4–9 (small) / 4–18 (large) | Full MMS lifecycle implemented; Guidance Note gaps closed | All T1/T2 docs complete; Validation programme running; Consumer disclosures live |
| **Phase 3 — Maturity** | Months 10–18+ | Sustainable compliance; continuous improvement | Internal Audit AI plan; Board AI Dashboard; Training programme complete |

---

## Phase 1 — Foundation (Months 1–3): Stop the Bleeding

**Objective:** Ensure minimum viable governance is in place and demonstrable to examiners today. Focus on the highest-risk gaps first.

---

### Workstream 1.1 — Establish AI Governance Structure

**Why now:** The CBUAE Guidance Note is already in effect. Examiners will look for a governance structure from Day 1 of any examination.

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 1.1.1 | Designate a Responsible AI Officer (RAO) at Senior Management level with formal terms of reference | CEO/Board | Week 1 | Appointment letter; ToR |
| 1.1.2 | Constitute an AI/Model Governance Committee with documented membership and ToR | CRO + Legal | Week 2 | Committee ToR; membership list |
| 1.1.3 | Define Committee meeting cadence (minimum quarterly), quorum rules, and escalation protocol | CRO + Legal | Week 2 | ToR document |
| 1.1.4 | Prepare a Board paper formally adopting UAE AI Charter principles into AI Policy | RAO + Legal | Week 3–4 | Board paper; draft AI Policy |
| 1.1.5 | Schedule Board AI risk agenda item at next Board/Risk Committee meeting | Company Secretary | Week 2 | Board agenda; invitation |
| 1.1.6 | Define first/second/third line responsibilities for AI risk in RACI format | CRO + HR | Month 2 | RACI matrix |
| 1.1.7 | Get Board (or Board Risk Committee) approval for AI Risk Policy | CRO | Month 3 (or next board cycle) | Signed policy; Board minutes |

> **Timing note:** If no board meeting falls in Month 3, seek Board Risk Committee or equivalent delegated approval for the policy as an interim measure. Do not delay governance work waiting for a board meeting — the Committee structure and RAO designation are independent of the board cycle.

**Minimum Viable Outcome by Month 3:**
- ✅ Named RAO with ToR
- ✅ Governance Committee constituted and first meeting held with minutes
- ✅ Board AI Risk Policy approved (or interim approval obtained) referencing UAE AI Charter

---

### Workstream 1.2 — Build Model Inventory (Current State)

**Why now:** The Model Inventory is the first document any CBUAE examiner will request. Without it, the examination starts badly.

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 1.2.1 | Issue a "Model Census" exercise to all business units requiring registration of all AI/ML/model systems | RAO + CRO | Week 1 | Census request email; deadline |
| 1.2.2 | Define Model Inventory template (name, ID, owner, purpose, inputs, outputs, risk tier, high-impact classification, validation status) | Model Risk | Week 1–2 | Inventory template |
| 1.2.3 | Collect responses from all business units; consolidate into central inventory | Model Risk | Month 1–2 | Inventory v1.0 |
| 1.2.4 | Obtain completeness attestation from each business unit head | RAO | Month 2 | Signed attestations |
| 1.2.5 | Present Inventory v1.0 to Governance Committee; identify critical gaps | RAO | Month 3 | Committee minutes |
| 1.2.6 | Establish process for ongoing inventory maintenance (new model registration trigger) | Model Risk | Month 3 | Process document |

**What must be in the Inventory:**
- All statistical models (scorecards, regression models, IRB models)
- All ML models (gradient boosting, neural networks, clustering, NLP)
- All AI systems (chatbots, virtual assistants, recommendation engines)
- All vendor/third-party AI systems deployed by the institution
- All rule-based systems that materially influence decisions
- Models in development (not yet in production)

**Minimum Viable Outcome by Month 3:**
- ✅ Model Inventory v1.0 covering all known models with high-impact classification column populated
- ✅ Business unit attestations completed
- ✅ Process for ongoing maintenance documented

---

### Workstream 1.3 — High-Impact AI Triage and Model Tiering

**Why now:** The Guidance Note obligations for human oversight, explainability, and consumer disclosure are immediate requirements for high-impact consumer-facing AI. Tiering must be done before validation prioritisation and resource planning.

#### The Tiering Decision Framework

Use the following five-question assessment to tier each model. Answer each question and apply the highest tier triggered by any "Yes" answer.

---

**Question 1 — Consumer Financial Access Impact**
> Does this model make or materially influence a decision about a customer's access to, eligibility for, or continued use of any financial product or service?

| Answer | Indicator | Examples |
|--------|-----------|---------|
| **Yes** | → **Tier 1** | Credit approval/rejection; loan eligibility; account opening decisions; overdraft limit; mortgage offer; BNPL; product restriction |
| No | → Proceed to Q2 | |

---

**Question 2 — Consumer Financial Terms Impact**
> Does this model make or materially influence the price, interest rate, fee, or contractual terms applied to a specific customer?

| Answer | Indicator | Examples |
|--------|-----------|---------|
| **Yes** | → **Tier 1** | Risk-based pricing engines; interest rate decisioning; insurance premium calculation; fee tier assignment |
| No | → Proceed to Q3 | |

---

**Question 3 — Regulatory or Legal Consequence**
> Does this model trigger or suppress a regulatory action, legal consequence, or formal risk classification that directly affects the customer?

| Answer | Indicator | Examples |
|--------|-----------|---------|
| **Yes** | → **Tier 1** | AML transaction monitoring; fraud detection leading to account freeze; sanctions screening; SAR-triggering models; credit bureau reporting |
| No | → Proceed to Q4 | |

---

**Question 4 — Material Business Decision / Internal Risk**
> Does this model materially influence a significant internal business decision, regulatory capital calculation, or risk rating — even if not directly customer-facing?

| Answer | Indicator | Examples |
|--------|-----------|---------|
| **Yes** | → **Tier 2** | IFRS 9 ECL models; internal credit risk models; capital adequacy models; liquidity risk models; portfolio stress testing |
| No | → Proceed to Q5 | |

---

**Question 5 — Scale and Breadth**
> Does this model affect more than 1,000 customers simultaneously, or does it operate across a portfolio in a way that could amplify or systematically introduce errors at scale?

| Answer | Indicator | Examples |
|--------|-----------|---------|
| **Yes, and affects customer outcomes** | → **Tier 1 or 2** (apply Q1–3 to determine) | Marketing segmentation affecting product availability; repricing engines; automated complaints triage |
| **Yes, but purely internal** | → **Tier 2** | Internal portfolio analytics; management reporting |
| **No** | → **Tier 3** | Narrow, low-impact, transparent models |

---

**Tiering Summary Scorecard**

| Any "Yes" to Q1, Q2, or Q3? | Any "Yes" to Q4 or Q5 (internal)? | Tier Assignment |
|-----------------------------|-----------------------------------|----------------|
| ✅ Yes | Any | **Tier 1** — Full independent validation; Board oversight; annual review; all Guidance Note consumer obligations apply |
| ❌ No | ✅ Yes | **Tier 2** — Proportionate validation; Senior Management oversight; 18-month cycle; Guidance Note consumer obligations may apply if customer-facing |
| ❌ No | ❌ No | **Tier 3** — Documented owner; periodic review; lighter validation; standard controls only |

> **Documentation requirement:** For every model, record the five question answers, the tier assigned, and the rationale — especially for any borderline cases. The Responsible AI Officer must approve all Tier 1 and Tier 2 assignments. This record must be held in or alongside the Model Inventory and available for CBUAE examination.

---

**Triage Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 1.3.1 | Apply 5-question tiering framework to all models in inventory | Model Risk + Business | Month 1–2 | Tiering assessment per model |
| 1.3.2 | Identify all Tier 1 models — these are the highest-risk examination exposure | RAO + Model Risk | Month 2 | Tier 1 model list |
| 1.3.3 | For each Tier 1 model, assess Guidance Note gaps: human override? consumer disclosure? complaints pathway? explainability? | Compliance | Month 2 | Gap Assessment per model |
| 1.3.4 | Document all gaps as findings with owners and remediation timelines | RAO | Month 2 | Gap Register |
| 1.3.5 | Escalate critical gaps (no human override, no disclosure on live Tier 1 models) for immediate interim controls | RAO + CTO | Month 2–3 | Escalation record; interim control evidence |
| 1.3.6 | RAO approves all Tier 1 and Tier 2 tier assignments; update inventory | RAO | Month 3 | Inventory update; RAO sign-off |

**Minimum Viable Outcome by Month 3:**
- ✅ All models tiered using documented 5-question framework
- ✅ Tier 1 model list agreed and RAO-approved
- ✅ Gap Assessment against all 7 Guidance Note Pillars for each Tier 1 model
- ✅ Critical gaps escalated with interim controls in place

---

## Phase 2 — Operationalisation (Months 4–9 for small; 4–18 for large): Build the Machine

**Objective:** Operationalise the full MMS lifecycle and close all Guidance Note compliance gaps.

---

### Workstream 2.1 — Model Risk Framework Documentation

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.1.1 | Draft comprehensive Model Risk Management Policy and Framework | CRO | Month 4 | Draft document |
| 2.1.2 | Include: model definition, tiering methodology (5-question framework), development standards, validation requirements (with Tier 2 proportionality definition), monitoring requirements, change management, decommissioning, roles, reporting | CRO | Month 4 | Policy draft |
| 2.1.3 | Circulate for review (Legal, Compliance, Internal Audit, Technology) | CRO | Month 5 | Review comments |
| 2.1.4 | Finalise and obtain Board/BRC approval | CRO | Month 6 | Signed policy; Board minutes |
| 2.1.5 | Communicate to all relevant staff; conduct awareness briefings | RAO + HR | Month 6 | Training records |

---

### Workstream 2.2 — Complete Model Documentation (T1 Priority First, T2 Second)

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.2.1 | Prioritise documentation gap-fill for all Tier 1 models | Model Risk | Month 4 | Priority list |
| 2.2.2 | Retrospectively produce Model Concept Documents for existing Tier 1 models | Model Developers | Month 4–5 | Concept docs per model |
| 2.2.3 | Produce Model Development Documents for all Tier 1 models | Model Developers | Month 4–6 | Dev docs per model |
| 2.2.4 | Produce Operational Manuals for all Tier 1 models | Model Owners | Month 5–6 | Operational manuals |
| 2.2.5 | Initiate Model Change Log for all production models from this date forward | Model Owners | Month 4 | Change logs initiated |
| 2.2.6 | Repeat for Tier 2 models (scaled by institution size) | Model Developers | Month 6–12 | T2 docs |

---

### Workstream 2.3 — Stand Up Independent Validation Capability

**Three options — select based on institution type:**

| Option | Suitable For | Approach |
|--------|-------------|----------|
| **A — Internal standalone team** | D-SIB / Large banks | Dedicated Model Validation team reporting to CRO; structurally separate from development; full-time |
| **B — Internal rotation model** | Mid-size banks | Qualified Risk/Analytics staff who did not build the model perform validation; documented independence; acceptable for Tier 2 |
| **C — External validator** | Fintechs; small banks; all institutions for Tier 1 models outside internal expertise | Engage qualified external firm; brief them on UAE MMS requirements |

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.3.1 | Determine validation structure (A, B, C, or hybrid) based on model count, tiers, and internal capability | CRO | Month 4 | Decision paper |
| 2.3.2 | Build validation queue: Tier 1 first, sequenced by risk level; estimate capacity vs. backlog | Validation Lead | Month 4 | Validation queue plan with timeline |
| 2.3.3 | Establish Validation function independence (org chart, ToR, reporting line) | CRO + HR | Month 5 | Org chart; ToR |
| 2.3.4 | Create Validation Report template including: opinion section, explainability assessment, fairness testing section | Validation Lead | Month 5 | Template |
| 2.3.5 | Begin Tier 1 validation queue — highest risk models first | Validation Team | Month 5 onwards | Validation reports per model |
| 2.3.6 | Track all findings in Validation Finding Tracker with severity, owners, due dates | Model Risk | Month 5 onwards | Findings tracker |

> **Capacity planning note:** At 4–8 weeks per Tier 1 model, plan validation throughput realistically. A single validator handles 6–12 models per year. Large institutions with 20+ Tier 1 models need multiple validators or a phased external engagement. The validation queue plan (2.3.2) is a critical path document — produce it before committing to any timeline to management or the board.

---

### Workstream 2.4 — Implement Model Monitoring

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.4.1 | Define monitoring metric set per model type (PSI, KS, Gini, AUC, outcome rates, fairness metrics) | Model Risk | Month 4–5 | Monitoring standards doc |
| 2.4.2 | Define alert thresholds per metric per model | Model Owners | Month 5–6 | Monitoring plan per model |
| 2.4.3 | Implement automated monitoring dashboards where possible | Technology | Month 6–8 | Live dashboards |
| 2.4.4 | Define monitoring breach escalation protocol | Model Risk | Month 5 | Escalation protocol |
| 2.4.5 | Produce first monitoring reports and present to Governance Committee | Model Owners | Month 8–9 | Monitoring reports; minutes |
| 2.4.6 | Integrate fairness/bias metrics into monitoring for all Tier 1/2 models | Model Risk | Month 7–8 | Updated monitoring plans |

---

### Workstream 2.5 — Consumer-Facing Compliance (Guidance Note Pillars 2–5)

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.5.1 | Audit all customer-facing products and channels for AI disclosure gaps | Compliance + Legal | Month 4 | Disclosure audit report |
| 2.5.2 | Draft and approve disclosure language for: product terms, website, mobile app, chatbot opening screens | Legal + Marketing | Month 5–6 | Approved disclosure templates |
| 2.5.3 | Implement "AI used in this decision" notifications for all high-impact adverse decisions | Technology + Ops | Month 6–8 | Notification templates; system config |
| 2.5.4 | Build consumer explanation process: request channel → explanation generation → delivery → logging | Operations + Technology | Month 6–8 | Process document; test cases |
| 2.5.5 | Build human review request workflow: request channel → assignment → SLA → outcome → logging | Operations | Month 6–8 | Workflow documentation; SLA |
| 2.5.6 | Update complaints system to create AI complaints as named category | Technology + Compliance | Month 6 | System config; complaints procedure |
| 2.5.7 | Update AI chatbots/virtual assistants to identify themselves as AI at session start | Technology | Month 5 | UI implementation; test evidence |
| 2.5.8 | Document and test all redress mechanisms for AI-caused customer harm | Compliance + Operations | Month 8 | Process document; test records |

---

### Workstream 2.6 — Fairness and Bias Programme

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.6.1 | Define Fairness Testing Framework: protected characteristics, fairness metrics per model type, testing methodology | Model Risk + Legal | Month 4–5 | Framework document |
| 2.6.2 | Integrate fairness testing checklist into validation methodology | Validation Lead | Month 5 | Updated validation checklist |
| 2.6.3 | Conduct retrospective fairness testing for all live Tier 1 models not previously tested | Validation Team | Month 5–8 | Fairness test reports |
| 2.6.4 | Integrate ongoing fairness metrics into all Tier 1/2 model monitoring plans | Model Risk | Month 7 | Updated monitoring plans |
| 2.6.5 | Define and document escalation SLAs for fairness findings | Compliance | Month 5 | Escalation process doc |
| 2.6.6 | Report fairness programme status to Governance Committee | RAO | Month 9 | Committee report; minutes |

---

### Workstream 2.7 — Vendor AI Due Diligence

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.7.1 | Inventory all third-party AI systems currently deployed | Procurement + Technology | Month 4 | Vendor AI inventory |
| 2.7.2 | Develop AI-specific vendor risk assessment questionnaire | Risk + Legal | Month 4–5 | Questionnaire template |
| 2.7.3 | Conduct AI risk assessment for each live vendor AI system | Risk | Month 5–7 | Completed assessments |
| 2.7.4 | Review all vendor AI contracts for: audit rights, explainability obligations, model change notification, exit provisions | Legal | Month 5–7 | Contract review report |
| 2.7.5 | Engage vendors to negotiate contract amendments where required | Legal + Procurement | Month 7–9 | Amended contracts |
| 2.7.6 | Integrate AI risk into standard TPRM onboarding process | Risk + Procurement | Month 8 | Updated TPRM process |

---

## Phase 3 — Maturity and Continuous Improvement (Months 10+)

### Workstream 3.1 — Internal Audit AI Coverage

| # | Action | Owner | Timeline |
|---|--------|-------|----------|
| 3.1.1 | Include AI/Model risk in annual Internal Audit plan | Head of IA | Month 10 |
| 3.1.2 | Conduct Model Inventory completeness audit | Internal Audit | Month 11 |
| 3.1.3 | Conduct Model documentation compliance audit (sample of T1/T2) | Internal Audit | Month 12 |
| 3.1.4 | Conduct Tiering Decision Framework consistency audit (are models correctly tiered?) | Internal Audit | Month 12 |
| 3.1.5 | Conduct Consumer disclosure compliance audit | Internal Audit | Month 13 |
| 3.1.6 | Conduct Vendor AI contract compliance audit | Internal Audit | Month 14 |
| 3.1.7 | Conduct Fairness monitoring audit | Internal Audit | Month 15 |
| 3.1.8 | Track all IA findings in Governance Committee; require management response | Governance Committee | Ongoing |

---

### Workstream 3.2 — Board AI Risk Reporting

| # | Action | Owner | Timeline |
|---|--------|-------|----------|
| 3.2.1 | Design Board AI Risk Dashboard template | RAO + CRO | Month 10 |
| 3.2.2 | Dashboard content: inventory & tier breakdown; validation status; open findings aging; consumer AI complaints; fairness monitoring results; vendor AI issues; new model pipeline; tiering changes | RAO | Month 10 |
| 3.2.3 | Present quarterly Board AI Risk report | RAO | From Month 12 |

---

### Workstream 3.3 — Training and Culture

| Audience | Training Content | Delivery | Cadence |
|----------|-----------------|----------|---------|
| AI/ML developers | UAE regulatory requirements; responsible AI development; documentation standards; fairness testing; tiering criteria | Instructor-led or e-learning | Annual; on-boarding |
| Model Risk and Compliance | Framework requirements; validation methodology; 5-question tiering framework; consumer protection obligations | Instructor-led | Annual |
| Senior Management | AI risk landscape; regulatory expectations; personal accountability; tiering and high-impact classification | Board/ExCo briefing | Annual |
| Board | AI risk awareness; key questions to ask; regulatory trends | Board briefing | Annual |
| All staff | What AI is used for; how to identify AI risk; escalation channels | E-learning | Annual |

---

### Workstream 3.4 — Regulatory Engagement and Change Management

| # | Action | Owner | Timeline |
|---|--------|-------|----------|
| 3.4.1 | Assign regulatory watch responsibility for AI-related publications | Compliance | Month 10 |
| 3.4.2 | Establish AI regulatory change triage process | Compliance | Month 10 |
| 3.4.3 | Monitor: CBUAE, UAE AI Office, FSRA, DFSA, Insurance Authority, IAIS, FSB, BIS | Compliance | Ongoing |
| 3.4.4 | Proactively engage CBUAE before deploying significant new AI use cases | RAO | As needed |
| 3.4.5 | Participate in CBUAE industry consultations on AI guidance | RAO + Legal | As issued |

---

## Key Milestones Summary

| Milestone | Fintech / Small Bank | Mid-size Bank | Large Bank / D-SIB | Framework |
|-----------|---------------------|---------------|-------------------|-----------|
| RAO designated; Governance Committee constituted | Month 1 | Month 1 | Month 1 | GN + MMS |
| Model Inventory v1.0 + tiering complete | Month 2 | Month 2–3 | Month 3–4 | MMS |
| High-Impact AI Gap Assessment complete | Month 3 | Month 3 | Month 4 | GN |
| Board AI Risk Policy approved | Month 3 | Month 3–4 | Month 4–5 | All |
| Model Risk Framework approved | Month 6 | Month 6 | Month 6 | MMS |
| Tier 1 documentation complete | Month 6 | Month 6–9 | Month 9–12 | MMS |
| Validation programme running | Month 6 | Month 6 | Month 6 | MMS |
| Consumer AI disclosures live | Month 8 | Month 8–10 | Month 10–12 | GN |
| Human review workflow operational | Month 8 | Month 8–10 | Month 10–12 | GN |
| All Tier 1 models validated | Month 9 | Month 12–15 | Month 18–24 | MMS |
| Vendor AI contracts reviewed/remediated | Month 9 | Month 9–12 | Month 12–15 | GN |
| Fairness testing complete (Tier 1) | Month 9 | Month 12 | Month 15–18 | GN + MMS |
| Internal Audit AI programme launched | Month 10 | Month 12 | Month 18 | All |
| Board AI Dashboard live | Month 12 | Month 12–15 | Month 18 | All |
| First complete compliance cycle | Month 15 | Month 18 | Month 30–36 | All |

---

*Version 1.1 | Last updated: April 2026 | Part of the [UAE AI Compliance Guide](./README.md) | See [CHANGELOG.md](./CHANGELOG.md)*
