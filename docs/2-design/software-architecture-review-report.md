# Software Architecture Review Report

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
>    3.1 Implementation of System and Product Requirements
>    3.2 Implementation of Software Requirements
>    3.3 Implementation of Risk Control Requirements
>    3.4 External Interfaces
>    3.5 SOUP Correct Functioning
>    3.6 Architectural Separations for Risk Control [Class C]
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-SAD-RR-001 --> |
| Title | Software Architecture Review Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal review of the Software Architecture Document (SAD) for the <!-- TODO: project name --> software development project.

The purpose of this review is to verify that the software architecture satisfies the criteria required by IEC 62304 §5.3 before detailed design begins. The review covers implementation of system and product requirements, implementation of software requirements, risk control requirements, external interfaces, correct functioning of SOUP items, and — for Class C software — architectural separations necessary for risk control.

**Scope:** This review report covers the SAD identified in §2.1. It does not assess the completeness of the underlying requirements — that is covered by the Software Requirements Specification Review Report.

**Intended audience:** Software quality assurance, software project manager, regulatory affairs, design review board.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Document Under Review

| Field | Value |
|---|---|
| Document Title | Software Architecture Document |
| Document ID | <!-- TODO: e.g. PRJ-SAD-001 --> |
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
> The author of the SAD should not act as review chair. At least one reviewer should be independent of the software development team (e.g. quality assurance or regulatory affairs).

### 2.3 Review Process

> [!NOTE]
> **IEC 62304 §5.3.6**
> IEC 62304 requires that the software architecture be reviewed for correctness, consistency with software requirements, and ability to implement all software requirements before proceeding to detailed design. The criteria in §3 operationalise this requirement.

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. Software Requirements Specification PRJ-SRS-001 v1.0, Risk Management File PRJ-RMF-001 v1.0, SOUP list PRJ-SOUP-001 v1.0 --> |

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

### 3.1 Implementation of System and Product Requirements

> [!NOTE]
> **IEC 62304 §5.3.1**
> The software architecture shall implement system and product requirements, including those allocated to software from the system-level design.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-01 | Each system or product requirement allocated to software is addressed by one or more architectural elements (components, modules, or layers). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |
| RC-02 | No system or product requirement allocated to software is left without a corresponding architectural element or explicit justification for its exclusion. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-03 | The architecture is consistent with any hardware or system-level constraints imposed by upstream design documents. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.2 Implementation of Software Requirements

> [!NOTE]
> **IEC 62304 §5.3.1**
> The architecture shall provide a framework within which all software requirements can be implemented.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-04 | Each software requirement in the SRS is traceable to one or more architectural elements. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-05 | The allocation of software requirements to architectural elements is documented (e.g. in a traceability matrix within the SAD or a linked traceability tool). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-06 | No software requirement is left unallocated in the architecture without documented justification. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.3 Implementation of Risk Control Requirements

> [!NOTE]
> **IEC 62304 §5.3.1 and ISO 14971**
> Software requirements derived from risk management activities shall be implemented by the architecture.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-07 | Each software requirement identified as a risk control measure in the risk management file is allocated to an architectural element. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-08 | The architectural elements responsible for risk control measures are identified and distinguishable from other elements in the architecture description. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-09 | The architecture does not introduce new hazards or compromise existing risk controls identified in the risk management file. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.4 External Interfaces

> [!NOTE]
> **IEC 62304 §5.3.2**
> The software architecture shall specify external interfaces between the software system and other systems, hardware components, operators, and users.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-10 | All interfaces between the software system and external software components (e.g. operating system, third-party services, communication protocols) are identified and described in the architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-11 | All interfaces between the software system and hardware components (e.g. sensors, actuators, communication peripherals) are identified and described in the architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-12 | The architecture specifies data formats, communication protocols, timing constraints, and error-handling strategies for each external interface. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-13 | Interface specifications are consistent with the corresponding software requirements and with the system-level interface definitions. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.5 SOUP Correct Functioning

> [!NOTE]
> **IEC 62304 §5.3.3 and §8.1.2**
> The architecture shall identify SOUP items and the requirements for their correct functioning within the system, including performance, robustness, and known anomaly handling.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-14 | All SOUP items used by the software system are identified in the architecture (name, version, supplier, intended use). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-15 | For each SOUP item, the architectural description specifies the requirements and constraints necessary for its correct functioning (e.g. configuration parameters, required platform, resource limits). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-16 | Known anomalies or limitations of each SOUP item are documented, and the architecture describes how the system tolerates or mitigates those anomalies. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
### 3.6 Architectural Separations for Risk Control [Class C]

> [!WARNING]
> **IEC 62304 §5.3.4 — Class C software only**
> For Class C software, the architecture shall include separations necessary to implement risk control measures, and the effectiveness of those separations shall be documented or verified.
>
> Mark each criterion **N/A** with justification if the software is Class A or Class B.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-17 | Architectural separations (e.g. partitioning, isolation mechanisms, memory protection, process boundaries) necessary to implement risk controls are identified in the architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-18 | For each separation mechanism, the architecture describes what hazardous failure modes it is intended to prevent or mitigate. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-19 | The effectiveness of each architectural separation is either documented (e.g. by analysis or reference to a recognised standard) or verified (e.g. by test or formal method), and the evidence is referenced in the architecture description. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-20 | The chosen separation mechanisms are appropriate to the severity of the associated hazard (i.e. higher-severity hazards use stronger or formally verified separation). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved and the SAD updated before approval of the architecture
> - **MINOR** — should be resolved; may be deferred to next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Architectural Element(s) Affected | Owner | Resolution | Status |
|---|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. RC-04 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: e.g. Module X, Interface Y --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO: e.g. 20 --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. The software architecture is approved and the detailed design phase may proceed.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision of the SAD. The detailed design phase may proceed provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "Component X interface specification must be updated to include error codes before v1.1 is issued."

**NOT APPROVED** — One or more MAJOR findings remain open. The SAD must be updated and re-reviewed before the detailed design phase begins.

### 5.3 Approval Signatures

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Software Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Quality Assurance | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
