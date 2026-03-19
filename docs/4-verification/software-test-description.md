# Software Test Description

## Table of Contents

> [!NOTE]
> Update this table of contents to reflect the sections in this document.
>      In the MkDocs web view, the table of contents is generated automatically in the sidebar.
>      This section is intended for printed or exported (PDF) versions of the document.
>
> Example:
> 1. IDENTIFICATION
>    1.1 Document Overview
>    1.2 Abbreviations and Glossary
>    1.3 References
>    1.4 Conventions
> 2. TEST PREPARATIONS
>    2.1 <Preparation scope name>
>       2.1.1 Hardware Preparation
>       2.1.2 Software Preparation
>       2.1.3 Other Test Preparation
>       2.1.4 Safety, Security and Privacy Precautions
>       2.1.5 Test Platform Configuration Verification
> 3. TEST DESCRIPTIONS
>    3.1 <Test group name>

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-STD-001 --> |
| Title | Software Test Description |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document is the Software Test Description of the <!-- TODO: project name --> software development project. It contains the description of tests listed in the Software Test Plan <!-- TODO: ref. PRJ-STP-001 -->. These tests are executed during <!-- TODO: project name --> integration and verification:

- Software Integration tests,
- Software Verification tests.

**Scope:** <!-- TODO: Describe the scope of this document, e.g. which software items, modules or testing phases are covered. -->

**Intended audience:** <!-- TODO: e.g. Integration engineers, test engineers, quality managers. -->

--8<-- "snippets/glossary-and-references.md"

## 2. TEST PREPARATIONS

> [!NOTE]
> This section contains tasks and recommendations to be performed before executing tests.
>
> Describe the test preparation tasks for a phase, a category of tests, or a single test (in the latter case, use the test identifier). Give sub-sections a name that matches the scope of the described tasks. The tests impacted by each preparation shall be listed, or a reference shall be given to a test list in the Software Test Plan or in §3 of this document.

### 2.1 Choose a sub-section name

> **Note:** The sub-section name may be:
>
> - Testing phase *xxx*
> - or category of tests *xxx*
> - or test *xxx* if a single test deserves special preparation
> - or some other logic to group tests

> [!NOTE]
> List or reference the tests impacted by the preparations described below.

#### 2.1.1 Hardware Preparation

> [!NOTE]
> Describe platform configuration operations, such as specific hardware to be used and physical network configuration. Add a diagram and steps to set up hardware if needed.
>
> Note: these steps are different from those in the Software Test Plan, where the installation of the whole platform is described.

#### 2.1.2 Software Preparation

> [!NOTE]
> Describe software set-up and configuration operations, such as simulators or software test tools to be used and logical network configuration. Consider preparing test sample data, emptying databases or directories before beginning tests. Add a diagram and steps to set up software if needed.

#### 2.1.3 Other Test Preparation

> [!NOTE]
> Describe any other specific tasks to be performed before tests.

#### 2.1.4 Safety, Security and Privacy Precautions

> [!NOTE]
> Add warnings or precautions about safety, security and privacy. Consider this carefully if tests are performed in a healthcare environment.

#### 2.1.5 Test Platform Configuration Verification

> [!NOTE]
> If necessary, add a step to verify the versions of the hardware and software environment:
>
> - HW components,
> - SW tools, such as simulators,
> - For cloud software, verifying the versions of the environment,
> - Environment variables, configuration files.

| Component | Expected Version / Value | Actual Version / Value | Pass / Fail |
|---|---|---|---|
| Operating system | Windows 10 22H2 (64-bit) | | |
| Application under test | V1.2.0 (build 20240315) | | |
| Test automation framework | Selenium 4.18 | | |
| <!-- TODO: Hardware component name --> | <!-- TODO: version --> | | |
| <!-- TODO: Software tool / simulator --> | <!-- TODO: version --> | | |
| <!-- TODO: Environment variable or config file --> | <!-- TODO: expected value --> | | |

## 3. TEST DESCRIPTIONS

> **Note:** Tests may be organised by testing phase, by group, in alphabetical order, or — most effectively — in chronological order of execution for each phase so that testers do not waste time searching for tests. If a sequence of actions is executed more than once, either duplicate it (accepting the risk of inconsistency when modifying) or reference the common procedure.
>
> Each test defined in the Software Test Plan shall be described here. For most tests only a subset of fields in the table is used; mark unused fields N/A (not applicable) or omit the row if no test in the group uses it.
>
> Two table patterns are available — **long** and **short** — as shown below.

#### Long test table pattern

> **Note:** Use the long pattern when the test involves data collection, post-processing, specific assumptions, or when test inputs and outputs must be fully traceable.

| Field | Value | Notes |
|---|---|---|
| Test ID | Same ID as in the Software Test Plan | |
| Test description | Same as in the Software Test Plan | |
| Verified requirement | SRS-REQ-001 | Verification method: I / A / D / T |
| Initial conditions | The state of software before the test | May reference a procedure or be the result of a previous test |
| Test inputs | Input data from any test tool, input file names and locations | May reference a procedure to use the test tool |
| Data collection actions | Recording and post-processing of output data | May reference a procedure to record data with a test tool |
| Test outputs | Output data file names and locations, logs, etc. | Give unique names to output data files |
| Assumptions and constraints | If any, e.g. limited access to a tool or licence | |
| Expected results and criteria | List the expected results of the test | Criteria to evaluate the result |


| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | Perform action step 1 | Step 1 result is observed |
| 2 | Perform action step 2 | Step 2 result meets expected criteria |

#### Short test table pattern

> **Note:** Use the short pattern for straightforward tests that do not require data collection or extensive setup.

| Field | Value | Notes |
|---|---|---|
| Test ID | Same ID as in the Software Test Plan | |
| Test description | Same as in the Software Test Plan | |
| Verified requirement | SRS-REQ-001 | |
| Initial conditions | The state of software before the test | May reference a procedure or be the result of a previous test |

| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | Perform action step 1 | Step 1 result is observed |
| 2 | Perform action step 2 | Step 2 result is observed |
| 3 | Perform action step 3 | Last step gives the expected result of the test |

### 3.1 Choose a sub-section name

> **Note:** The sub-section name may be:
>
> - Testing phase *xxx*
> - or category of tests *xxx*
> - or some other logic to group tests

#### T-SRS-REQ-001 — <!-- TODO: Short test title -->

> **Example — Inspection:** The following shows an example of an **Inspection** test. Remove or replace it with actual tests.

| Field | Value | Notes |
|---|---|---|
| Test ID | T-SRS-REQ-001 | |
| Test description | Same description as in the Software Test Plan | |
| Verified requirement | SRS-REQ-001 | Inspection |
| Initial conditions | e.g. XXX Software is started and idle | |
| Test inputs | N/A | |
| Data collection actions | N/A | |
| Test outputs | N/A | |
| Assumptions and constraints | N/A | |
| Expected results and criteria | Describe the expected outcome and the criteria to evaluate it | |

| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | Open the document under inspection, navigate to the relevant section | Section is located and accessible |
| 2 | Verify that the required element or content is present | Element is present and matches the expected value |

> **Example — Demonstration:** The following shows an example of a **Demonstration** test. Remove or replace it with actual tests.

| Field | Value | Notes |
|---|---|---|
| Test ID | T-SRS-REQ-002 | |
| Test description | Same description as in the Software Test Plan | |
| Verified requirement | TODO: SRS-REQ-002 | Demonstration |
| Initial conditions | e.g. XXX Software is started and idle | |
| Test inputs | N/A | |
| Data collection actions | N/A | |
| Test outputs | N/A | |
| Assumptions and constraints | N/A | |
| Expected results and criteria | e.g. The chosen item is selected. See last step for criteria. | |

| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | Open the relevant screen or function | Screen or function is displayed |
| 2 | Perform the action under test | Action completes; result is displayed as expected |
| 3 | Validate or confirm the result | Expected state is reached and confirmed |

> **Example — Analysis:** The following shows an example of an **Analysis** test involving data generation and post-processing. Remove or replace it with actual tests.

| Field | Value | Notes |
|---|---|---|
| Test ID | T-SRS-REQ-003 | |
| Test description | Same description as in the Software Test Plan | |
| Verified requirement | SRS-REQ-003 | Analysis |
| Initial conditions | e.g. XXX Software is started and set in "Verbose" mode | |
| Test inputs | e.g. Script xxx to generate data | See procedure xxx on how to use the script |
| Data collection actions | e.g. Log file xxx-verbose.log and post-processor script | |
| Test outputs | e.g. xxx-post-process.txt and xxx-post-process.png | See procedure xxx on how to use the script |
| Assumptions and constraints | e.g. Do not run the data generator script with more than 1000 loops | |
| Expected results and criteria | Describe the expected output files and their content, including numerical criteria and tolerances | E.g.: The post process graph is a gausian. The post process values are: Chi2 = … Mean = … stdev= … (with x% error margin) |

| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | Set the required mode and restart the software | Software starts; expected log file is created in the expected directory |
| 2 | Run the data generator script | Data binary file is generated |
| 3 | Open the data file with the software | Software processes the file; completion message is displayed |
| 4 | Run the post-processing script and wait for completion | Output files are generated |
| 5 | Open the output files | Results meet the specified numerical criteria |

> **Example — Test (functional):** The following shows an example of a functional **Test** using a simulator. Remove or replace it with actual tests.

| Field | Value | Notes |
|---|---|---|
| Test ID | T-SRS-REQ-004 | |
| Test description | Same description as in the Software Test Plan | |
| Verified requirement | SRS-REQ-004 | Test |
| Initial conditions | e.g. XXX Software is started; YYY simulator is started | TODO: See procedure yyy on how to use YYY simulator |
| Test inputs | N/A | |
| Data collection actions | N/A | |
| Test outputs | N/A | |
| Assumptions and constraints | e.g. YYY simulator works only in the range of zzz | |
| Expected results and criteria | TODO: e.g. Data received and processed. See test procedure for criteria. | |

| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | Send data with the YYY simulator | Simulator displays "data sent" message |
| 2 | Open the relevant window in the XXX software | Sent data are displayed with date-time of reception |
| 3 | Press the run button | Data are processed; result is displayed and meets the expected value or range |

> **Example — Test (performance):** The following shows an example of a performance **Test** involving multiple users. Remove or replace it with actual tests.

| Field | Value | Notes |
|---|---|---|
| Test ID | T-SRS-REQ-005 | |
| Test description | Same description as in the Software Test Plan | |
| Verified requirement | TODO: SRS-REQ-005 | Test |
| Initial conditions | e.g. XXX Software is started | |
| Test inputs | N/A | |
| Data collection actions | Stopwatch | |
| Test outputs | N/A | |
| Assumptions and constraints | e.g. Users shall have received basic training to use the software | |
| Expected results and criteria | e.g. Results displayed in less than one minute | |

| Step | Operator actions | Expected result and evaluation criteria |
|---|---|---|
| 1 | For each of 3 users, run the main use scenario 3 times | Note the length of execution for each run of each user |
| 2 | Compute average length | Average length is less than 1 minute |
