# Software Test Report

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
> 2. OVERVIEW OF TEST RESULTS
>    2.1 Tests Log
>    2.2 Rationale for Decision
>    2.3 Overall Assessment of Tests
>    2.4 Test Platform Configuration
>    2.5 Impact of Test Environment
> 3. DETAILED TEST RESULTS
>    3.1 <!-- TODO: Sub-section name matching test description document -->

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-STR-001 --> |
| Title | Software Test Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document is the software test report of the xxx testing phase of the XXX software development project. It contains the results of tests which were executed during the testing phase xxx.

**Scope:** <!-- TODO: Describe the scope of this document, e.g. which software items, modules, or test phases are covered. -->

**Intended audience:** <!-- TODO: e.g. software engineers, quality assurance, regulatory affairs. -->

--8<-- "snippets/glossary-and-references.md"

## 2. OVERVIEW OF TEST RESULTS

### 2.1 Tests Log

> [!NOTE]
> Provide synthetic information about the tests executed in this phase.

The XXX software (version x.y.z) was tested on the xxx test platform located in xxx, from yyyy/mm/dd to yyyy/mm/dd. The tests of the test phase (ref. software test plan) were executed.

Testers were:

> [!NOTE]
> List the full names of all testers. Recording tester names is mandatory.

- <!-- TODO: e.g. John Doe -->
- <!-- TODO: e.g. Marc Smith -->

### 2.2 Rationale for Decision

After executing a test, the decision is defined according to the following rules:

| Decision | Definition |
|---|---|
| **PASSED** | The test sheet is set to "PASSED" state when all steps are in "PASSED" state. The real result is compliant to the expected result. |
| **FAILED** | The test sheet is set to "FAILED" state when all steps of the test are set to "FAILED" state, or when the result of a step differs from the expected result. |
| **Partial PASSED** | The test sheet is set to "Partial PASSED" state when at least one step of the test is set to "FAILED" state, or when the result of a step is partially compliant to the expected result. |
| **NOT RUN** | Default state of a test sheet not yet executed. |
| **NOT COMPLETED** | The test sheet is set to "NOT COMPLETED" state when at least one step of the test is set to "NOT RUN" state. |

> [!NOTE]
> Partial PASSED: Keep it or remove. It may be subject to tester's interpretation and source of inconsistencies.

> [!NOTE]
> For each FAILED step, at least one bug shall be created (or referenced if one already exists).
 
Tests results are listed in §3.

### 2.3 Overall Assessment of Tests

> [!NOTE]
> Give a qualitative overall assessment of the tests. Examples:
> - All tests with interfaces passed; graphical user interface is not optimized for screens of the test platform.
> - All tests passed but software is too slow for acceptable use.

**Quantitative results — test statistics:**

| Outcome | Count | Percentage |
|---|---|---|
| PASSED | <!-- TODO --> | <!-- TODO --> % |
| FAILED | <!-- TODO --> | <!-- TODO --> % |
| Partial PASSED | <!-- TODO --> | <!-- TODO --> % |
| NOT RUN | <!-- TODO --> | <!-- TODO --> % |
| NOT COMPLETED | <!-- TODO --> | <!-- TODO --> % |

**Bug and enhancement statistics:**

| Category | Count |
|---|---|
| Total | <!-- TODO --> |
| Critical | <!-- TODO --> |
| Major | <!-- TODO --> |
| Minor | <!-- TODO --> |
| Enhancements | <!-- TODO --> |

### 2.4 Test Platform Configuration

> [!NOTE]
> Record here the results of the test platform configuration verification section from the test description document.

### 2.5 Impact of Test Environment

> [!NOTE]
> Describe the impact of the test environment, if any.
> Describe differences between expected conditions and real conditions, such as a software test tool, a simulator, or hardware that did not work as expected.

## 3. DETAILED TEST RESULTS

For each executed test, this section contains:

- Test identification;
- Test title;
- Test decision;
- A comment containing additional information or problems encountered during execution, and differences with the test procedure.

For problems leading to a bug, the bug ID is reported in the result of the step where the problem was encountered.

> [!WARNING]
> For each FAILED step, at least one bug shall be created (or referenced if one already exists).

### 3.1 Sub-section name

> [!NOTE]
> Copy the section names and tests from the software test description document.
>      For each test, fill in the Comment and Decision columns.
>      Add a Result column to the test procedure steps table.

> [!NOTE]
> Repeat the block below for each test in this sub-section.

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | Same ID as in test description | <!-- TODO --> | <!-- TODO: PASSED / FAILED / Partial PASSED / NOT RUN / NOT COMPLETED --> |
| Test description | Same as in test description | | |
| Verified Requirement | e.g. SRS-REQ-001 — same as in test description | | |
| Initial conditions | Same as in test description | <!-- TODO --> | |
| Tests inputs | Same as in test description | <!-- TODO --> | |
| Data collection actions | Same as in test description | <!-- TODO --> | |
| Tests outputs | Same as in test description | <!-- TODO --> | |
| Assumptions and constraints | Same as in test description | <!-- TODO --> | |
| Expected results and criteria | Same as in test description | | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start foo | Foo is started | PASSED |
| 2 | Establish connection | Foo-Bar connection established | FAILED, bug #123 |
| <!-- TODO: step number --> | Same as in test description | Same as in test description | <!-- TODO: PASSED / FAILED / NOT RUN --> |
| <!-- TODO: step number --> | Same as in test description | Same as in test description | <!-- TODO: PASSED / FAILED / NOT RUN --> |

> [!NOTE]
> Add further test blocks (copy the table pair above) for each additional test.

#### Example: PASSED

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | Same ID as in test desc. | | PASSED |
| Test description | Same as in test description. | | |
| Verified Requirement | SRS-REQ-001 | Same as in test desc. | |
| Initial conditions | Same as in test desc. | Same as in test desc. | |
| Tests inputs | Same as in test desc. | Same as in test desc. | |
| Data collection actions | Same as in test desc. | Same as in test desc. | |
| Tests outputs | Same as in test desc. | Same as in test desc. | |
| Assumptions and constraints | If any, may be limited access to a tool, license … | | |
| Expected results and criteria | FOO AND BAR ARE STARTED, CONNECTION IS ESTABLISHED | | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start foo | Foo is started | PASSED |
| 2 | Start bar | Bar is started | PASSED |
| 3 | Establish connection | Foo-Bar connection established | PASSED |

#### Example: FAILED

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | Same ID as in test desc. | | FAILED |
| Test description | Same as in test description. | | |
| Verified Requirement | SRS-REQ-001 | Same as in test desc. | |
| Initial conditions | Same as in test desc. | Same as in test desc. | |
| Tests inputs | Same as in test desc. | Same as in test desc. | |
| Data collection actions | Same as in test desc. | Same as in test desc. | |
| Tests outputs | Same as in test desc. | Same as in test desc. | |
| Assumptions and constraints | If any, may be limited access to a tool, license … | | |
| Expected results and criteria | FOO AND BAR ARE STARTED, CONNECTION IS ESTABLISHED | | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start foo | Foo is started | PASSED |
| 2 | Start bar | Bar is started | PASSED |
| 3 | Establish connection | Foo-Bar connection established | FAILED, bug #234 |

#### Example: Partial PASSED

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | Same ID as in test desc. | | Partial PASSED |
| Test description | Same as in test description. | Connection loss after 1 min is acceptable for this test phase. | |
| Verified Requirement | SRS-REQ-001 | Same as in test desc. | |
| Initial conditions | Same as in test desc. | Same as in test desc. | |
| Tests inputs | Same as in test desc. | Same as in test desc. | |
| Data collection actions | Same as in test desc. | Same as in test desc. | |
| Tests outputs | Same as in test desc. | Same as in test desc. | |
| Assumptions and constraints | If any, may be limited access to a tool, license … | | |
| Expected results and criteria | CONNECTION IS ESTABLISHED | | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start foo | Foo is started | PASSED |
| 2 | Start bar | Bar is started | PASSED |
| 3 | Establish connection | Foo-Bar connection established | PASSED, but connection lost after 1 min. Bug #123 |

#### Example: NOT RUN — default state

> It is not necessary to write "NOT RUN" everywhere when creating the document. NOT RUN shall be used to mark tests not run at the end of a testing phase.

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | Same ID as in test desc. | | NOT RUN |
| Test description | Same as in test description. | | |
| Verified Requirement | SRS-REQ-001 | Same as in test desc. | |
| Initial conditions | Same as in test desc. | Same as in test desc. | |
| Tests inputs | Same as in test desc. | Same as in test desc. | |
| Data collection actions | Same as in test desc. | Same as in test desc. | |
| Tests outputs | Same as in test desc. | Same as in test desc. | |
| Assumptions and constraints | If any, may be limited access to a tool, license … | | |
| Expected results and criteria | CONNECTION IS ESTABLISHED | | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start foo | Foo is started | NOT RUN |
| 2 | Start bar | Bar is started | NOT RUN |
| 3 | Establish connection | Foo-Bar connection established | NOT RUN |

#### Example: NOT COMPLETED

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | Same ID as in test desc. | | NOT COMPLETED |
| Test description | Same as in test description. | Unable to establish connection, network cable missing. | |
| Verified Requirement | SRS-REQ-001 | Same as in test desc. | |
| Initial conditions | Same as in test desc. | Same as in test desc. | |
| Tests inputs | Same as in test desc. | Same as in test desc. | |
| Data collection actions | Same as in test desc. | Same as in test desc. | |
| Tests outputs | Same as in test desc. | Same as in test desc. | |
| Assumptions and constraints | If any, may be limited access to a tool, license … | | |
| Expected results and criteria | CONNECTION IS ESTABLISHED | | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start foo | Foo is started | PASSED |
| 2 | Start bar | Bar is started | PASSED |
| 3 | Establish connection | Foo-Bar connection established | NOT RUN |

#### Example: Security test PASSED

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | T-SRS-SEC-001 | | PASSED |
| Test description | Verify that open ports are 443 and 22 only | None | |
| Verified Requirement | SRS-SEC-001 | None | |
| Initial conditions | XXX Software is started | None | |
| Tests inputs | N/A | None | |
| Data collection actions | Nmap output using T-SRS-SEC-001-NMAP.sh | None | |
| Tests outputs | T-SRS-SEC-001.log | None | |
| Assumptions and constraints | PC used to perform nmap scan is connected on the same LAN without network restrictions | None | |
| Expected results and criteria | Open ports are 443 and 22 only | None | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start T-SRS-SEC-001-NMAP.sh from the connected PC | T-SRS-SEC-001.log file is created | PASSED |
| 2 | Open T-SRS-SEC-001.log | Open ports are 443 and 22 only | PASSED |

#### Example: Security test PASSED (second example)

| Field | Value | Comment | Decision |
|---|---|---|---|
| Test ID | T-SRS-SEC-002 | | PASSED |
| Test description | Verify that only known vulnerabilities are detected | None | |
| Verified Requirement | SRS-SEC-002 | The requirement is generic and doesn't list the known vulnerabilities. They are present in the architecture doc. | |
| Initial conditions | XXX Software is started | None | |
| Tests inputs | N/A | None | |
| Data collection actions | Nmap output using T-SRS-SEC-002-VULSCAN.sh | None | |
| Tests outputs | T-SRS-SEC-002.log | None | |
| Assumptions and constraints | PC used to perform nmap + vulscan is connected on the same LAN without network restrictions | None | |
| Expected results and criteria | Known vulnerabilities are CVE 20XX-XXXX and CVE 20YY-YYYY | None | |

**Test procedure:**

| Step number | Operator actions | Expected result and evaluation criteria | Result |
|---|---|---|---|
| 1 | Start T-SRS-SEC-002-vulscan.sh from the connected PC | T-SRS-SEC-002.log file is created | PASSED |
| 2 | Open T-SRS-SEC-002.log | Detected known vulnerabilities are CVE 20XX-XXXX and CVE 20YY-YYYY | PASSED |
