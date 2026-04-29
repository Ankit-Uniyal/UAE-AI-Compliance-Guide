# Changelog: UAE AI Compliance Guide

All notable changes to this guide are documented here.

Format: `[Version] — Date — Summary`

Frameworks monitored for updates:
- CBUAE Publications: https://www.cbuae.gov.ae
- UAE AI Office: https://ai.gov.ae
- Insurance Authority UAE: https://ia.gov.ae
- FSRA (ADGM): https://www.fsra.ae
- DFSA (DIFC): https://www.dfsa.ae

---

## [v1.1] — April 2026

### Summary
Quality review and gap-fix release. Six substantive issues identified in v1.0 have been addressed. No new regulatory instruments were published between v1.0 and v1.1 — all changes are quality improvements to the guide itself.

### Changes by File

#### README.md
- **Fixed:** Regulatory hierarchy diagram corrected. The v1.0 diagram incorrectly implied a simple top-down stack (Charter → MMS → Guidance Note) suggesting the Guidance Note was "below" the MMS in regulatory authority. The v1.1 diagram accurately shows the MMS and Guidance Note as parallel instruments, with the Charter as an overarching ethical foundation that both draw upon. Added explanatory note distinguishing legal hierarchy from examination priority.
- **Added:** Section 3 — High-Impact AI Decision Definition. A new standalone section providing: (1) a five-criteria definition of "high-impact" (financial access, financial terms, regulatory consequence, customer relationship, scale threshold); (2) a decision tree for borderline cases; (3) a classification table for 12 common use cases; (4) documentation requirements for the classification itself.
- **Added:** Section 8.7 — Bancassurance and Insurance-Adjacent AI. New section noting that LFIs with bancassurance or embedded insurance operations face a parallel AI governance layer from the Insurance Authority of the UAE (IA), and that this guide covers only the CBUAE frameworks.
- **Added:** Insurance Authority (IA) to the Regulatory Watch list.
- **Updated:** Scope table to include bancassurance/insurance-adjacent operations.
- **Updated:** Glossary with new terms: High-Impact AI Decision, D-SIB, Insurance Authority (IA).
- **Updated:** Artefacts Library — added Item 6 (High-Impact AI Decision Classification per model) as a required document. Items renumbered accordingly (previously 20 artefacts; now 21).
- **Updated:** Board Briefing Card to reference high-impact classification in the three board questions.
- **Updated:** Phase summary timeline note added: timelines are calibrated for proportionate institutions; large banks should plan 18–24 months.
- **Added:** Version header (v1.1) and "Last Reviewed Against Frameworks" date.

#### FRAMEWORK-MAPPING.md
- **Fixed:** Framework architecture description corrected to align with README.md v1.1 — parallel instrument relationship, not a vertical hierarchy. Added table showing distinct function and legal nature of each framework.
- **Fixed:** Regulatory hierarchy section (Section 4) updated with an explanatory note clarifying that the Guidance Note's position at "conflict resolution priority 1" reflects current examination priority, not legislative supremacy over the MMS.
- **Added:** "High-Impact AI Decision classification" as a new row in the Master Requirements Matrix (Section 1) — CRITICAL priority, Guidance Note mandatory.
- **Updated:** Proportionality Map (Section 5) — removed the specific "AED 20Bn assets" threshold, which was not a CBUAE-defined regulatory category. Replaced with institution-type descriptions (D-SIB/Large Bank, Mid-size Bank, Small Bank/Finance Co., Regulated Fintech) with a clear note that these are illustrative and proportionality should be based on actual risk profile, not balance sheet alone.
- **Updated:** Section 2.2 (MMS unique obligations) — added "Proportionate Tier 2 validation" as a distinct obligation, noting that the definition of "proportionate" must be codified in the Model Risk Management Policy.
- **Added:** Bancassurance/Insurance Authority row in Master Requirements Matrix.
- **Added:** Version header (v1.1).

#### IMPLEMENTATION-ROADMAP.md
- **Added:** "Timeline Calibration by Institution Size" section at the top of the document — a table showing realistic compliance timelines for four institution types (Fintech, Small Bank, Mid-size Bank, D-SIB/Large Bank) across all three phases. Replaces the implicit assumption that all institutions follow the same schedule.
- **Added:** Validation capacity planning note — explicit guidance that a single complex ML model validation takes 4–8 weeks; large institutions with 20+ Tier 1 models need multiple validators or phased external engagement; the validation queue plan is a critical path document.
- **Added:** Board meeting cycle note — the "Board Policy by Month 3" milestone may not be achievable if no board meeting falls in that window; interim Board Risk Committee approval is a valid alternative.
- **Replaced:** Workstream 1.3 (previously a simple gap assessment) — fully replaced with the 5-Question Tiering Decision Framework. The framework provides five sequential questions with thresholds, a tiering scorecard table, documentation requirements, and a worked action plan with evidence columns. Tier 1 is triggered by any "Yes" to questions 1–3; Tier 2 by questions 4–5; Tier 3 otherwise.
- **Updated:** Workstream 2.3 — added validation queue planning action (2.3.2) and capacity planning note.
- **Updated:** Workstream 2.1 — added 5-question tiering framework as explicit content of the Model Risk Management Policy.
- **Updated:** Key Milestones Summary — expanded to three-column table showing timelines for Fintech/Small Bank, Mid-size Bank, and Large Bank/D-SIB separately.
- **Added:** Internal Audit action 3.1.4 — Tiering Decision Framework consistency audit (are models correctly tiered?).
- **Added:** Training content for Senior Management and developers updated to include tiering criteria and high-impact classification.
- **Updated:** Regulatory watch list to include Insurance Authority UAE.
- **Added:** Version header (v1.1).

#### AUDIT-CHECKLIST.md
- **Reclassified:** DA2 (Training data quality assessment) upgraded from 🟠 HIGH to 🔴 CRITICAL. Rationale: training data quality is a core validation input; absence directly undermines the validity of any validation report and is a first-order examination finding.
- **Reclassified:** DA3 (Lawful basis for training data under UAE PDPL) upgraded from 🟠 HIGH to 🔴 CRITICAL. Rationale: using personal data without a documented lawful basis is a PDPL enforcement risk independent of AI governance; CBUAE examiners increasingly coordinate with data protection reviews.
- **Reclassified:** DA5 (Cross-border data transfer assessment) upgraded from 🟠 HIGH to 🔴 CRITICAL. Rationale: the majority of UAE institutions use foreign cloud providers; without a transfer assessment, the institution has an undocumented PDPL and CBUAE data governance exposure affecting every cloud-based AI deployment.
- **Updated:** Summary Dashboard — Domain 9 CRITICAL count updated from 0 to 3; total CRITICAL count updated from 40 to 43.
- **Clarified:** V3 (Tier 2 validation) — reworded to specify "proportionate depth as defined in Model Risk Policy" and added a note explaining that Tier 2 validation may be lighter-touch than Tier 1, but "proportionate" must be defined in policy and the report must still reach a formal opinion.
- **Updated:** I3 (Model Inventory record completeness) — added "high-impact classification" as a required inventory field.
- **Added:** IA4 (new control) — Tiering consistency audit: are models correctly tiered using the documented framework?
- **Updated:** Examiner Focus Areas — added items 8 (training data quality for Tier 1) and 9 (cross-border data flows for cloud AI).
- **Updated:** Preparation tip — references 21 key artefacts (up from 20).
- **Added:** Explanatory notes below DA2, DA3, DA5 and Domain 10 explaining the rationale for priority ratings.
- **Added:** Version header (v1.1) and v1.1 change summary note at the top.

#### BOARD-BRIEFING.md
- **Fixed:** Removed reference to "AED 20Bn assets" threshold in the proportionality context — this was an illustrative number not based on any CBUAE-defined regulatory category and could have misled institutions near that threshold.
- **Updated:** "What the Board Is Personally Responsible For" — added note that examiners check Board minutes for evidence of active challenge (not just noting) of AI risk.
- **Updated:** "Five Things Every Board Member Must Know" — Item 1 now includes high-impact classification as a required element of the Model Inventory, not just the inventory itself.
- **Updated:** Question 1 red flags — added "No high-impact classification column" and "Vendor AI systems are not included" as explicit red flags.
- **Updated:** Question 2 red flags — added "Fairness/bias testing was not part of validation scope."
- **Updated:** Examination Risk Assessment table — added two new rows: (a) No training data quality documentation and (b) No cross-border data transfer assessment (cloud AI), both rated HIGH with Urgent timelines.
- **Updated:** Board Resolution — added Item 6 directing management to present a size-calibrated implementation plan; added reference to IMPLEMENTATION-ROADMAP.md; added timeline realism note.
- **Updated:** "Where to Read More" — added CHANGELOG.md.
- **Added:** Clarifying note that all three frameworks are parallel instruments (not hierarchical) in the "What Has Been Issued" section.
- **Added:** Version header (v1.1).

#### CHANGELOG.md (this file)
- **Created:** New file. Tracks all material changes to the guide by version, file, and rationale. Provides a regulatory watch list for ongoing monitoring.

---

## [v1.0] — April 2026

### Summary
Initial publication of the UAE AI Compliance Guide.

### Files Published
- README.md — Full 9-part guide covering all three frameworks, implementation overview, artefacts library, UAE-specific considerations, glossary, and board briefing card
- FRAMEWORK-MAPPING.md — 47-row cross-framework requirements matrix, unique obligations per framework, convergence points, regulatory hierarchy, proportionality map
- IMPLEMENTATION-ROADMAP.md — 3-phase phased plan with 7 workstreams, 60+ action items, owners, timelines, and milestones summary
- AUDIT-CHECKLIST.md — 70 controls across 10 domains with evidence requirements, priority ratings, and examiner focus areas
- BOARD-BRIEFING.md — Board-level 5-minute briefing with five things every board member must know, three questions for management, examination risk assessment, and board resolution template
- LICENSE — CC0-1.0 (Public Domain)

### Frameworks Covered at v1.0
- CBUAE Guidance Note on Consumer Protection and Responsible AI (February 2026)
- CBUAE Rulebook: Big Data Analytics and AI — Model Management Standards (in force)
- UAE AI Charter (June 2024)

---

## Regulatory Watch Log

| Date | Source | Update Type | Impact on Guide | Action Taken |
|------|--------|-------------|-----------------|--------------|
| April 2026 | — | Guide published (v1.0) | — | Initial publication |
| April 2026 | — | Quality review (v1.1) | Six gaps addressed | Updated all files |
| *[future]* | CBUAE | *[new circular/guidance]* | *[TBD]* | *[TBD]* |

---

## How to Contribute or Flag Issues

If you identify an error, a missing requirement, or a new regulatory development that should be reflected in this guide:
1. Open a GitHub Issue describing the change needed
2. Reference the specific framework section and regulatory source
3. A pull request with the proposed change is welcome

---

*Maintained by [Ankit Uniyal](https://github.com/Ankit-Uniyal) | License: CC0-1.0 | For UAE Banking & Fintech AI Compliance*
