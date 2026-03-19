# Software Requirements Specification Review Report

## Table of Contents

> [!NOTE]
> Update this table of contents to reflect the sections in this document.
>      In the MkDocs web view, the table of contents is generated automatically in the sidebar.
>      This section is intended for printed or exported (PDF) versions of the document.
>
> 1. IDENTIFICATION
>    1.1 Document Overview
>    1.2 Abbreviations and Glossary
>    1.3 References
>    1.4 Conventions
> 2. REVIEW CONTEXT
>    2.1 Document Under Review
>    2.2 Review Team
>    2.3 Review Process
> 3. REVIEW CHECKLIST
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-SRS-RR-001 --> |
| Title | Software Requirements Specification Review Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal review of the Software Requirements Specification (SRS) for the <!-- TODO: project name --> software development project.

The purpose of this review is to verify that the SRS meets the quality criteria required by IEC 62304 §5.2 before the software design phase begins. The review covers requirement uniqueness, unambiguity, consistency, testability, SOUP-related requirements, risk management traceability, and alignment with upstream system requirements.

**Scope:** This review report covers the SRS identified in §2.1. It does not assess the correctness of the requirements against clinical or user needs — that is covered by the system-level validation activities.

**Intended audience:** Software quality assurance, software project manager, regulatory affairs, design review board.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Document Under Review

| Field | Value |
|---|---|
| Document Title | Software Requirements Specification |
| Document ID | <!-- TODO: e.g. PRJ-SRS-001 --> |
| Version Reviewed | <!-- TODO: e.g. 1.0 --> |
| Date of Version | <!-- TODO: YYYY-MM-DD --> |

### 2.2 Review Team

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| <!-- TODO: Add rows as needed --> | | | |

> [!NOTE]
> The author of the SRS should not act as review chair. At least one reviewer should be independent of the software development team (e.g. quality assurance or regulatory affairs).

### 2.3 Review Process

> [!NOTE]
> **IEC 62304 §5.2.6**
> IEC 62304 requires that software requirements be reviewed for correctness, consistency, completeness, feasibility, and testability before proceeding to the design phase. The criteria in §3 operationalise this requirement.

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. System Requirements Specification PRJ-SYRS-001 v1.0, Risk Management Plan PRJ-RMP-001 v1.0 --> |

## 3. REVIEW CHECKLIST

> [!NOTE]
> For each criterion, record the verdict and, if the criterion is not fully satisfied, create a finding in §4.
>
> **Verdict codes:**
>
> - **OK** — criterion is fully satisfied
> - **MINOR** — criterion is partially satisfied; a finding is raised but does not block approval
> - **MAJOR** — criterion is not satisfied; a finding is raised and must be resolved before approval
> - **N/A** — criterion is not applicable to this project (provide justification)

### 3.1 Requirement Identification and Uniqueness

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-01 | Each software requirement has a unique identifier that distinguishes it from all other requirements in the SRS. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |

### 3.2 Unambiguity

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-02 | Each requirement admits only one interpretation; it is free from ambiguous terms (e.g. "fast", "easy", "appropriate", "etc."). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-03 | Software requirements are expressed in unambiguous, precise technical language. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.3 Consistency

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-04 | There are no contradictions or conflicts between software requirements (within the SRS or with referenced upstream documents). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.4 SOUP Requirements

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-05 | Software requirements that are supported by, or dependent on, SOUP items are explicitly defined and identified in the SRS. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-06 | Requirements specific to the proper functioning of each SOUP within the software system are defined (e.g. SOUP version, configuration, known anomalies, integration constraints). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

> [!NOTE]
> **IEC 62304 §5.2.3 and §8.1.2**
> IEC 62304 requires that software requirements identify the use of SOUP and that requirements for the SOUP's correct functioning in the system are established.

### 3.5 Testability

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-07 | Each software requirement is testable, with objective and measurable acceptance criteria (pass/fail conditions free from subjective judgement). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-08 | Each requirement specifies or implies a verification method (test, inspection, demonstration, or analysis). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.6 Feasibility

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-09 | The feasibility of implementing each requirement is ensured, taking into account design constraints, operational environment, and maintenance considerations. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.7 Traceability

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-10 | Each software requirement is traceable to at least one upstream source: a system requirement, user need, regulatory requirement, risk control, or other documented source. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-11 | System or product requirements are fully taken into account and reflected in the SRS (no upstream requirement is left without a corresponding software requirement or explicit justification for exclusion). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.8 Risk Management

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-12 | Requirements derived from risk management activities (ISO 14971 risk controls) are identified and included in the SRS. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.9 System Requirements Alignment

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-13 | System requirements have been re-evaluated in light of the SRS, and any necessary updates to the system requirements have been made and documented. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved and the SRS updated before approval of the SRS
> - **MINOR** — should be resolved; may be deferred to next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Requirement ID(s) Affected | Owner | Resolution | Status |
|---|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. RC-02 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: e.g. SRS-FUN-003 --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO: e.g. 13 --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. The SRS is approved and the software design phase may proceed.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision of the SRS. The software design phase may proceed provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "SRS-FUN-003 must be reworded to remove ambiguity before v1.1 is issued."

**NOT APPROVED** — One or more MAJOR findings remain open. The SRS must be updated and re-reviewed before the software design phase begins.

### 5.3 Approval Signatures

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Software Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Quality Assurance | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
