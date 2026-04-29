# UAE AI Compliance Guide for Banking & Fintech

## Three-Framework Integration: CBUAE Responsible AI Guidance Note · CBUAE Model Management Standards · UAE AI Charter

> **Edition: 2026 | Target Audience: Licensed Financial Institutions (LFIs), Fintechs, Boards, CROs, CTOs, Compliance Officers**

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
![Sector](https://img.shields.io/badge/Sector-UAE%20Banking%20%26%20Fintech-blue)
![Status](https://img.shields.io/badge/Status-Active-green)

---

## 📁 Repository Structure

| File | Description |
|------|-------------|
| `README.md` | Full end-to-end guide (this file) |
| `FRAMEWORK-MAPPING.md` | Detailed cross-framework requirements matrix |
| `IMPLEMENTATION-ROADMAP.md` | Phased implementation plan with workstreams |
| `AUDIT-CHECKLIST.md` | Complete audit & examination readiness checklists (70 controls) |
| `BOARD-BRIEFING.md` | One-page board briefing card |

---

## 📋 Table of Contents

1. [Executive Overview](#1-executive-overview)
2. [Understanding the Three Frameworks](#2-understanding-the-three-frameworks)
3. [Framework Mapping](#3-framework-mapping)
4. [Implementation Roadmap](#4-implementation-roadmap)
5. [Audit & Examination Readiness Checklist](#5-audit-and-examination-readiness-checklist)
6. [Key Artefacts Library](#6-key-artefacts-library)
7. [UAE-Specific Practical Considerations](#7-uae-specific-practical-considerations)
8. [Glossary](#8-glossary)
9. [Board Briefing Card](#9-board-briefing-card)

---

## 1. Executive Overview

### 1.1 Why This Guide Exists

The UAE has moved faster than most jurisdictions in translating AI ambition into binding supervisory expectation. Three instruments now define the compliance landscape for any bank or fintech deploying AI or data-driven models in the UAE:

| # | Framework | Status | Who It Binds |
|---|-----------|--------|--------------|
| 1 | **CBUAE Guidance Note on Consumer Protection & Responsible AI** | Issued Feb 2026; in effect | All Licensed Financial Institutions |
| 2 | **CBUAE Rulebook — Big Data Analytics & AI (Model Management Standards)** | In-force; foundational | All Licensed Financial Institutions |
| 3 | **UAE AI Charter** | Published June 2024; actively cited | All entities operating in UAE |

These three instruments form a **layered compliance architecture**:

```
UAE AI Charter (national ethical values & principles)
        ↓
CBUAE Model Management Standards (operational model governance)
        ↓
CBUAE Guidance Note on Responsible AI (consumer-facing AI obligations)
```

### 1.2 Who Is In Scope

| Entity Type | MMS | Guidance Note | AI Charter |
|-------------|-----|---------------|------------|
| UAE-licensed banks (national and foreign) | ✅ Full | ✅ Full | ✅ Policy baseline |
| Finance companies (CBUAE licensed) | ✅ Full | ✅ Full | ✅ Policy baseline |
| Exchange houses | ⚡ Partial (where AI used) | ⚡ Partial | ✅ Policy baseline |
| Licensed payment service providers | ✅ Where AI models used | ✅ Where consumer-facing | ✅ Policy baseline |
| Fintechs (CBUAE regulated) | ✅ Proportionate | ✅ Full | ✅ Policy baseline |
| ADGM/DIFC-licensed entities | ⚡ Indirect (own regulators) | ⚡ Indirect | ✅ Policy baseline |

---

## 2. Understanding the Three Frameworks

### 2.1 CBUAE Guidance Note on Consumer Protection and Responsible AI (February 2026)

**Nature:** Supervisory guidance note — takes immediate effect as examination expectation. Non-compliance triggers findings, remediation orders, or restrictions on AI deployment.

#### Seven Pillars

| Pillar | Core Requirement |
|--------|----------------|
| **1 — Governance & Accountability** | Board bears ultimate accountability; named Responsible AI Officer at Senior Management level; cross-functional AI Governance Committee |
| **2 — Human Oversight & Intervention** | Human review mechanism for all high-impact AI decisions; customers have right to request human review; overrides logged |
| **3 — Explainability** | Technical explainability for examiners; plain-language consumer explanations for adverse decisions; black-box is not acceptable |
| **4 — Fairness & Non-Discrimination** | Pre-deployment and ongoing bias testing; protected characteristics excluded as features; proxy discrimination monitored |
| **5 — Consumer Protection Disclosures** | Customers notified AI made decisions affecting them; AI chatbots must identify themselves; redress mechanism for AI harm |
| **6 — Data Governance for AI** | Training data documented and fit-for-purpose; data lineage maintained; UAE PDPL compliance mandatory |
| **7 — Third-Party & Vendor AI** | LFI fully responsible for vendor AI; due diligence required; contracts must include audit rights, explainability obligations, exit provisions |

> **Key principle:** "We bought it from a vendor" is **not** a valid supervisory defence.

---

### 2.2 CBUAE Rulebook — Big Data Analytics and AI: Model Management Standards (MMS)

**Nature:** Binding Rulebook standard — mandatory, not guidance. Governs the full model lifecycle.

**Model Definition:** Any quantitative method processing inputs to produce outputs used in business decisions — including statistical models, ML, generative AI, AML/fraud analytics, pricing engines, and chatbot systems.

#### Model Risk Tiering

| Tier | Characteristics | Minimum Requirements |
|------|----------------|----------------------|
| **Tier 1 (High)** | High-impact consumer decisions; regulatory capital; complex/opaque methodology | Full independent validation; Board oversight; annual review |
| **Tier 2 (Medium)** | Moderate impact; internal management; simpler methodology | Validation required; Senior Management oversight; 18-month cycle |
| **Tier 3 (Low)** | Low impact; narrow use; transparent methodology | Documented owner; periodic review; lighter validation |

#### Five Required Model Documents (per Tier 1 & 2 model)

| # | Document | When |
|---|----------|------|
| 1 | Model Concept Document | Pre-development |
| 2 | Model Development Document | Post-development |
| 3 | Independent Validation Report | Pre-deployment |
| 4 | Operational Manual | At deployment |
| 5 | Model Change Log | Continuously |

#### Independent Validation Requirements
- Validation team structurally independent from model development (four-eyes principle)
- Must cover: conceptual soundness, data quality, performance, outcome analysis, stress testing, explainability, fairness
- Formal opinion required: **Approve / Approve with Conditions / Reject**
- All findings tracked in remediation log with owners and due dates

#### Model Monitoring (all production models)
- Metrics: PSI (input drift), KS/Gini/AUC (performance), outcome analysis, fairness metrics
- Thresholds defined; breaches trigger escalation
- Tier 1: minimum quarterly reporting to governance committee

---

### 2.3 UAE AI Charter (June 2024)

**Nature:** National policy document with significant regulatory weight — CBUAE and other regulators explicitly reference it. Boards must formally adopt Charter principles into AI Policy.

#### Eight Principles and Their Banking/Fintech Implications

| # | Principle | Banking/Fintech Implication |
|---|-----------|----------------------------|
| 1 | **Human Wellbeing & Beneficence** | AI must serve genuine customer interests, not extract value at their expense |
| 2 | **Safety and Reliability** | Pre-deployment testing, stress testing, monitoring — links to MMS validation |
| 3 | **Privacy and Data Protection** | UAE PDPL compliance in all AI data pipelines; consent, purpose limitation, data minimisation |
| 4 | **Transparency and Explainability** | Consumers know when AI is used and how decisions are made |
| 5 | **Fairness and Non-Discrimination** | Bias audits across demographic groups; disparate impact analysis |
| 6 | **Accountability** | Named individual responsible for each AI system — not just committees |
| 7 | **Sustainability** | ESG reporting; environmental impact of AI operations (emerging) |
| 8 | **Inclusivity** | AI must not exclude underserved populations; financial inclusion mandate |

---

## 3. Framework Mapping

See **[FRAMEWORK-MAPPING.md](./FRAMEWORK-MAPPING.md)** for the complete cross-framework requirements matrix.

### Three Themes Spanning All Three Frameworks

**Theme A — Accountable Governance**
All three require named human accountability, committee oversight, and Board-level responsibility. Build this governance structure once; it satisfies all three instruments simultaneously.

**Theme B — Explainability**
Charter (Principle 4), MMS (documentation requirement), Guidance Note (consumer right). A single XAI framework covering both technical and consumer-facing explanations satisfies all three.

**Theme C — Fairness and Bias**
MMS (validation requirement), Guidance Note (ongoing monitoring obligation), Charter (Principle 5). One fairness programme with documented metrics satisfies all three.

### Unique Obligations by Framework

| Framework | Obligations Found Nowhere Else |
|-----------|-------------------------------|
| **Guidance Note Only** | Consumer AI disclosure at point of interaction; individual right to human review; AI chatbot identification requirement; customer redress mechanism; vendor contract audit rights |
| **MMS Only** | Formal 3-tier model risk tiering; five-document model lifecycle kit; formal Validation Report with an opinion; model decommissioning process; model change log |
| **AI Charter Only** | Environmental sustainability considerations; inclusivity for underserved populations; national AI strategic alignment framing |

---

## 4. Implementation Roadmap

See **[IMPLEMENTATION-ROADMAP.md](./IMPLEMENTATION-ROADMAP.md)** for the full phased plan with workstreams, deliverables, and timelines.

### Phase Summary

| Phase | Timeline | Objective | Key Deliverables |
|-------|----------|-----------|-----------------|
| **Phase 1 — Foundation** | Months 1–3 | Stop the Bleeding: minimum viable governance | AI Governance Committee, Model Inventory v1, High-Impact AI Gap Assessment |
| **Phase 2 — Operationalisation** | Months 4–9 | Build the Machine: full MMS lifecycle + Guidance Note gaps closed | Model docs, Validation programme, Monitoring, Consumer disclosures, Vendor AI review |
| **Phase 3 — Maturity** | Months 10–18+ | Sustain and Improve: audit coverage, board reporting, regulatory engagement | Internal Audit AI plan, Board AI Dashboard, Training programme, Regulatory watch |

---

## 5. Audit and Examination Readiness Checklist

See **[AUDIT-CHECKLIST.md](./AUDIT-CHECKLIST.md)** for all 70 controls across 10 domains.

| Domain | Controls | Framework |
|--------|----------|-----------|
| Governance & Accountability | 7 | All three |
| Model Inventory | 7 | MMS |
| Model Development & Documentation | 7 | MMS |
| Independent Validation | 7 | MMS |
| Model Monitoring | 6 | MMS |
| Consumer Protection & Disclosure | 9 | Guidance Note + Charter |
| Fairness & Bias | 7 | All three |
| Third-Party & Vendor AI | 7 | Guidance Note |
| Data Governance for AI | 6 | Guidance Note + Charter |
| Internal Audit AI Coverage | 7 | All three |
| **TOTAL** | **70** | |

---

## 6. Key Artefacts Library

Every LFI must produce and maintain the following documentation:

| # | Document | Owner | Approver | Cadence | Framework |
|---|----------|-------|----------|---------|-----------|
| 1 | AI Risk Policy | CRO/RAO | Board | Annual review | All |
| 2 | Model Risk Management Framework | CRO | Board | Annual review | MMS |
| 3 | AI Governance Committee ToR | Legal/Governance | Board | Annual review | GN + MMS |
| 4 | Model Inventory Register | CRO/CDO | Gov Committee | Continuous | MMS |
| 5 | Model Tiering Methodology | CRO | Gov Committee | Annual review | MMS |
| 6 | Model Concept Document (per model) | Model Developer | Model Risk | Pre-development | MMS |
| 7 | Model Development Document (per model) | Model Developer | Gov Committee | Post-development | MMS |
| 8 | Validation Report (per model) | Validation Team | Gov Committee | Per cycle | MMS |
| 9 | Validation Finding Tracker | Model Risk | CRO | Continuous | MMS |
| 10 | Operational Manual (per model) | Model Owner | Model Risk | At deployment | MMS |
| 11 | Model Change Log (per model) | Model Owner | Model Risk | Per change | MMS |
| 12 | Model Monitoring Plan (per model) | Model Owner | Model Risk | At deployment | MMS |
| 13 | Monitoring Reports (per model) | Model Owner | Gov Committee | Quarterly (T1) | MMS |
| 14 | Fairness Testing Report (per model) | Validation Team | Gov Committee | Per validation | MMS + GN |
| 15 | Vendor AI Risk Assessment | Procurement/Risk | CRO | Per vendor | GN |
| 16 | Consumer AI Disclosure Language | Legal/Compliance | CCO | Annual review | GN + Charter |
| 17 | Human Review Process Document | Operations | CCO | Annual review | GN |
| 18 | AI Complaints Procedure | Compliance | CCO | Annual review | GN |
| 19 | Board AI Risk Report | CRO/RAO | Board | Quarterly | All |
| 20 | AI Regulatory Change Register | Compliance | CCO | Continuous | All |

---

## 7. UAE-Specific Practical Considerations

### 7.1 Regulatory Examination Preparation

CBUAE examiners will assess:
- **Model Inventory** — first document requested; must be complete and current
- **Tier 1 documentation packs** — sample of 3–5 high-impact models with all five documents
- **Interviews** — Responsible AI Officer and Validation team leads
- **Consumer complaints data** — AI-related themes and resolution
- **Human review process** — tested with a sample scenario
- **Board/committee minutes** — evidence of AI risk discussion at governance level
- **Fairness testing evidence** — results and remediation actions taken

> **Key insight:** Examiners differentiate between governance *on paper* vs. governance *in practice*. Meeting minutes, escalation logs, remediation trackers, and monitoring dashboards are the operational evidence that matters.

### 7.2 ADGM and DIFC Entities

ADGM/DIFC entities are primarily regulated by FSRA/DFSA respectively, which have their own AI guidance developing in parallel. However the UAE AI Charter applies federally. Entities with dual onshore/free-zone operations must manage compliance across jurisdictions. This guide represents the CBUAE baseline; monitor FSRA and DFSA publications in addition.

### 7.3 Fintech-Specific Proportionality

Proportionality is explicitly recognised in CBUAE's approach. It applies to **how** requirements are met — not **whether** they are met. A fintech with one AI credit scoring model still needs a documented model, a validation (external if needed), a monitoring plan, a consumer disclosure, and a governance mechanism (CEO/board in small entities).

**Always document proportionality decisions explicitly — examiners will ask.**

### 7.4 Generative AI Specific Controls

GenAI (LLMs for customer service, document generation, financial advice, compliance) is explicitly in scope. Additional required controls:

| Risk | Required Control |
|------|-----------------|
| Hallucination | Output filtering; human-in-loop for consequential outputs; disclose AI-generated content |
| Prompt injection | Security testing for adversarial input manipulation |
| Data privacy in prompts | Govern what customer data enters LLM prompts; assess third-party API data flows |
| Vendor LLM dependency | Full vendor AI due diligence; audit rights; model version change notification in contracts |
| Model drift | Re-evaluation as underlying LLM versions change |

### 7.5 AML and Fraud AI Considerations

AML transaction monitoring and fraud detection systems are **Tier 1 models**. Specific considerations:
- Alert suppression rates and false positive/negative rates are model performance metrics — monitor them
- Human analyst review of AI-generated alerts is the "human oversight" mechanism — formally document it
- Model threshold adjustments and retraining are material changes requiring change management and re-validation
- CBUAE FIU requirements on SAR filing: AI cannot file SARs autonomously — human review and sign-off is mandatory

### 7.6 Interaction with UAE Personal Data Protection Law (PDPL)

Federal Decree-Law No. 45 of 2021 intersects with AI governance at every stage:

| PDPL Requirement | AI Implementation Action |
|-----------------|--------------------------|
| Lawful basis for processing | Document consent / contract / legitimate interest basis for all training data |
| Purpose limitation | Training data must only be used for the stated model purpose |
| Data minimisation | Feature selection must minimise personal data use |
| Individual rights (access, correction, erasure) | Must be technically operable on training data and inference records |
| Automated decision-making | Right to human review aligns with Guidance Note Pillar 2 |
| Cross-border data transfers | Assess and approve all cross-border model training / inference data flows |

---

## 8. Glossary

| Term | Definition |
|------|-----------|
| **CBUAE** | Central Bank of the United Arab Emirates |
| **LFI** | Licensed Financial Institution — any entity licensed by CBUAE |
| **MMS** | Model Management Standards — CBUAE Rulebook standard for model governance |
| **Guidance Note** | CBUAE Guidance Note on Consumer Protection and Responsible AI (February 2026) |
| **AI Charter** | UAE Charter for the Development and Use of AI (June 2024) |
| **Model** | Any quantitative method processing data to produce outputs used in business decisions |
| **Tier 1 Model** | High-impact, complex model requiring full independent validation and Board oversight |
| **Tier 2 Model** | Medium-impact model requiring validation and Senior Management oversight |
| **Tier 3 Model** | Low-impact model requiring periodic documented review |
| **Model Inventory** | Central register of all models in use, development, or recently decommissioned |
| **RAO** | Responsible AI Officer — named Senior Management accountable for AI governance |
| **PSI** | Population Stability Index — measures distributional shift in model input data |
| **KS Statistic** | Kolmogorov-Smirnov — measures model discrimination power |
| **Gini / AUC** | Model performance metrics measuring ranking/discrimination ability |
| **XAI** | Explainable AI — methods enabling human-understandable AI decision explanations |
| **PDPL** | UAE Personal Data Protection Law (Federal Decree-Law No. 45 of 2021) |
| **ADGM** | Abu Dhabi Global Market — financial free zone regulated by FSRA |
| **DIFC** | Dubai International Financial Centre — financial free zone regulated by DFSA |
| **FSRA** | Financial Services Regulatory Authority (ADGM regulator) |
| **DFSA** | Dubai Financial Services Authority (DIFC regulator) |
| **FIU** | Financial Intelligence Unit (CBUAE) |
| **SAR** | Suspicious Activity Report |
| **TPRM** | Third-Party Risk Management |
| **GenAI / LLM** | Generative AI / Large Language Model |
| **Proxy Discrimination** | Indirect discrimination via variables statistically correlated with protected characteristics |
| **Four-Eyes Principle** | Requirement for independent review by a person not involved in original work |
| **CSI** | Characteristic Stability Index — measures stability of model feature distributions |

---

## 9. Board Briefing Card

See **[BOARD-BRIEFING.md](./BOARD-BRIEFING.md)** for the full one-page briefing.

### 30-Second Executive Summary

> The CBUAE now requires every licensed financial institution deploying AI to have: **(1)** a named Senior Manager accountable for AI, **(2)** a complete inventory of all AI/ML models, **(3)** independent validation of high-impact models, **(4)** consumer disclosures and human override mechanisms, and **(5)** ongoing bias monitoring. These are examination requirements **in effect now** — not future aspirations.

### Three Questions Every Board Must Ask Management

1. *"Show me our Model Inventory — how many AI systems do we operate, and which are Tier 1 high-impact?"*
2. *"Which Tier 1 models have had independent validation in the last 12 months — and what did validation find?"*
3. *"How do we tell customers that AI made a decision affecting them, and what is their recourse?"*

---

## 📌 Regulatory Watch

Monitor for updates from:
- [CBUAE Publications](https://www.cbuae.gov.ae) — new circulars, examination findings, updated guidance
- [UAE AI Office](https://ai.gov.ae) — national AI strategy updates, Charter amendments
- [FSRA (ADGM)](https://www.fsra.ae) — if operating in Abu Dhabi Global Market
- [DFSA (DIFC)](https://www.dfsa.ae) — if operating in Dubai International Financial Centre

---

## Disclaimer

This guide is for informational and educational purposes only. It does not constitute legal or regulatory advice. Institutions should obtain independent legal and compliance counsel tailored to their specific circumstances. Regulatory requirements may change — always verify against the latest official CBUAE publications.

---

*Published: April 2026 | License: CC0-1.0 (Public Domain) | Maintained by: [Ankit Uniyal](https://github.com/Ankit-Uniyal)*
