# Software Design Specification Review Report

> [!NOTE]
> **Applicability by software safety class**
> **This review document is optional for Class A and Class B software** and may be merged into a single combined design review document together with the software architecture review.
>
> The level of detail required for software units differs by safety class:
>
> - **Class A and Class B** — Software units may be treated as **black boxes**: the review verifies that the units satisfy their specified interfaces and externally observable behaviour without requiring inspection of internal logic or implementation detail.
> - **Class C** — Software units shall be treated as **white boxes**: the review verifies that the internal structure, logic, algorithms, and data flows are specified in sufficient detail to implement and verify each unit unambiguously.

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
>    3.1 Correct Implementation of the Software Architecture
>    3.2 Consistency with the Software Architecture
>    3.3 Traceability from Architectural Software Items to Detailed Design Software Units [Optional]
>    3.4 Sufficient Detail for Implementation [Class C]
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-SDS-RR-001 --> |
| Title | Software Design Specification Review Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal review of the Software Design Specification (SDS) for the <!-- TODO: project name --> software development project.

The purpose of this review is to verify that the detailed design correctly and completely implements the software architecture before coding begins. The review covers the correct implementation of architectural software items through the definition of software units and their interactions, consistency of the detailed design with the architecture, traceability from architectural software items to detailed design software units, and — for Class C software — sufficient specification detail to implement each software unit and its interfaces.

**Scope:** This review report covers the SDS identified in §2.1. It does not re-assess the correctness of the software architecture itself — that is covered by the Software Architecture Review Report.

**Intended audience:** Software quality assurance, software project manager, regulatory affairs, design review board.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Document Under Review

| Field | Value |
|---|---|
| Document Title | Software Design Specification |
| Document ID | <!-- TODO: e.g. PRJ-SDS-001 --> |
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
> The author of the SDS should not act as review chair. At least one reviewer should be independent of the software development team (e.g. quality assurance or regulatory affairs).

### 2.3 Review Process

> [!NOTE]
> **IEC 62304 §5.4.3**
> IEC 62304 requires that the detailed design of each software item be reviewed for correctness and its ability to implement the software requirements before coding begins. The criteria in §3 operationalise this requirement.

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. Software Architecture Document PRJ-SAD-001 v1.0, Software Requirements Specification PRJ-SRS-001 v1.0, Software Architecture Review Report PRJ-SAD-RR-001 v1.0 --> |

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

### 3.1 Correct Implementation of the Software Architecture

> [!NOTE]
> **IEC 62304 §5.4.1**
> The detailed design shall correctly implement the software architecture by defining the parent software items as software units and specifying the interactions between those software units.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-01 | Each software item defined in the architecture is decomposed into one or more software units in the detailed design. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |
| RC-02 | The decomposition of each architectural software item into software units is complete — no part of an architectural software item is left unaddressed in the detailed design. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-03 | The interactions (data flows, control flows, events, calls, messages) between software units are specified and are consistent with the interactions defined between software items at the architectural level. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-04 | The interfaces between software units (inputs, outputs, pre-conditions, post-conditions, error handling) are defined for each unit. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-05 | The allocation of responsibility among software units is unambiguous — each functional or non-functional requirement allocated to an architectural software item can be clearly attributed to one or more specific software units. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.2 Consistency with the Software Architecture

> [!NOTE]
> **IEC 62304 §5.4.1**
> The specification of software units shall not contradict the software architecture. Any deviation from the architecture must be identified and the architecture updated accordingly before proceeding.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-06 | No software unit introduces behaviour, data flow, or dependency that contradicts the decomposition, partitioning, or constraints defined in the software architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-07 | Interfaces between software units that cross architectural boundaries (e.g. between layers, subsystems, or partitions) are consistent with the corresponding interface specifications in the architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-08 | Any SOUP items used at the unit level are already identified in the architecture; no new SOUP dependencies are introduced without a corresponding update to the architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-09 | Risk control measures allocated to architectural software items are preserved and not weakened by the decomposition into software units. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.3 Traceability from Architectural Software Items to Detailed Design Software Units [Optional]

> [!NOTE]
> **IEC 62304 §5.4.1 — traceability is recommended but not explicitly mandated**
> Although IEC 62304 does not explicitly require a traceability matrix between architectural software items and software units, documenting this traceability aids verification, change impact assessment, and regulatory inspection. This section may be marked N/A with justification if traceability is maintained by other means (e.g. a linked requirement management tool).

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-10 | A traceability mapping from each architectural software item to the software units that implement it is documented (e.g. in the SDS, in a traceability matrix, or in a linked tool). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-11 | The traceability mapping is complete — every architectural software item maps to at least one software unit, and every software unit maps back to at least one architectural software item. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-12 | The traceability mapping is consistent with the decomposition described in the detailed design — no discrepancies exist between the mapping and the design text or diagrams. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.4 Sufficient Detail for Implementation [Class C]

> [!WARNING]
> **IEC 62304 §5.4.2 — Class C software only**
> For Class C software, the detailed design shall specify each software unit in sufficient detail that the unit can be correctly implemented by a developer without requiring additional design decisions. This includes specifying algorithms, data structures, internal logic, and all unit interfaces.
>
> For Class A and Class B software, this section may be marked **N/A** with justification. Software units need only be specified to the level of their external interfaces and observable behaviour (black-box specification).

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-13 | Each software unit is described with sufficient detail that a developer can implement it without making design decisions — algorithms, logic, state transitions, and data structures are specified where relevant. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-14 | All interfaces of each software unit (function signatures, method parameters, return types, error codes, pre-conditions, post-conditions) are fully specified. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-15 | Memory, timing, and resource constraints relevant to each software unit are identified and specified where applicable. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-16 | Error detection and handling logic within each software unit is described, including how the unit responds to invalid inputs, resource failures, and exception conditions. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-17 | The detailed design provides sufficient information to derive unit verification criteria (e.g. test cases, formal proofs, or static analysis rules) for each software unit. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved and the SDS updated before approval of the detailed design
> - **MINOR** — should be resolved; may be deferred to next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Software Unit(s) Affected | Owner | Resolution | Status |
|---|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. RC-03 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: e.g. Unit X, Interface Y --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO: e.g. 17 --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. The software detailed design is approved and the coding phase may proceed.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision of the SDS. The coding phase may proceed provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "Unit X error-handling specification must be completed before coding of that unit begins."

**NOT APPROVED** — One or more MAJOR findings remain open. The SDS must be updated and re-reviewed before the coding phase begins.

### 5.3 Approval Signatures

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Software Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Quality Assurance | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
