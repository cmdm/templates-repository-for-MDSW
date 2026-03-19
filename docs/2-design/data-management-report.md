# Data Management Report

## Table of Contents

> **Note:** Update this table of contents to reflect the sections in this document.
> In the MkDocs web view, the table of contents is generated automatically in the sidebar.
> This section is intended for printed or exported (PDF) versions of the document.
>
> 1. IDENTIFICATION
>    1.1 Document Overview
>    1.2 Abbreviations and Glossary
>    1.3 References
>    1.4 Conventions
> 2. DATA ACQUISITION SUMMARY
> 3. DATASET XXX
>    3.1 Data Sources
>    3.2 Traceability
>    3.3 Privacy and Security
>    3.4 Regulatory Compliance
>    3.5 Data Annotation
>    3.6 Data Preparation Operations
>    3.7 Data Quality Model Results
>    3.8 Dataset Provisioning
> 4. DATASET YYY

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-DMR-001 --> |
| Title | Data Management Report |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document contains the data management report for XXX device and YYY dataset(s). It contains the records of steps performed to provide data for training / tuning / AI validation / AI test of the AI system integrated in XXX medical device.

--8<-- "snippets/glossary-and-references.md"

## 2. Data Acquisition Summary

> **Note:** OPTIONAL: Add a summary of data acquisition activities described in the dataset sections below.

<!-- TODO: Summarize the overall data acquisition activities across all datasets, or remove this section if not needed. -->

## 3. Dataset XXX

> **Note:** Replace "XXX" in this section heading with the actual dataset name or identifier.

### 3.1 Data Sources

> **Note:** For each dataset provided to the AI model design, describe or reference data sources. Examples of source types include:
>
> - Anonymized or pseudonymized data
> - Off-the-shelf registries or databases (secondary use of clinical data) maintained by third parties
> - Retrospective clinical studies (secondary use of clinical data)
> - Clinical data from a register built in PMCF of another manufacturer's device (secondary use of clinical data)
> - Clinical investigation results
> - Other

<!-- TODO: Describe or reference the data sources used for this dataset. -->

### 3.2 Traceability

> **Note:** Describe or reference artifacts providing traceability to data sources, especially for datasets built from multiple sources. Include:
>
> - Origin of data
> - Version of original data
> - Traceability artifacts, such as DVC records

<!-- TODO: Describe or reference traceability artifacts for this dataset. -->

### 3.3 Privacy and Security

> **Note:** If applicable, describe or reference documents giving evidence of data privacy and security. Such documents may have been referenced in the data management plan and left unchanged until this report is issued.

<!-- TODO: Describe or reference privacy and security evidence, or mark as N/A if not applicable. -->

### 3.4 Regulatory Compliance

> **Note:** If applicable, describe or reference documents giving evidence of regulatory compliance. Examples include:
>
> - Presence of patient consent
> - Appropriate methods of anonymisation

<!-- TODO: Describe or reference regulatory compliance evidence, or mark as N/A if not applicable. -->

### 3.5 Data Annotation

> **Note:** Describe or reference documents containing:
>
> - Evidence of qualification of annotators
> - Annotation quality metrics
> - Deviations in the annotation process and their impact on clinical validity of data

<!-- TODO: Describe or reference annotation evidence for this dataset. -->

### 3.6 Data Preparation Operations

> **Note:** Describe or reference documents containing:
>
> - Operations performed: aggregation, sampling, augmentation, imputation, splitting, normalization, etc.
> - Why such operations were performed
> - The impact or absence of impact on clinical validity of data

<!-- TODO: Describe or reference data preparation operations applied to this dataset. -->

### 3.7 Data Quality Model Results

> **Note:** Describe or reference documents containing:
>
> - A statistical description of the dataset:
>     - Bringing evidence of representativeness and absence of bias
>     - Supporting the data quality model
> - Data quality model results, for example:
>     - Data completion measured to 99.5%
>     - Anomalies detected and remediation actions taken

<!-- TODO: Describe or reference data quality model results for this dataset. -->

### 3.8 Dataset Provisioning

> **Note:** Provide the dataset identification details:
>
> - Identifier
> - Version
> - Date of provisioning
> - Repository where it is stored
> - Optionally, dataset integrity (e.g. SHA checksum)
>
> Additionally, add evidence of AI test dataset segregation from AI training / AI validation datasets.

| Field | Value |
|---|---|
| Identifier | <!-- TODO: Dataset identifier --> |
| Version | <!-- TODO: Dataset version --> |
| Date of Provisioning | <!-- TODO: YYYY-MM-DD --> |
| Repository | <!-- TODO: Repository URL or reference --> |
| Integrity (optional) | <!-- TODO: e.g. SHA-256: abc123... --> |

<!-- TODO: Add evidence of AI test dataset segregation from AI training / AI validation datasets. -->

## 4. Dataset YYY

> **Note:** Replace "YYY" in this section heading with the actual dataset name or identifier. Repeat the pattern of section 3 for each additional dataset. Add further sections (5, 6, …) as needed.
