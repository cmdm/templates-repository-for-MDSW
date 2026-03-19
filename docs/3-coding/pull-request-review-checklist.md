# Pull Request Review Checklist

> [!NOTE]
> **Purpose of this template**
> This template is used as a **pull request comment** to record that the assigned reviewer evaluated the changes against established review criteria before the PR is merged. One completed checklist per PR reviewer is expected. The filled-in comment constitutes objective evidence that a code review was performed, as required by IEC 62304 §5.5.

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
> 2. REVIEW GUIDELINES
>    2.1 Code Clarity
>    2.2 Code Comments
>    2.3 Code Maintainability
>    2.4 Suitable Implementation of Software Units
>    2.5 Handling Deviations
> 3. PR CHECKLIST

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-PRRC-001 --> |
| Title | Pull Request Review Checklist |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document defines the review guidelines and the checklist template used by reviewers when evaluating a pull request (PR) for the <!-- TODO: project name --> software development project.

The guidelines in §2 describe what reviewers should look for. The checklist in §3 is a concise comment template that reviewers copy into each PR to record the outcome of their review.

**Scope:** This checklist applies to every pull request that introduces changes to software units or their associated unit verification artifacts.

**Intended audience:** Software developers, software quality assurance, software project manager.

--8<-- "snippets/glossary-and-references.md"

## 2. REVIEW GUIDELINES

This section describes what reviewers should assess when examining a pull request. The four areas below correspond directly to the four checklist criteria in §3.

### 2.1 Code Clarity

Code should be immediately understandable to a developer who did not write it. Reviewers should check that:

- Functions and methods are short enough to read in one screen. A function that requires scrolling to understand is a candidate for splitting.
- Names of variables, functions, types, and modules are descriptive and unambiguous. Single-letter or cryptic abbreviations are acceptable only in well-established local conventions (e.g. loop indices, mathematical notation matching a specification).
- Control flow is as simple as the problem allows. Deeply nested conditionals, implicit fall-throughs, and non-obvious short-circuit logic should be refactored or at minimum commented.
- There is no dead code (unreachable branches, unused variables, commented-out blocks) left in the change. If code is deliberately disabled, it must be accompanied by a comment explaining why and referencing a ticket.

### 2.2 Code Comments

Comments should explain **why** the code does something, not restate **what** it does. Reviewers should check that:

- Non-obvious design decisions, algorithmic choices, and workarounds are explained inline. A reader should not need to trace the full call stack or read the specification to understand the intent of a function.
- Public APIs (functions, classes, modules) that will be called by other units carry documentation comments (docstrings, Doxygen, JSDoc, or equivalent) describing their contract: purpose, parameters, return value, and any exceptions or error conditions.
- Safety-critical or security-sensitive sections are marked clearly so that future maintainers know to treat them with extra care (e.g. `// SAFETY: ...` or `// SECURITY: ...` annotation conventions as defined in the project coding standards).
- TODO or FIXME comments reference a ticket number and must not be introduced for known defects that must be fixed before the unit is accepted.

### 2.3 Code Maintainability

The change should leave the codebase in a state that is easier, or at least no harder, to maintain than before. Reviewers should check that:

- The change follows the coding standards and style guide defined in the Software Development Plan (naming conventions, formatting, forbidden constructs, complexity limits). Automated formatters and linters are the first line of enforcement; the review focuses on what tooling cannot catch.
- Magic numbers and hard-coded strings are replaced by named constants or configuration values, unless their meaning is self-evident from context.
- Logic that is used in more than one place is extracted into a shared function or module rather than duplicated.
- Error conditions and boundary cases are handled explicitly. The code must not silently swallow exceptions, ignore error return values, or rely on undefined behaviour. Each error path should either recover gracefully or propagate the failure in a way the caller can handle.
- Dependencies on external libraries or components are introduced only when justified and are consistent with the dependency management policy in the Software Development Plan.

### 2.4 Suitable Implementation of Software Units

> [!NOTE]
> **IEC 62304 §5.5.1, §5.5.2, §5.5.3, §5.5.4, and §5.5.5**
> Each software unit shall be implemented in accordance with the detailed design. Verification procedures and acceptance criteria shall exist for each unit. For Class C software, §5.5.4 imposes additional unit acceptance criteria.

Beyond code style, the reviewer must assess whether the implementation is technically correct and appropriately verified:

- The changes implement what is specified in the Software Design Specification (SDS) or in an approved design change record. The interfaces (function signatures, data structures, APIs, communication protocols) of new or modified units match their specification.
- Unit tests or other unit verification procedures have been added or updated to cover every new or modified software unit. Acceptance criteria are objective and have an unambiguous pass/fail condition. All tests pass.
- No existing unit tests have been disabled, skipped, or deleted without a documented rationale.
- For **Class C software**, the additional unit acceptance criteria of IEC 62304 §5.5.4 are satisfied: the unit has been evaluated for correct operation across its full range of inputs and boundary conditions, and the applicable structural coverage level (branch coverage or MC/DC as required by the project) has been achieved and recorded.
- The change does not introduce safety hazards or violate safety constraints identified in the risk management documentation, and does not introduce security vulnerabilities (e.g. injection flaws, insecure data handling, unvalidated inputs at system boundaries, hard-coded credentials).

### 2.5 Handling Deviations

> [!WARNING]
> **Deviations must be tracked**
> If any review criterion in §3 is not satisfied, the reviewer **must** choose one of the following actions. Simply noting a concern without taking action is not acceptable.
>
> 1. **Refuse the PR** — request changes and do not approve until the criterion is fully met. This is the default action for any criterion that affects correctness, safety, security, or regulatory compliance.
> 2. **Open a deviation record** — if the team agrees that merging is acceptable despite the deviation, a formal record must be opened before or at the time of approval:
>     - An **anomaly ticket** in the project issue tracker for deviations from coding standards, unit verification procedures, or implementation correctness.
>     - A **safety risk item** in the risk management file if the deviation could affect a safety control measure or introduces a potential hazard.
>     - A **security risk item** in the security risk register if the deviation affects a security control or introduces a potential vulnerability.
>
> The PR comment must reference the ticket or risk item number. Merging without one of these two actions is not permitted.

---

## 3. PR CHECKLIST

> [!TIP]
> Copy the table below (from the horizontal rule onwards) and paste it as a pull request comment.

---

For each criterion: **OK** — satisfied · **Deviation** — not fully satisfied (see §2.5: PR refused or deviation record opened and referenced in the PR) · **N/A** — not applicable (justify).

| # | Criterion | Verdict | Notes |
|---|---|---|---|
| RC-01 | The code follows the project coding guidelines (clarity, comments, maintainability, coding standards). | <!-- OK / Deviation / N/A --> | |
| RC-02 | Static source code analysis and all other automated tools (linters, formatters, security scanners) pass without new unresolved findings. | <!-- OK / Deviation / N/A --> | |
| RC-03 | The code implements the software units as specified in the design, with adequate unit verification (tests added/updated, all tests pass, acceptance criteria defined and met). | <!-- OK / Deviation / N/A --> | |
| RC-04 | The additional unit acceptance criteria of IEC 62304 §5.5.4 are fulfilled (Class C software only; mark N/A with justification for Class A/B). | <!-- OK / Deviation / N/A --> | |
