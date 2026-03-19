# Software Test Plan Review Report

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
>    3.1 Test Environment and Infrastructure
>    3.2 Integration Test Coverage
>    3.3 Integration Test Procedures
>    3.4 Integration Regression Testing
>    3.5 Test Content and Structure
>    3.6 Requirements Coverage
>    3.7 Test Procedure Adequacy
>    3.8 Requirements Traceability
>    3.9 Change Management and Regression Testing
> 4. REVIEW FINDINGS
> 5. REVIEW CONCLUSION

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-STP-RR-001 --> |
| Title | Software Test Plan Review Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document presents the results of the formal review of the Software Test Plan (STP) for the <!-- TODO: project name --> software development project.

The purpose of this review is to verify that the STP meets the quality criteria required by IEC 62304 §5.7 before integration and verification testing begins. The review covers the specification of test phases, platforms, and tools; coverage of software components and interfaces by integration tests; correctness and adequacy of test procedures; test content structure; traceability to the Software Requirements Specification; and provisions for change management and regression testing.

**Scope:** This review report covers the STP identified in §2.1. It does not assess the correctness of the underlying software requirements — that is covered by the Software Requirements Specification Review Report.

**Intended audience:** Software quality assurance, software project manager, regulatory affairs, design review board.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW CONTEXT

### 2.1 Document Under Review

| Field | Value |
|---|---|
| Document Title | Software Test Plan |
| Document ID | <!-- TODO: e.g. PRJ-STP-001 --> |
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
> The author of the STP should not act as review chair. At least one reviewer should be independent of the software development team (e.g. quality assurance or regulatory affairs).

### 2.3 Review Process

> [!NOTE]
> **IEC 62304 §5.7**
> IEC 62304 requires that the software integration and system testing activities be planned, that each test identify its inputs, expected results, and pass/fail criteria, and that tests be traceable to software requirements. The criteria in §3 operationalise these requirements.

The review was conducted as follows:

| Field | Value |
|---|---|
| Review method | <!-- TODO: e.g. Walkthrough / Inspection / Peer review --> |
| Review meeting date | <!-- TODO: YYYY-MM-DD, or N/A if asynchronous --> |
| Review meeting location / tool | <!-- TODO: e.g. Teams call, Confluence, GitHub PR --> |
| Supporting documents consulted | <!-- TODO: e.g. Software Requirements Specification PRJ-SRS-001 v1.0, Software Architecture Document PRJ-SAD-001 v1.0, Risk Management File PRJ-RMF-001 v1.0 --> |

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

### 3.1 Test Environment and Infrastructure

> [!NOTE]
> **IEC 62304 §5.7.1**
> The test plan shall identify the test phases, the hardware and software platforms used for testing, and the tools required to execute the tests.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-01 | The test plan identifies all testing phases (e.g. unit, integration, verification, security, end-user) and defines the scope and objectives of each phase. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO: e.g. F-01, or — --> | <!-- TODO --> |
| RC-02 | The hardware and software platforms on which tests are executed are specified (name, version, configuration) and are representative of the intended operational environment. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-03 | All software tools required to execute the tests (test frameworks, simulators, data generators, coverage analysers, security test tools, etc.) are identified with their name and version. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.2 Integration Test Coverage

> [!NOTE]
> **IEC 62304 §5.7.2**
> Integration tests shall cover all software components to be integrated and their interfaces, both internal (between software components) and external (between the software system and external systems or hardware).

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-04 | Integration tests address each software component identified in the software architecture. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-05 | Integration tests cover all internal interfaces between software components (data exchanges, function calls, shared resources, inter-process communication, etc.). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-06 | Integration tests cover all external interfaces between the software system and external entities (hardware, operating system, third-party services, communication protocols, user interfaces, etc.). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.3 Integration Test Procedures

> [!NOTE]
> **IEC 62304 §5.7.3**
> Integration test procedures shall be adequate to verify the correct integration of software components and the correct behaviour of interfaces.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-07 | Integration test procedures verify the correct integration of software components (e.g. correct data passing, correct sequencing, correct error propagation between components). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-08 | Integration test procedures verify the correct behaviour of interfaces between software components and between the software system and external entities (e.g. boundary conditions, protocol compliance, error handling). | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.4 Integration Regression Testing

> [!NOTE]
> **IEC 62304 §5.7.4**
> Integration testing shall include regression tests to confirm that changes or additions to the integrated software have not introduced new defects.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-09 | The test plan includes a defined set of integration regression tests intended to detect defects introduced into the software during integration activities. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.5 Test Content and Structure

> [!NOTE]
> **IEC 62304 §5.7.3 and §5.7.5**
> Each test shall specify input stimuli, expected results, and pass/fail criteria so that the outcome of the test is unambiguous and reproducible.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-10 | Each test specifies the input stimuli (data, signals, user actions, environmental conditions, or other preconditions) required to execute the test. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-11 | Each test specifies the expected results (outputs, states, or observable behaviours) that the software shall produce in response to the input stimuli. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-12 | Each test specifies objective and measurable pass/fail criteria that allow the tester to determine unambiguously whether the test has passed or failed, without subjective judgement. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.6 Requirements Coverage

> [!NOTE]
> **IEC 62304 §5.7.5**
> Tests shall cover all software requirements of the Software Requirements Specification and, by extension, all software components of the software system.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-13 | Every requirement in the Software Requirements Specification is addressed by at least one test in the test plan, or its exclusion is explicitly justified and documented. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-14 | As a consequence of RC-13, every software component of the software system is exercised by at least one test. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.7 Test Procedure Adequacy

> [!NOTE]
> **IEC 62304 §5.7.5**
> Test procedures shall be adequate to verify the requirements of the Software Requirements Specification correctly and completely.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-15 | The test procedures are sufficient to verify each SRS requirement correctly — the test stimuli, environment, and measurement approach are capable of detecting a failure to meet the requirement. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.8 Requirements Traceability

> [!NOTE]
> **IEC 62304 §5.7**
> The test plan shall provide traceability between the requirements of the Software Requirements Specification and the test procedures that verify them.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-16 | A traceability matrix (or equivalent mechanism) is provided that links each SRS requirement to the test procedure(s) that verify it, and each test procedure to the SRS requirement(s) it verifies. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

### 3.9 Change Management and Regression Testing

> [!NOTE]
> **IEC 62304 §5.7.6 and §6.2**
> When the software system is modified, tests shall be updated or added to verify the changes, to verify defect corrections, and to demonstrate that no side effects have been introduced.

| # | Review Criterion | Verdict | Finding Ref. | Comments |
|---|---|---|---|---|
| RC-17 | When changes are made to the software system (including defect corrections), the test plan provides for adding new tests or modifying existing tests to verify those changes. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |
| RC-18 | The test plan includes a non-regression testing strategy to demonstrate that changes to the software system have not introduced side effects into previously correct functionality. | <!-- TODO: OK / MINOR / MAJOR / N/A --> | <!-- TODO --> | <!-- TODO --> |

## 4. REVIEW FINDINGS

> [!NOTE]
> Record each finding raised in §3 here. Each finding must have a unique reference, a description, a severity, an owner, and a resolution status.
>
> **Severity codes:**
>
> - **MAJOR** — must be resolved and the STP updated before approval of the test plan
> - **MINOR** — should be resolved; may be deferred to next version with written justification
> - **OBSERVATION** — improvement suggestion; resolution is optional

| Finding Ref. | RC # | Description | Severity | Test(s) / Section(s) Affected | Owner | Resolution | Status |
|---|---|---|---|---|---|---|---|
| F-01 | <!-- TODO: e.g. RC-10 --> | <!-- TODO: Describe the issue clearly and precisely. --> | <!-- TODO: MAJOR / MINOR / OBSERVATION --> | <!-- TODO: e.g. T-SRS-REQ-010-1, §4.2 --> | <!-- TODO: Name --> | <!-- TODO: Describe corrective action taken, or reason for deferral. --> | <!-- TODO: Open / Closed --> |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

> [!TIP]
> If no findings were raised, replace this table with: *"No findings were identified during this review."*

## 5. REVIEW CONCLUSION

### 5.1 Summary

| Metric | Count |
|---|---|
| Total criteria reviewed | <!-- TODO: e.g. 18 --> |
| Criteria with verdict OK or N/A | <!-- TODO --> |
| Criteria with verdict MINOR | <!-- TODO --> |
| Criteria with verdict MAJOR | <!-- TODO --> |
| Total findings raised | <!-- TODO --> |
| Findings closed at time of conclusion | <!-- TODO --> |
| Findings remaining open | <!-- TODO --> |

### 5.2 Overall Verdict

> [!NOTE]
> Select one of the three verdicts below and delete the others.

**APPROVED** — All review criteria are satisfied (OK or N/A). No open MAJOR findings. The Software Test Plan is approved and integration and verification testing may proceed.

**APPROVED WITH CONDITIONS** — No open MAJOR findings. One or more MINOR findings remain open and must be resolved in the next revision of the STP. Integration and verification testing may proceed provided the conditions listed below are met.

> [!NOTE]
> List conditions, e.g.: "Traceability matrix must be completed for requirements SRS-REQ-040 through SRS-REQ-060 before testing begins."

**NOT APPROVED** — One or more MAJOR findings remain open. The STP must be updated and re-reviewed before integration and verification testing begins.

### 5.3 Approval Signatures

| Role | Name | Signature | Date |
|---|---|---|---|
| Review Chair | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Software Project Manager | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
| Quality Assurance | <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |
