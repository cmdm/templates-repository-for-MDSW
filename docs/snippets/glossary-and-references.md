### 1.2 Abbreviations and Glossary

#### 1.2.1 Abbreviations

| Abbreviation | Definition |
|---|---|
| IEC | International Electrotechnical Commission |
| SRS | Software Requirements Specification |
| SW | Software |
| <!-- TODO --> | <!-- TODO --> |

#### 1.2.2 Glossary

| Term | Definition |
|---|---|
| AI Training | The process of fitting a machine learning model to a dataset by optimising model parameters (e.g. weights) so that the model learns to perform a target task. Training uses a dedicated training dataset and is performed during development, before deployment. |
| AI Validation | Confirmation, through objective evidence, that an AI/ML model meets the requirements for its intended use within its intended operating environment. AI validation is concerned with the correctness and fitness-for-purpose of the model itself (e.g. performance metrics on a held-out test set or in a clinical study). In common practice, the training and validation datasets are derived from the same source dataset, typically split 80 % for training and 20 % for validation. |
| AI Test | The systematic evaluation of an AI/ML model against defined acceptance criteria using a test dataset that is independent from the training and validation datasets. AI testing verifies that the model generalises correctly and meets performance thresholds prior to integration into the medical device software. |
| Medical Device Verification | Confirmation, through the provision of objective evidence, that specified requirements have been fulfilled (ISO 9000). In the context of IEC 62304, verification demonstrates that each software development output conforms to its input requirements (e.g. code review, unit testing, integration testing). |
| Medical Device Validation | Confirmation, through the provision of objective evidence, that the requirements for a specific intended use or application have been fulfilled (ISO 9000). In the context of medical device software, validation demonstrates that the complete device (including software) meets user needs and its intended purpose under real-world or simulated-use conditions. |
| <!-- TODO: Term --> | <!-- TODO: Definition --> |

> [!WARNING]
> **AI Validation vs. Medical Device Validation**
> These two terms use the word *validation* with different meanings and must not be confused:
>
> - **AI Validation** is a machine-learning engineering activity. It evaluates whether a trained model is accurate and fit for its modelling task, typically by measuring performance metrics (e.g. AUC, sensitivity, specificity) on a held-out validation dataset. It is an internal development activity performed by data scientists or ML engineers.
> - **Medical Device Validation** is a regulatory and quality-system activity defined by ISO 9000 and required by IEC 62304 / ISO 13485. It demonstrates that the finished medical device (hardware + software) satisfies user needs and its intended clinical purpose under real-use or simulated-use conditions. It is the final stage of the device development lifecycle and forms part of the design validation evidence submitted to regulatory authorities.
>
> A model that has been *AI validated* (good benchmark performance) still requires *medical device validation* (clinical / usability evidence) before the device can be placed on the market.

### 1.3 References

#### 1.3.1 Project References

| Ref | Document Title | Document ID | Version |
|---|---|---|---|
| [P-01] | Software Development Procedure | PRJ-PROC-001 | 1.0 |
| <!-- TODO: [P-02] --> | <!-- TODO: Document title --> | <!-- TODO: DOC-ID --> | <!-- TODO: 1.0 --> |

#### 1.3.2 Standard References

| Ref | Title | Edition |
|---|---|---|
| [ISO 13485] | Medical devices — Quality management systems — Requirements for regulatory purposes | 2016 |
| [ISO 14971] | Medical devices — Application of risk management to medical devices | 2019 |
| [IEC 62304] | Medical device software — Software life cycle processes | 2006+AMD1:2015 |
| [IEC 81001-5-1] | Health software and health IT systems safety, effectiveness and security — Part 5-1: Security — Activities in the product life cycle | 2021 |
| [IEC 82304-1] | Health software — Part 1: General requirements for product safety | 2016 |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

#### 1.3.3 Regulatory References

| Ref | Title | Edition |
|---|---|---|
| [FDA-SW] | Content of Premarket Submissions for Device Software Functions | Sep 2022 |
| [FDA-CS] | Cybersecurity in Medical Devices: Quality System Considerations and Content of Premarket Submissions | Feb 2026 |
| <!-- TODO --> | <!-- TODO --> | <!-- TODO --> |

### 1.4 Conventions

> [!NOTE]
> Describe any document conventions used in this document, for example:
> - Text formatting (bold for defined terms, italic for references)
> - Status codes or classification tags
> - Notation used in tables or diagrams
