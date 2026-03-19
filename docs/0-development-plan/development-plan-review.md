# Development Plan Review

## Table of Contents

> [!NOTE]
> Update this table of contents to reflect the sections in this document.
> In the MkDocs web view, the table of contents is generated automatically in the sidebar.
> This section is intended for printed or exported (PDF) versions of the document.
>
> 1. IDENTIFICATION
>    1.1 Document Overview
>    1.2 Abbreviations and Glossary
>    1.3 References
>    1.4 Conventions
> 2. REVIEW CONTEXT
>    2.1 Documents Under Review
>    2.2 Review Team
>    2.3 Review Process
> 3. REVIEW CHECKLIST
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-DPR-001 --> |
| Title | Development Plan Review |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal review of the development planning documents for the <!-- TODO: project name --> software development project.

The purpose of this review is to verify that the Project Management Plan (PMP), Software Development Plan (SDP), Software Configuration Management Plan (SCMP), and Data Management Plan (DMP) are complete, consistent with each other, and consistent with higher-level plans before the project proceeds to the next phase. The review covers completeness of all sections, definition of the project team and responsibilities, and alignment with higher-level plans such as the system design and development plan.

**Scope:** This review report covers the development planning documents identified in §2.1, at the versions specified therein. It does not assess the technical correctness of design decisions — that is covered by design reviews.

**Intended audience:** Project managers, technical leads, quality managers, and all participants in the development plan review for the <!-- TODO: project name --> project.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Documents Under Review

| Ref | Document | Document ID | Version | Date |
|---|---|---|---|---|
| [PMP] | Project Management Plan | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| [SDP] | Software Development Plan | <!-- TODO --> | <!-- TODO --> | <!-- TODO: or N/A if not instantiated --> |
| [SCMP] | Software Configuration Management Plan | <!-- TODO --> | <!-- TODO --> | <!-- TODO: or N/A if not instantiated --> |
| [DMP] | Data Management Plan | <!-- TODO --> | <!-- TODO --> | <!-- TODO: or N/A if not instantiated --> |

> [!NOTE]
> Mark a document as N/A if it has not been instantiated for this project. Justify the decision in the Project Management Plan.

### 2.2 Review Team

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| <!-- TODO: Add rows as needed --> | | | |

> [!NOTE]
> The author of the plans should not act as review chair. At least one reviewer should be independent of the software development team (e.g. quality assurance or regulatory affairs).

### 2.3 Review Process

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. System Design and Development Plan PRJ-SDDP-001 v1.0 --> |

## 3. REVIEW CHECKLIST

> [!NOTE]
> For each criterion, record the verdict and, if the criterion is not fully satisfied, create a finding in §4.
>
> **Verdict codes:**
>
> - **OK** — criterion is fully satisfied
> - **MINOR** — criterion is partially satisfied; a finding is raised but does not block approval
> - **MAJOR** — criterion is not satisfied; a finding is raised and must be resolved before approval
> - **N/A** — criterion is not applicable to this project or document (provide justification in Comments)

### 3.1 General Criteria — All Plans

The following criteria apply to all development planning documents listed in §2.1. Assess each criterion across all applicable documents; if any document does not satisfy the criterion, record the verdict accordingly and identify the affected document(s) in the Comments column.

#### 3.1.1 Completeness

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| G-01 | All sections of each plan are either completed with content or explicitly marked as not applicable with a written justification. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |
| G-02 | All placeholder text (e.g. `<!-- TODO -->`) has been resolved; no placeholder remains in the released version of any plan. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-03 | The document identification table (Document ID, Title, Version, Date, Status) is fully populated in each plan. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-04 | The version and date of each plan are consistent with the configuration management records. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

#### 3.1.2 Project Team and Responsibilities

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| G-05 | The project team roles are defined in the PMP, with a named person or team assigned to each role. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-06 | Responsibilities for each role are clearly described, including accountability for document authoring, review, and approval. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-07 | The organizational chart or team structure in the PMP is present and up to date. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-08 | Responsibilities for quality and regulatory compliance activities are assigned across the plans. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

#### 3.1.3 Consistency with Higher-Level Plans

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| G-09 | The development lifecycle model is consistent with the system design and development plan (or equivalent higher-level plan). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-10 | The project scope, objectives, and constraints are aligned with the higher-level plans. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-11 | Milestone dates and phase boundaries are consistent across all plans and with the higher-level plans. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| G-12 | References to higher-level plans use the correct document ID and version. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.2 Project Management Plan

> [!TIP]
> If the PMP is correct in all respects, you may replace the table below with a single statement such as: *"All criteria were reviewed and found to be satisfied. No findings were raised."*

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| PMP-01 | Team roles and responsibilities are defined (§2.1 of the PMP), and each role has a named person or team assigned. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-02 | The work breakdown structure and project planning are present, with tasks, dependencies, and milestones identified (§2.2). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-03 | Required resources (tools, test environments, calibrated equipment) are identified and managed under configuration control (§2.3). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-04 | Secure development assets are identified with ownership and CIA measures described (§2.4). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-05 | Relationships with stakeholders (customer, subcontractors, other teams) are described (§2.6). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-06 | Communication and review processes (meetings, bug triage, formal reviews) are defined (§2.7). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-07 | System requirements and project input data are referenced and their change management is described (§3). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-08 | Configuration management for software, documentation, and data is described or references the SCMP (§4). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-09 | Software development management is described or references the SDP (§5). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-10 | Test phases (integration, verification, security, penetration tests) are described or reference the SDP (§6). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| PMP-11 | Problem resolution process for externally reported issues is defined (§7). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.3 Software Development Plan

> [!NOTE]
> **Optional Document**
> If the SDP has not been instantiated for this project, mark this entire section N/A and verify that the corresponding topics are covered in the PMP.

> [!TIP]
> If the SDP is correct in all respects, you may replace the table below with a single statement such as: *"All criteria were reviewed and found to be satisfied. No findings were raised."*

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| SDP-01 | The software development lifecycle model is defined and the choice is justified. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-02 | Development phase activities, entry criteria, exit criteria, and deliverables are defined for each phase. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-03 | Roles and responsibilities for each development activity are assigned. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-04 | The CI/CD or DevOps strategy is described, or the section is marked N/A with justification. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-05 | Software development tools are listed with their versions; tool qualification obligations are addressed. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-06 | Coding standards and rules are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-07 | Secure coding standards are specified and compliance verification methods are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-08 | Integration test phases are described with entry/exit criteria. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-09 | Verification test phases are described with acceptance criteria and tester independence addressed. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SDP-10 | Security and penetration testing activities are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.4 Software Configuration Management Plan

> [!NOTE]
> **Optional Document**
> If the SCMP has not been instantiated for this project, mark this entire section N/A and verify that configuration management is covered in the PMP.

> [!TIP]
> If the SCMP is correct in all respects, you may replace the table below with a single statement such as: *"All criteria were reviewed and found to be satisfied. No findings were raised."*

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| SCMP-01 | The organizational model for configuration management is defined and the SCM manager role is assigned. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SCMP-02 | The SCM tool, branching strategy, and repository structure are described. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SCMP-03 | Software configuration items (source code, documentation, SOUPs, build artefacts, release packages) are identified. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SCMP-04 | Version numbering and naming conventions for configuration items are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SCMP-05 | The procedure for creating and archiving release packages is described. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SCMP-06 | The procedure for patch and hotfix management is described or marked N/A with justification. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| SCMP-07 | The security of configuration items (access control, backup, integrity) is addressed. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.5 Data Management Plan

> [!NOTE]
> **Optional Document**
> If the DMP has not been instantiated for this project (e.g. no AI/ML algorithms are used), mark this entire section N/A and verify that the justification is recorded in the PMP.

> [!TIP]
> If the DMP is correct in all respects, you may replace the table below with a single statement such as: *"All criteria were reviewed and found to be satisfied. No findings were raised."*

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| DMP-01 | Roles and responsibilities for data management are defined and assigned. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-02 | The tools and environment used for data management are described. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-03 | Data requirements (types, sources, volume, format) are specified. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-04 | Data quality criteria and the data quality model are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-05 | Data acquisition, annotation, preparation, and splitting processes are described. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-06 | The data review process and acceptance criteria for each dataset are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-07 | Data security, privacy, and access control measures are described. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-08 | Data decommissioning and retention policies are defined. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| DMP-09 | Regulatory compliance obligations for data (GDPR, local data protection law, etc.) are addressed. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved and the affected plan updated before approval
> - **MINOR** — should be resolved; may be deferred to next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Plan(s) Affected | Owner | Resolution | Status |
|---|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. G-05 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: e.g. PMP --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. All development plans are approved and the project may proceed to the next phase.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision of the affected plan(s). The project may proceed provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "PMP §2.1 must be updated to assign a named person to the Quality Manager role before v1.1 is issued."

**NOT APPROVED** — One or more MAJOR findings remain open. The affected plan(s) must be updated and re-reviewed before the project proceeds to the next phase.

### 5.3 Approval Signatures

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Quality Assurance | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
