# Implementation Roadmap: UAE AI Compliance for Banking & Fintech

> Phased plan covering CBUAE Guidance Note on Responsible AI, CBUAE Model Management Standards, and UAE AI Charter

---

## Overview

| Phase | Timeline | Goal | Key Output |
|-------|----------|------|-----------|
| **Phase 1 — Foundation** | Months 1–3 | Minimum viable governance; stop examination gaps | Governance structure live; Model Inventory v1; High-Impact AI triage complete |
| **Phase 2 — Operationalisation** | Months 4–9 | Full MMS lifecycle implemented; Guidance Note gaps closed | All T1/T2 docs complete; Validation programme running; Consumer disclosures live |
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
| 1.1.7 | Get Board approval for AI Risk Policy incorporating all three framework requirements | CRO | Month 3 | Signed policy; Board minutes |

**Minimum Viable Outcome by Month 3:**
- ✅ Named RAO with ToR
- ✅ Governance Committee constituted and first meeting held
- ✅ Board AI Risk Policy approved referencing UAE AI Charter

---

### Workstream 1.2 — Build Model Inventory (Current State)

**Why now:** The Model Inventory is the first document any CBUAE examiner will request. Without it, the examination starts badly.

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 1.2.1 | Issue a "Model Census" exercise to all business units requiring registration of all AI/ML/model systems | RAO + CRO | Week 1 | Census request email; deadline |
| 1.2.2 | Define Model Inventory template (name, ID, owner, purpose, inputs, outputs, risk tier, validation status) | Model Risk | Week 1–2 | Inventory template |
| 1.2.3 | Collect responses from all business units; consolidate into central inventory | Model Risk | Month 1–2 | Inventory v1.0 |
| 1.2.4 | Obtain completeness attestation from each business unit head | RAO | Month 2 | Signed attestations |
| 1.2.5 | Present Inventory v1.0 to Governance Committee; identify critical gaps | RAO | Month 3 | Committee minutes |
| 1.2.6 | Establish process for ongoing inventory maintenance (new model registration trigger) | Model Risk | Month 3 | Process document |

**What goes in the Inventory:**
- All statistical models (scorecards, regression models, IRB models)
- All ML models (gradient boosting, neural networks, clustering, NLP)
- All AI systems (chatbots, virtual assistants, recommendation engines)
- All vendor/third-party AI systems deployed by the institution
- All rule-based systems that materially influence decisions
- Models in development (not yet in production)

**Minimum Viable Outcome by Month 3:**
- ✅ Model Inventory v1.0 covering all known models
- ✅ Business unit attestations completed
- ✅ Process for ongoing maintenance documented

---

### Workstream 1.3 — High-Impact AI Triage

**Why now:** The Guidance Note obligations for human oversight, explainability, and consumer disclosure are immediate requirements for high-impact consumer-facing AI.

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 1.3.1 | From Inventory, identify all consumer-facing AI making/influencing: credit/eligibility decisions; AML/fraud alerts with consequence; product recommendations; chatbot/virtual assistant interactions | RAO + Business | Month 1–2 | High-Impact AI Register |
| 1.3.2 | For each high-impact AI, assess: Is there a human override mechanism? Is there a consumer disclosure? Is there a complaints pathway? | Compliance | Month 2 | Gap Assessment |
| 1.3.3 | Document all gaps as findings with owners and remediation timelines | RAO | Month 2 | Gap Register |
| 1.3.4 | Escalate critical gaps (no human override, no disclosure) for immediate interim remediation | RAO + CTO | Month 2–3 | Escalation record; remediation plan |
| 1.3.5 | Assign Tier 1 designation to all high-impact consumer-facing AI models | Model Risk | Month 3 | Inventory update |

**Minimum Viable Outcome by Month 3:**
- ✅ High-Impact AI Register complete
- ✅ Gap Assessment against all 7 Guidance Note Pillars
- ✅ Critical gaps escalated with remediation plans in place

---

## Phase 2 — Operationalisation (Months 4–9): Build the Machine

**Objective:** Operationalise the full MMS lifecycle and close all Guidance Note compliance gaps. By end of Phase 2, the institution should be examination-ready across all three frameworks.

---

### Workstream 2.1 — Model Risk Framework Documentation

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.1.1 | Draft comprehensive Model Risk Management Policy and Framework | CRO | Month 4 | Draft document |
| 2.1.2 | Include in Policy: model definition, tiering methodology, development standards, validation requirements, monitoring requirements, change management, decommissioning, roles, reporting | CRO | Month 4 | Policy draft |
| 2.1.3 | Circulate for internal review (Legal, Compliance, Internal Audit, Technology) | CRO | Month 5 | Review comments |
| 2.1.4 | Finalise and obtain Board approval | CRO | Month 6 | Signed policy; Board minutes |
| 2.1.5 | Communicate Policy to all relevant staff; conduct awareness briefings | RAO + HR | Month 6 | Training records |

---

### Workstream 2.2 — Complete Model Documentation (T1 and T2 Priority)

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.2.1 | Prioritise documentation gap-fill for all Tier 1 models | Model Risk | Month 4 | Priority list |
| 2.2.2 | Retrospectively produce Model Concept Documents (acceptable for existing models) | Model Developers | Month 4–5 | Concept docs per model |
| 2.2.3 | Produce Model Development Documents for all Tier 1 models | Model Developers | Month 4–6 | Dev docs per model |
| 2.2.4 | Produce Operational Manuals for all Tier 1 models | Model Owners | Month 5–6 | Operational manuals |
| 2.2.5 | Initiate Model Change Log for all production models from this date forward | Model Owners | Month 4 | Change logs initiated |
| 2.2.6 | Repeat documentation for Tier 2 models | Model Developers | Month 6–8 | T2 docs |

---

### Workstream 2.3 — Stand Up Independent Validation Capability

**Three options — select based on institution size:**

| Option | Suitable For | Approach |
|--------|-------------|----------|
| **A — Internal standalone team** | Large banks | Dedicated Model Validation team reporting to CRO; structurally separate from development |
| **B — Internal rotation model** | Mid-size banks | Qualified Risk/Analytics staff who did not build the model perform validation (acceptable T2; insufficient for systemic T1) |
| **C — External validator** | Fintechs; small banks; systemic T1 models for all sizes | Engage qualified external firm for validation |

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.3.1 | Determine validation structure (A, B, or C) based on model inventory size and tiers | CRO | Month 4 | Decision paper |
| 2.3.2 | Establish/formalise Validation function independence (org chart, ToR, reporting line) | CRO + HR | Month 5 | Org chart; ToR |
| 2.3.3 | Define validation scope and checklist (concept soundness, data quality, performance, explainability, fairness, stress tests) | Validation Lead | Month 5 | Validation methodology doc |
| 2.3.4 | Create Validation Report template with formal opinion section | Validation Lead | Month 5 | Template |
| 2.3.5 | Begin validation queue — prioritise Tier 1 models | Validation Team | Month 5–9 | Validation reports per model |
| 2.3.6 | Track all outstanding findings in Validation Finding Tracker with owners and due dates | Model Risk | Month 5 onwards | Findings tracker |

---

### Workstream 2.4 — Implement Model Monitoring

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.4.1 | Define monitoring metric set per model type (PSI, KS, Gini, AUC, outcome rates, fairness metrics) | Model Risk | Month 4–5 | Monitoring standards doc |
| 2.4.2 | Define alert thresholds per metric per model | Model Owners | Month 5–6 | Monitoring plan per model |
| 2.4.3 | Implement automated monitoring dashboards where possible | Technology | Month 6–8 | Live dashboards |
| 2.4.4 | Define monitoring breach escalation protocol (threshold breach → alert → investigation → escalation → action) | Model Risk | Month 5 | Escalation protocol |
| 2.4.5 | Produce first monitoring reports and present to Governance Committee | Model Owners | Month 8–9 | Monitoring reports; minutes |
| 2.4.6 | Integrate fairness/bias metrics into monitoring for all Tier 1/2 models | Model Risk | Month 7–8 | Monitoring plans updated |

---

### Workstream 2.5 — Consumer-Facing Compliance (Guidance Note Pillars 2–5)

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.5.1 | Audit all customer-facing products and channels for AI use disclosure gaps | Compliance + Legal | Month 4 | Disclosure audit report |
| 2.5.2 | Draft and approve disclosure language for: product terms, website, mobile app, chatbot opening screens | Legal + Marketing | Month 5–6 | Approved disclosure templates |
| 2.5.3 | Implement "AI used in this decision" notifications for all high-impact adverse decisions | Technology + Ops | Month 6–8 | Notification templates; system config |
| 2.5.4 | Build consumer explanation process: request channel → explanation generation → delivery → logging | Operations + Technology | Month 6–8 | Process document; test cases |
| 2.5.5 | Build human review request workflow: request channel → assignment → SLA → outcome → logging | Operations | Month 6–8 | Workflow documentation; SLA |
| 2.5.6 | Update complaints system to create AI complaints as named category | Technology + Compliance | Month 6 | System config; complaints procedure |
| 2.5.7 | Update AI chatbots/virtual assistants to identify themselves as AI at session start | Technology | Month 5 | UI implementation; test evidence |
| 2.5.8 | Document and test all redress mechanisms for AI-caused customer harm | Compliance + Operations | Month 8 | Process document; test records |

---

### Workstream 2.6 — Fairness and Bias Programme

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.6.1 | Define Fairness Testing Framework: protected characteristics, fairness metrics per model type, testing methodology | Model Risk + Legal | Month 4–5 | Framework document |
| 2.6.2 | Integrate fairness testing checklist into Validation methodology | Validation Lead | Month 5 | Updated validation checklist |
| 2.6.3 | Conduct retrospective fairness testing for all live Tier 1 models not previously tested | Validation Team | Month 5–8 | Fairness test reports |
| 2.6.4 | Integrate ongoing fairness metrics into all Tier 1/2 model monitoring plans | Model Risk | Month 7 | Updated monitoring plans |
| 2.6.5 | Define and document escalation SLAs for fairness findings | Compliance | Month 5 | Escalation process doc |
| 2.6.6 | Report fairness programme status to Governance Committee | RAO | Month 9 | Committee report; minutes |

---

### Workstream 2.7 — Vendor AI Due Diligence

**Actions:**

| # | Action | Owner | Timeline | Evidence |
|---|--------|-------|----------|----------|
| 2.7.1 | Inventory all third-party AI systems currently deployed | Procurement + Technology | Month 4 | Vendor AI inventory |
| 2.7.2 | Develop AI-specific vendor risk assessment questionnaire | Risk + Legal | Month 4–5 | Questionnaire template |
| 2.7.3 | Conduct AI risk assessment for each live vendor AI system | Risk | Month 5–7 | Completed assessments |
| 2.7.4 | Review all vendor AI contracts for: audit rights, explainability obligations, model change notification, exit provisions | Legal | Month 5–7 | Contract review report |
| 2.7.5 | Engage vendors to negotiate contract amendments where required | Legal + Procurement | Month 7–9 | Amended contracts or letter of undertaking |
| 2.7.6 | Integrate AI risk into standard TPRM onboarding process | Risk + Procurement | Month 8 | Updated TPRM process; template |

---

## Phase 3 — Maturity and Continuous Improvement (Months 10–18+)

**Objective:** Build a sustainable, self-improving AI compliance programme that stays ahead of regulatory evolution.

---

### Workstream 3.1 — Internal Audit AI Coverage

| # | Action | Owner | Timeline |
|---|--------|-------|----------|
| 3.1.1 | Include AI/Model risk in annual Internal Audit plan | Head of IA | Month 10 |
| 3.1.2 | Conduct Model Inventory completeness audit | Internal Audit | Month 11 |
| 3.1.3 | Conduct Model documentation compliance audit (sample of T1/T2) | Internal Audit | Month 12 |
| 3.1.4 | Conduct Consumer disclosure compliance audit | Internal Audit | Month 13 |
| 3.1.5 | Conduct Vendor AI contract compliance audit | Internal Audit | Month 14 |
| 3.1.6 | Conduct Fairness monitoring audit | Internal Audit | Month 15 |
| 3.1.7 | Track all IA findings in Governance Committee; require management response | Governance Committee | Ongoing |

---

### Workstream 3.2 — Board AI Risk Reporting

| # | Action | Owner | Timeline |
|---|--------|-------|----------|
| 3.2.1 | Design Board AI Risk Dashboard template | RAO + CRO | Month 10 |
| 3.2.2 | Dashboard content: model inventory and tier breakdown; validation status; open findings aging; consumer AI complaints; fairness monitoring results; vendor AI issues; new model pipeline | RAO | Month 10 |
| 3.2.3 | Present quarterly Board AI Risk report | RAO | From Month 12 |

---

### Workstream 3.3 — Training and Culture

| Audience | Training Content | Delivery | Cadence |
|----------|-----------------|----------|---------|
| AI/ML developers | UAE regulatory requirements; responsible AI development; documentation standards; fairness testing | Instructor-led or e-learning | Annual; on-boarding |
| Model Risk and Compliance | Framework requirements; validation methodology; consumer protection obligations | Instructor-led | Annual |
| Senior Management | AI risk landscape; regulatory expectations; their personal accountability | Board/ExCo briefing | Annual |
| Board | AI risk awareness; key questions to ask; regulatory trends | Board briefing | Annual |
| All staff | What AI is used for; how to identify AI risk; escalation channels | E-learning | Annual |

---

### Workstream 3.4 — Regulatory Engagement and Change Management

| # | Action | Owner | Timeline |
|---|--------|-------|----------|
| 3.4.1 | Assign regulatory watch responsibility for AI-related publications | Compliance | Month 10 |
| 3.4.2 | Establish AI regulatory change triage process: new guidance → impact assessment → owner assignment → remediation plan | Compliance | Month 10 |
| 3.4.3 | Monitor: CBUAE publications, UAE AI Office, FSRA (ADGM), DFSA (DIFC), IAIS, FSB, BIS on AI | Compliance | Ongoing |
| 3.4.4 | Proactively engage CBUAE supervisors before deploying significant new AI use cases | RAO | As needed |
| 3.4.5 | Participate in CBUAE industry consultations on AI guidance | RAO + Legal | As issued |

---

## Key Milestones Summary

| Milestone | Target Date | Framework |
|-----------|-------------|-----------|
| RAO designated; Governance Committee constituted | End Month 1 | GN + MMS |
| Model Inventory v1.0 complete | End Month 2 | MMS |
| High-Impact AI Gap Assessment complete | End Month 3 | GN |
| Board AI Risk Policy approved | End Month 3 | All |
| Model Risk Management Framework approved | End Month 6 | MMS |
| All Tier 1 model documentation complete | End Month 6 | MMS |
| Independent Validation programme running | End Month 6 | MMS |
| Consumer AI disclosures live across all channels | End Month 8 | GN |
| Human review workflow operational | End Month 8 | GN |
| All Tier 1 models validated | End Month 9 | MMS |
| Vendor AI contracts reviewed and remediated | End Month 9 | GN |
| Fairness testing complete for all Tier 1 models | End Month 9 | GN + MMS |
| Internal Audit AI programme launched | End Month 10 | All |
| Quarterly Board AI Risk Dashboard live | End Month 12 | All |
| First complete annual AI compliance cycle | End Month 18 | All |

---

*Last updated: April 2026 | Part of the [UAE AI Compliance Guide](./README.md)*
