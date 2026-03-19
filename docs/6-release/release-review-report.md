# Release Review Report

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
>    2.1 Version Under Review
>    2.2 Review Team
>    2.3 Review Process
> 3. REVIEW CHECKLIST
>    3.1 Verification and Testing
>    3.2 Defect Management
>    3.3 Documentation Completeness
>    3.4 Archiving and Configuration Management
>    3.5 Release Authorization
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION
>    5.1 Summary
>    5.2 Overall Verdict
>    5.3 Approval Signatures

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-RRR-001 --> |
| Title | Release Review Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal release review for version <!-- TODO: Vx.x alpha/beta/final --> of the <!-- TODO: project name --> software.

The purpose of this review is to verify that all criteria required by IEC 62304 §5.8 are satisfied before the software version is authorised for release. The review covers the completeness of verification and testing activities, the acceptability of residual defects, the completeness of development documentation (including secure operation and secure decommissioning guidelines, and release integrity and authenticity information), the integrity of the archived software and SOUP items, and the authorisation of the release by a person independent of the development team.

**Scope:** This review covers the software version identified in §2.1. It does not re-assess the correctness of individual test results — that is covered by the Software Test Report.

**Intended audience:** Software quality assurance, software project manager, regulatory affairs, design review board.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Version Under Review

| Field | Value |
|---|---|
| Software Name | <!-- TODO: XXX --> |
| Version | <!-- TODO: Vx.x alpha/beta/final --> |
| Version Delivery Description | <!-- TODO: Document ID and version, e.g. PRJ-VDD-001 v1.0 --> |
| Build ID | <!-- TODO: Source control build identifier --> |
| Delivery Date | <!-- TODO: YYYY-MM-DD --> |

### 2.2 Review Team

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Reviewer | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| <!-- TODO: Add rows as needed --> | | | |

> [!NOTE]
> The review chair and at least one reviewer must be independent of the development team (e.g. quality assurance or regulatory affairs). The development team may participate as information providers but shall not vote on the release verdict.

### 2.3 Review Process

> [!NOTE]
> **IEC 62304 §5.8**
> IEC 62304 §5.8 requires that the software developer ensure that the software is released in a controlled manner, that the release criteria have been met, and that a documented procedure is followed. The criteria in §3 operationalise these requirements.

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. Software Test Report PRJ-STR-001 v1.0, Version Delivery Description PRJ-VDD-001 v1.0, Risk Management File PRJ-RMF-001 v1.0 --> |

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

### 3.1 Verification and Testing

> [!NOTE]
> **IEC 62304 §5.8.1**
> Before releasing a software version, the developer shall ensure that all verification activities specified in the software development plan have been completed, and that the results have been evaluated against the acceptance criteria.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-01 | Verification activities are complete: all verification activities defined in the Software Development Plan and Software Test Plan for this version have been performed and their results are recorded. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |
| RC-02 | Test results have been evaluated: the results of all verification and testing activities have been reviewed against the defined acceptance criteria, and any deviations are documented. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.2 Defect Management

> [!NOTE]
> **IEC 62304 §5.8.1 and §9**
> Known residual defects (anomalies not corrected before release) shall be documented and assessed to ensure they do not introduce unacceptable risk to patients, users, or third parties.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-03 | Known residual defects are documented: all known software anomalies that are not corrected in this version are listed, described, and recorded (e.g. in the release notes or the anomaly tracking system). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-04 | Known residual defects do not pose an unacceptable risk: each documented residual defect has been evaluated for its impact on safety and effectiveness, and the risk management file confirms that the residual risks remain acceptable. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.3 Documentation Completeness

> [!NOTE]
> **IEC 62304 §5.8.1, §5.8.7 and IEC 81001-5-1**
> All development activities and associated documentation shall be complete before release. The released version shall be documented in a version delivery description, and the product shall be accompanied by documentation sufficient for its installation, use, maintenance, secure operation, and secure decommissioning. Information enabling end-users to verify the integrity and, where applicable, the authenticity of the release artefacts shall also be provided.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-05 | Development activities and associated documentation are complete: all software development lifecycle activities required for this version (design, implementation, verification, risk management updates) are finished, and the corresponding documents are in an approved or release-ready state. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-06 | The software version is documented and complete: a Version Delivery Description (or equivalent) identifying the released version, its composition, hardware configuration, dependencies, SBOM, and master location has been produced and approved. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-07 | The software product is released with documentation enabling the tasks required for its installation, use, and application maintenance: the release package includes or references an up-to-date installation manual, user manual, and maintenance documentation appropriate to the intended users. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-08 | Secure operation guidelines are present: the release documentation includes or references guidance covering secure configuration, access control, network exposure, credential management, and any other operational security measures necessary for the safe and secure use of the software in its intended environment. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-09 | Secure decommissioning guidelines are present: the release documentation includes or references guidance for the secure removal of the software, including procedures for the deletion or secure disposal of software artefacts, configuration data, and personal or sensitive data held by the software, in accordance with applicable data protection regulations. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-10 | Release integrity and authenticity verification information is provided: the release package includes cryptographic hash values (e.g. SHA-256) for all distributed artefacts, enabling recipients to verify that the delivered items have not been corrupted or tampered with. Where applicable, artefacts are digitally signed and the corresponding public key, certificate, or verification procedure is documented, enabling recipients to verify the authenticity of the release. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.4 Archiving and Configuration Management

> [!NOTE]
> **IEC 62304 §5.8.2 and §8.3**
> The released software version and all associated SOUP items shall be archived in a controlled manner that guarantees reproducibility and satisfies the record retention requirements imposed by applicable regulations (e.g. MDR Annex II, 21 CFR Part 820).

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-11 | The software product version is archived: all constituent items of the released software (binaries, executables, libraries, source code, compilation files, integration and assembly files, scripts, configuration files, etc.) are stored in the configuration management system under a uniquely identified label or tag, or in an equivalent controlled archive location. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-12 | The SOUP items for the software product version are archived: all SOUP items (binaries, executables, libraries, source code, compilation files, integration and assembly files, scripts, configuration files, etc.) used by this version are stored in a controlled archive location, with their version identifiers recorded in the Version Delivery Description or SBOM. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-13 | The version is archived to ensure retention of records for the duration required by regulations: the archive policy covering this version guarantees that the records will be retained for the period mandated by applicable regulations and standards for the markets in which the device is placed (e.g. at least 10 years under EU MDR, or as required by other applicable regulations). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.5 Release Authorization

> [!NOTE]
> **IEC 62304 §5.8.6**
> The release of the software shall be authorized by a person who is independent of the software development team, and who has the authority and competence to make the release decision.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-14 | A person independent of the development team authorizes the release of the software: the release authorization is provided by an individual (e.g. quality assurance manager, regulatory affairs representative) who was not part of the development team for this version, and whose authorization is documented with signature and date. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved before the release is authorised
> - **MINOR** — should be resolved; may be deferred to the next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Owner | Resolution | Status |
|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. RC-03 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO: e.g. 14 --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. The software version is approved for release.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision. The software version may be released provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "The known-defects list in the release notes must be updated to include BUG-042 before the release package is distributed."

**NOT APPROVED** — One or more MAJOR findings remain open. The identified issues must be resolved and this review must be repeated before the software version can be released.

### 5.3 Approval Signatures

> [!NOTE]
> **IEC 62304 §5.8.6**
> The release authorizer (row 3) must be a person independent of the development team.

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Software Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Release Authorizer (independent of development team) | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
