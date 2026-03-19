# Software Unit Implementation and Verification Review Report

> [!NOTE]
> **Applicability by software safety class**
> **This review document is required for Class C software only.** For Class A and Class B software, a formal review of unit implementation and unit verification is optional; those classes may rely on less formal oversight methods as long as records exist.

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
>    2.1 Artifacts Under Review
>    2.2 Review Team
>    2.3 Review Process
> 3. REVIEW CHECKLIST
>    3.1 Software Unit Implementation
>    3.2 Unit Verification Procedures and Acceptance Criteria
>    3.3 Unit Verification Execution
>    3.4 Traceability
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-SUIV-RR-001 --> |
| Title | Software Unit Implementation and Verification Review Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal review of software unit implementation and unit verification activities for the <!-- TODO: project name --> software development project.

The purpose of this review is to confirm that all software units have been implemented in accordance with the Software Design Specification and that unit verification has been performed for every software unit before integration begins. The review covers completeness of implementation, execution of unit verification procedures, satisfaction of acceptance criteria, and traceability from software units to unit test records.

**Scope:** This review report covers the software units and unit test records identified in §2.1. It does not assess the correctness of the detailed design itself — that is covered by the Software Design Specification Review Report.

**Intended audience:** Software quality assurance, software project manager, regulatory affairs, design review board.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Artifacts Under Review

> [!NOTE]
> This review covers two categories of artifact: the software unit implementation and the unit verification records. Both must be identified below.

**Software Unit Implementation**

| Field | Value |
|---|---|
| Artifact | Source code / software units |
| Reference (e.g. repository, release tag, or document ID) | <!-- TODO: e.g. git tag v1.0 at https://github.com/org/repo, or PRJ-SRC-001 --> |
| Version / Revision | <!-- TODO: e.g. v1.0 / commit abc1234 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |

**Unit Verification Records**

| Field | Value |
|---|---|
| Document Title | <!-- TODO: e.g. Software Unit Test Report --> |
| Document ID | <!-- TODO: e.g. PRJ-UTR-001 --> |
| Version Reviewed | <!-- TODO: e.g. 1.0 --> |
| Date of Version | <!-- TODO: YYYY-MM-DD --> |

**Supporting Design Document**

| Field | Value |
|---|---|
| Document Title | Software Design Specification |
| Document ID | <!-- TODO: e.g. PRJ-SDS-001 --> |
| Version | <!-- TODO: e.g. 1.0 --> |

### 2.2 Review Team

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| <!-- TODO: Add rows as needed --> | | | |

> [!NOTE]
> The developer(s) who implemented the software units should not act as review chair. At least one reviewer should be independent of the software development team (e.g. quality assurance or regulatory affairs).

### 2.3 Review Process

> [!NOTE]
> **IEC 62304 §5.5.1 and §5.5.5**
> IEC 62304 requires that each software unit be implemented and that unit verification be performed for every software unit before integration. The criteria in §3 operationalise these requirements.

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. Software Design Specification PRJ-SDS-001 v1.0, Software Design Specification Review Report PRJ-SDS-RR-001 v1.0 --> |

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

### 3.1 Software Unit Implementation

> [!NOTE]
> **IEC 62304 §5.5.1**
> Each software unit defined in the detailed design shall be implemented. The implementation shall conform to the design specification and to any applicable coding standards.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-01 | Every software unit defined in the Software Design Specification has a corresponding implementation — no unit from the design is absent from the codebase. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |
| RC-02 | Each software unit is implemented in accordance with its specification in the SDS (interface, behaviour, algorithms, data structures, and error handling). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-03 | The implementation conforms to the applicable coding standards or guidelines referenced in the Software Development Plan. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-04 | No software unit has been added to the implementation that is not defined in the SDS or formally recorded as a design change. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.2 Unit Verification Procedures and Acceptance Criteria

> [!NOTE]
> **IEC 62304 §5.5.2 and §5.5.3**
> Before unit verification is performed, verification procedures and acceptance criteria shall be established for each software unit. Acceptance criteria shall be based on the unit's specified interfaces, inputs, outputs, and functional behaviour.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-05 | Verification procedures (test cases, test scripts, or inspection checklists) exist for every software unit. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-06 | Acceptance criteria are defined for each software unit and are based on the unit's specified behaviour and interfaces in the SDS. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-07 | Acceptance criteria are objective and measurable — each criterion has an unambiguous pass/fail condition. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

> [!NOTE]
> Assert statements and equivalent pass/fail mechanisms in automated test frameworks (e.g. `assertEqual`, `assertRaises`, matcher libraries) satisfy the unambiguous pass/fail condition required by RC-07.

### 3.3 Unit Verification Execution

> [!NOTE]
> **IEC 62304 §5.5.5**
> Unit verification shall be performed for each software unit. The results shall be recorded and the software unit shall meet its acceptance criteria before it is integrated.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-08 | Unit verification has been executed for every software unit — no unit has been left unverified. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-09 | The unit verification results are recorded, with each test case linked to its outcome (pass/fail) and the version of the unit under test. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-10 | All software units meet their acceptance criteria — no unit has a recorded failing test without a documented resolution. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-11 | Any anomalies or failures detected during unit verification are recorded in the problem resolution system and their impact assessed before the unit is accepted. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-12 | For Class C software: unit acceptance criteria address all additional aspects required by IEC 62304 §5.5.4. For Class A and Class B software: mark N/A with justification. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

> [!NOTE]
> **RC-09 — Automated test logs**
> Output logs produced by automated test frameworks (e.g. JUnit XML reports, pytest output, TAP files) are accepted as unit verification result records, provided they identify the test case, the outcome (pass/fail), and the version of the software under test.

> [!NOTE]
> **RC-11 — Anomaly records during coding**
> Anomalies discovered while coding a software unit do not require a formal anomaly ticket to be opened in the problem resolution system. A ticket is required only when a unit test fails at the point the unit is submitted for integration or verification; at that stage the unit is considered not yet accepted and the failure must be tracked to closure.

### 3.4 Traceability

> [!NOTE]
> **IEC 62304 §5.5.5**
> The relationship between software units and their verification records shall be traceable so that each unit can be shown to have been verified.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-13 | Every software unit is traceable to at least one unit verification record (test case, test script, or inspection record) in the unit test documentation. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-14 | Every unit verification record is traceable back to a software unit — no orphaned test cases exist that do not map to a defined unit. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-15 | The traceability from software units to unit verification records is consistent with the traceability matrix or linkage maintained in the unit test documentation. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved before the software units are accepted and integration begins
> - **MINOR** — should be resolved; may be deferred to next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Software Unit(s) Affected | Owner | Resolution | Status |
|---|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. RC-08 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: e.g. Unit X, Module Y --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO: e.g. 15 --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. All software units are implemented and verified; the integration phase may proceed.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision of the affected artifacts. The integration phase may proceed provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "Unit X failing test for error path must be resolved before that unit is integrated."

**NOT APPROVED** — One or more MAJOR findings remain open. The identified software units must be corrected and/or re-verified before integration begins.

### 5.3 Approval Signatures

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Software Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Quality Assurance | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
