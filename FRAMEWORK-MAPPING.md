# Framework Mapping: UAE AI Compliance for Banking & Fintech

> **Version: 1.1 | Last Reviewed: April 2026**
> Cross-reference matrix for CBUAE Guidance Note on Responsible AI, CBUAE Model Management Standards Rulebook, and UAE AI Charter

---

## How the Three Frameworks Relate (Corrected Architecture)

The three frameworks are **parallel and complementary instruments**, not a simple top-down hierarchy. Understanding their distinct functions prevents both over-reliance on one instrument and gaps from assuming one covers the others.

| Framework | Function | Legal Nature | Examiner Use |
|-----------|----------|-------------|--------------|
| **UAE AI Charter** | National ethical values & principles | Policy document; referenced by all regulators | Basis for board-level policy expectations; increasingly cited in examinations |
| **CBUAE MMS Rulebook** | Model lifecycle governance — development, validation, monitoring, documentation | Binding Rulebook standard (mandatory) | Primary instrument for model risk examinations; establishes operational standards |
| **CBUAE Guidance Note (Feb 2026)** | Consumer-facing AI obligations — human oversight, explainability, fairness, disclosure | Supervisory guidance (examination expectation) | Highest current examination priority as the most recently issued instrument; drives consumer protection findings |

**Relationship:** The Charter informs and is incorporated into both operational instruments. The MMS and Guidance Note are parallel — neither is subordinate to the other. The MMS governs model governance broadly; the Guidance Note overlays consumer protection obligations specifically for AI decisions affecting customers.

**Conflict resolution priority:** Guidance Note (consumer protection; most recent; highest current examiner focus) → MMS (operational model standard) → Charter (ethical baseline; shapes interpretation).

---

## 1. Master Requirements Matrix

This matrix maps every major requirement domain to its applicable framework(s). Use this to eliminate duplication and identify compliance gaps.

**Priority key:** 🔴 CRITICAL (examination finding if missing) | 🟠 HIGH (significant finding) | 🟡 MEDIUM (noted finding) | 🟢 LOW/Emerging

| Requirement Domain | CBUAE Guidance Note (Feb 2026) | CBUAE MMS Rulebook | UAE AI Charter (June 2024) | Priority |
|---|---|---|---|---|
| Board ultimate accountability for AI | ✅ Mandatory | ✅ Mandatory | ✅ Principle 6 | 🔴 CRITICAL |
| AI/Model Governance Committee | ✅ Required | ✅ Required | Referenced | 🔴 CRITICAL |
| Named Responsible AI Officer (RAO) | ✅ Required | Implied via roles | Referenced | 🔴 CRITICAL |
| Board-level AI risk reporting | ✅ Min. annual | ✅ Required | Referenced | 🔴 CRITICAL |
| High-Impact AI Decision classification | ✅ Mandatory | Referenced | — | 🔴 CRITICAL |
| Model Inventory (central register) | Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Model Risk Tiering (3-tier minimum) | Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Model Concept Document | Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Model Development Document | Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Independent Model Validation (T1/T2) | Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Validation Report with formal opinion | — | ✅ Mandatory | — | 🔴 CRITICAL |
| Validation Finding Tracker | — | ✅ Mandatory | — | 🔴 CRITICAL |
| Model Operational Manual | — | ✅ Mandatory | — | 🔴 CRITICAL |
| Model Monitoring Plan | ✅ Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Performance drift monitoring (PSI/KS) | Referenced | ✅ Mandatory | — | 🔴 CRITICAL |
| Human override capability for high-impact AI | ✅ Mandatory | Referenced | Principle 1 | 🔴 CRITICAL |
| Customer right to request human review | ✅ Mandatory | — | Principle 1 | 🔴 CRITICAL |
| Explainability — Technical (for examiners) | ✅ Mandatory | ✅ In all model docs | Principle 4 | 🔴 CRITICAL |
| Explainability — Consumer (plain language) | ✅ Mandatory | Referenced | Principle 4 | 🔴 CRITICAL |
| Pre-deployment bias / fairness testing | ✅ Mandatory | ✅ In validation | Principle 5 | 🔴 CRITICAL |
| Ongoing fairness monitoring | ✅ Mandatory | ✅ In monitoring | Principle 5 | 🔴 CRITICAL |
| Protected characteristics excluded as features | ✅ Mandatory | ✅ Dev standards | Principle 5 | 🔴 CRITICAL |
| Training data quality assessment | ✅ Referenced | ✅ Mandatory | Principle 3 | 🔴 CRITICAL |
| Training data lineage documentation | ✅ Referenced | ✅ Mandatory | Principle 3 | 🔴 CRITICAL |
| Lawful basis for training data (UAE PDPL) | ✅ Referenced | Referenced | ✅ Principle 3 | 🔴 CRITICAL |
| Consumer AI disclosure (at point of interaction) | ✅ Mandatory | — | Principle 4 | 🟠 HIGH |
| AI chatbot identification requirement | ✅ Mandatory | — | Principle 4 | 🟠 HIGH |
| Adverse decision notification to customer | ✅ Mandatory | — | Principle 1 | 🟠 HIGH |
| AI complaints category in complaints system | ✅ Mandatory | — | Principle 1 | 🟠 HIGH |
| Customer redress for AI-caused harm | ✅ Mandatory | — | Principle 1 | 🟠 HIGH |
| UAE PDPL compliance in AI pipelines (broadly) | ✅ Referenced | Referenced | ✅ Principle 3 | 🟠 HIGH |
| Third-party / vendor AI inventory | ✅ Mandatory | Referenced | — | 🟠 HIGH |
| Vendor AI risk assessment | ✅ Mandatory | Referenced | — | 🟠 HIGH |
| Vendor contract: audit rights | ✅ Mandatory | — | — | 🟠 HIGH |
| Vendor contract: explainability obligations | ✅ Mandatory | — | Principle 4 | 🟠 HIGH |
| Vendor contract: exit / replacement provisions | ✅ Mandatory | — | — | 🟠 HIGH |
| Vendor contract: model change notification | ✅ Mandatory | Referenced | — | 🟠 HIGH |
| Model Change Management process | — | ✅ Mandatory | — | 🟠 HIGH |
| Material change re-validation requirement | — | ✅ Mandatory | — | 🟠 HIGH |
| Proxy discrimination analysis | ✅ Mandatory | ✅ In validation | Principle 5 | 🟠 HIGH |
| Bias remediation escalation (with SLA) | ✅ Mandatory | Referenced | — | 🟠 HIGH |
| Cross-border data transfer assessment | ✅ Referenced | Referenced | Principle 3 | 🟠 HIGH |
| AI stress testing | Referenced | ✅ In validation | Principle 2 | 🟡 MEDIUM |
| Model Decommissioning process | — | ✅ Mandatory | — | 🟡 MEDIUM |
| Monitoring results to governance committee | ✅ Referenced | ✅ Mandatory | — | 🟡 MEDIUM |
| AI complaints reported to governance | ✅ Mandatory | — | — | 🟡 MEDIUM |
| AI inclusivity for underserved populations | Referenced | — | ✅ Principle 8 | 🟡 MEDIUM |
| Training programme (staff + board) | Referenced | Referenced | Referenced | 🟡 MEDIUM |
| Regulatory change management process | Referenced | Referenced | Referenced | 🟡 MEDIUM |
| GenAI hallucination controls | ✅ Referenced | ✅ Model risk | Principle 2 | 🟡 MEDIUM |
| Bancassurance AI (Insurance Authority overlay) | ⚡ Partial (CBUAE scope) | ⚡ Partial (CBUAE scope) | Referenced | 🟡 MEDIUM |
| ESG / Sustainability in AI operations | — | — | ✅ Principle 7 | 🟢 LOW/Emerging |

---

## 2. Framework-by-Framework Unique Obligations

### 2.1 Obligations Unique to CBUAE Guidance Note on Responsible AI

These requirements appear **only** in the Guidance Note and have no direct equivalent in the MMS or Charter:

| Requirement | Detail |
|-------------|--------|
| High-Impact AI Decision classification | Institutions must formally classify which AI systems constitute high-impact decisions and document the rationale |
| Consumer AI disclosure at point of interaction | Customers must be told they are interacting with an AI at the moment of interaction — not just in product terms |
| AI chatbot / virtual assistant identification | Chatbots must identify themselves as AI at session start |
| Individual right to request human review | Each customer has the right to ask for a human to review any high-impact AI decision affecting them |
| Human review SLA and logging | The institution must document the process, turnaround time, and log all human review requests and outcomes |
| Adverse decision notification | Customers must be proactively notified when an AI made or materially influenced an adverse decision about them |
| AI complaints as named category | AI-related complaints must be a distinct, tracked category in the complaints system |
| Customer redress mechanism | A formal pathway must exist for customers harmed by AI decisions to obtain remedy |
| Vendor contract: audit rights | Contracts with AI vendors must give the LFI the right to audit the vendor model |
| Vendor contract: exit provisions | Contracts must allow the LFI to exit or replace a vendor AI system that fails governance standards |
| "Vendor-bought" defence explicitly rejected | Regulatory guidance explicitly states LFI responsibility cannot be passed to vendors |

### 2.2 Obligations Unique to CBUAE MMS Rulebook

These requirements appear **only** in the MMS and have no direct equivalent in the Guidance Note or Charter:

| Requirement | Detail |
|-------------|--------|
| Formal 3-tier model risk tiering | Documented tiering methodology assigning every model to Tier 1, 2, or 3 |
| Model Concept Document (pre-development) | Required before any model development begins |
| Model Development Document | Full technical specification including feature justification, selection rationale, test results |
| Validation Report with formal opinion | The opinion must be one of three explicit options: Approve / Approve with Conditions / Reject |
| Validation independence (four-eyes) | Structural separation between model development team and validation team |
| Proportionate Tier 2 validation | Tier 2 validation may be lighter-touch than Tier 1 — the institution must define in policy what "proportionate" means |
| Model Operational Manual | How-to guide for running, monitoring, and overriding the model in production |
| Model Change Log | Continuous log of all post-deployment changes |
| Model Change Management process | Defined workflow for material vs. minor model changes, including re-validation triggers |
| Model Decommissioning process | Formal process for retiring models — data retention, inventory update, decision archaeology |
| Population Stability Index (PSI) monitoring | Specific metrics for input distribution drift — not just outcome monitoring |

### 2.3 Obligations Unique to UAE AI Charter

These appear **only** in the Charter and are not directly codified in the MMS or Guidance Note:

| Requirement | Detail |
|-------------|--------|
| Environmental sustainability of AI | AI development and operation should consider environmental impact (Principle 7) |
| Inclusivity for underserved populations | AI must not exclude or disadvantage the financially underserved (Principle 8) |
| National AI strategic alignment | Board AI policy should explicitly align with UAE national AI strategy |
| Human wellbeing as design principle | AI must be designed to benefit individuals and society — not just comply with rules |

---

## 3. Convergence Points — Build Once, Satisfy All Three

The following requirements are addressed by all three frameworks. A single programme satisfying all three simultaneously is the most efficient compliance approach.

### 3.1 Governance Architecture (All Three)

**What all three require:** Named individual accountability; committee oversight; Board ultimate responsibility.

**Single solution:** Constitute an AI Governance Committee with documented ToR; designate a Responsible AI Officer at Senior Management level; ensure Board-level AI risk reporting. Formally adopt UAE AI Charter principles into the AI Policy document approved by the Board.

**Evidence that satisfies all three:** Board minutes with AI agenda item; AI Policy document referencing Charter; Governance Committee ToR and meeting minutes; RAO appointment letter.

### 3.2 Explainability Framework (All Three)

**What all three require:**
- Charter Principle 4: People know when AI is used and understand how it works
- MMS: Model documentation must capture methodology, assumptions, and limitations
- Guidance Note: Consumers receive plain-language explanations of adverse AI decisions

**Single solution:** Implement a two-tier explainability framework:
- *Tier A (Technical)*: XAI methods (SHAP, LIME, attention weights as appropriate) integrated into model validation and documentation
- *Tier B (Consumer)*: Standard explanation templates per model type, delivered automatically for adverse decisions and on request

**Evidence that satisfies all three:** Validation reports with explainability section; consumer explanation templates; process documentation for adverse decision notifications.

### 3.3 Fairness and Bias Programme (All Three)

**What all three require:**
- Charter Principle 5: AI treats people fairly; bias audits across demographic groups
- MMS Validation: Fairness testing as part of every T1/T2 validation
- Guidance Note: Pre-deployment testing AND ongoing monitoring; protected characteristic exclusions; proxy discrimination monitoring

**Single solution:** A Fairness Testing and Monitoring Framework covering:
- Defined protected characteristics for each model
- Defined fairness metrics per model type (demographic parity, equalised odds, predictive parity)
- Pre-deployment fairness testing integrated into validation checklist
- Post-deployment fairness monitoring integrated into model monitoring plan
- Escalation and remediation process for fairness findings

**Evidence that satisfies all three:** Fairness Testing Framework document; validation reports with fairness section; monitoring plan fairness metrics; escalation records.

---

## 4. Regulatory Hierarchy and Conflict Resolution

When requirements across frameworks appear to conflict, apply this hierarchy for **conflict resolution purposes**:

1. **CBUAE Guidance Note** — highest current examiner focus; consumer protection requirements; most recently issued (Feb 2026)
2. **CBUAE MMS Rulebook** — binding operational standard; model lifecycle requirements; foundational
3. **UAE AI Charter** — ethical and policy baseline; shapes interpretation; apply where more demanding than above

> **Note:** In practice, genuine conflicts between these instruments are rare — they are deliberately complementary. Where the Charter sets a higher standard than the MMS or Guidance Note on a specific point (e.g., inclusivity for underserved populations), aspire to meet the Charter standard, as regulatory expectations in that area are likely to harden.

> **Note on Guidance Note hierarchy:** The Guidance Note sitting at position 1 for *conflict resolution purposes* does not mean it is a higher-level instrument than the MMS in a legislative sense. The MMS is a binding Rulebook standard (formally superior in legal hierarchy). The positioning here reflects *current examination priority* — examiners are actively using the Feb 2026 Guidance Note as their primary assessment lens for consumer-facing AI. Both instruments must be fully satisfied.

---

## 5. Proportionality Map by Institution Type

| Institution Type | Tier 1 Model Approach | Governance Structure | Validation Approach | Third-Party AI |
|-----------------|----------------------|---------------------|--------------------|--------------------|
| **D-SIB / Large Bank** | Full standalone validation team; quarterly board reporting; dedicated RAO role; likely 20+ Tier 1 models; 18–24 month validation cycle for full coverage | Board AI Committee or Board Risk Committee with AI sub-agenda; stand-alone Model Risk function | Internal validation team; external specialist for highest-risk GenAI/ML Tier 1 models | Full TPRM integration; Legal review of all AI contracts; ongoing monitoring of vendor model versions |
| **Mid-size Bank** | Internal validation capability; senior management reporting; 10–20 Tier 1 models typical; 12–18 month cycle | AI risk embedded in Risk Committee; RAO = CRO or dedicated Head of Model Risk | Internal team (may share resources); external for models outside internal expertise | AI due diligence checklist; contract review; risk-rated vendor register |
| **Small Bank / Finance Co.** | Proportionate — justify and document; typically 3–10 Tier 1 models | RAO = CRO or CEO; governance via existing risk committee with AI standing agenda item | External validation acceptable and recommended for Tier 1 | Standard vendor AI risk questionnaire; legal review of material contracts |
| **Regulated Fintech** | Proportionate to model count; typically 1–5 Tier 1 models | RAO = CTO or CEO; board-level oversight; proportionality rationale documented | External validation; or structured internal peer review with documented independence | Third-party AI assessed per engagement; contract templates reviewed by Legal |

> **Proportionality note:** These categories are illustrative guidance — they are NOT CBUAE-defined regulatory tiers. Institutions should apply proportionality based on their actual model inventory, risk profile, and consumer impact — not balance sheet size alone. Critically: proportionality adjusts **how** requirements are met, never **whether** they apply.

---

*Version 1.1 | Last updated: April 2026 | Part of the [UAE AI Compliance Guide](./README.md) | See [CHANGELOG.md](./CHANGELOG.md)*
