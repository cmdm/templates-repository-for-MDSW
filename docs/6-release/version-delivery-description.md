# Version Delivery Description

## Table of Contents

> [!NOTE]
> Update this table of contents to match the final document structure

- [1. IDENTIFICATION](#1-identification)
  - [1.1 Document Overview](#11-document-overview)
  - [1.2 Abbreviations and Glossary](#12-abbreviations-and-glossary)
  - [1.3 References](#13-references)
  - [1.4 Conventions](#14-conventions)
- [2. Version Description](#2-version-description)
  - [2.1 Hardware Configuration](#21-hardware-configuration)
  - [2.2 Version Composition](#22-version-composition)
  - [2.3 Identification and Location of Software Bill of Materials – SBOM](#23-identification-and-location-of-software-bill-of-materials--sbom)
  - [2.4 Identification and Location of Master](#24-identification-and-location-of-master)
  - [2.5 Delivery Generation Procedure](#25-delivery-generation-procedure)
  - [2.6 Control of Private Keys](#26-control-of-private-keys)
- [3. Use of Version](#3-use-of-version)
  - [3.1 Version Content](#31-version-content)
  - [3.2 Restrictions of Use](#32-restrictions-of-use)
  - [3.3 Interface Compatibility](#33-interface-compatibility)
  - [3.4 Configuration Data](#34-configuration-data)
  - [3.5 Compatibility of Use](#35-compatibility-of-use)
  - [3.6 Integrity Control](#36-integrity-control)
  - [3.7 Installation Procedure](#37-installation-procedure)
  - [3.8 Use](#38-use)
  - [3.9 Uninstallation Procedure](#39-uninstallation-procedure)
- [4. Release Notes](#4-release-notes)
  - [4.1 Possible Problems](#41-possible-problems)
  - [4.2 Known Bugs](#42-known-bugs)
  - [4.3 Fixed Bugs](#43-fixed-bugs)

## 1. IDENTIFICATION

| Field | Value |
|---|---|
| Document ID | <!-- TODO: e.g. PRJ-VDD-001 --> |
| Title | Version Delivery Description |
| Version | <!-- TODO: e.g. 1.0 --> |
| Date | <!-- TODO: YYYY-MM-DD --> |
| Status | <!-- TODO: Draft / Under Review / Approved --> |

### 1.1 Document Overview

This document is the version description document of XXX system/software.

It describes:

- The identification of the version
- The hardware configuration
- The software configuration
- The documentation associated to this configuration
- The release notes

--8<-- "snippets/glossary-and-references.md"

## 2. Version Description

The XXX Vx.x alpha/beta/final version is the version issued after the XXX test/development/maintenance phase of the XXX software project. It was delivered the 20XX/MM/JJ from source control build Id ZZZ.

> [!NOTE]
> If this VDD is an update to an existing system, reference the VDD that this version replaces in §1.3.1.

### 2.1 Hardware Configuration

> [!NOTE]
> Describe the hardware configuration for the delivered version:
> - If software is embedded in a medical device, give relevant information to identify without error on which version of the medical device it runs.
> - If software runs on standard hardware (standalone software on PC), describe either the minimum hardware requirements (may already be in the user/installation manual) or the hardware specifications.
> - If software runs on a cloud system, describe if necessary the hardware resources (CPU, memory, disk).

### 2.2 Version Composition

The software components managed in configuration are listed in the table below:

| Name | Identifier | Configuration |
|---|---|---|
| DR Analyser — inference service | dr-analyser-inference | Git tag v1.0.0 on branch main, commit sha abc1234 |
| <!-- TODO: Component/package name --> | <!-- TODO: Component/package identification --> | <!-- TODO: Component identification in source control --> |
| <!-- TODO: Component/package name --> | <!-- TODO: Component/package identification --> | <!-- TODO: Component identification in source control --> |
| <!-- TODO: Component/package name --> | <!-- TODO: Component/package identification --> | <!-- TODO: Component identification in source control --> |

> [!TIP]
> You can also reference descriptor files such as `package.json`, `pom.xml`, or similar files. All referenced descriptor files shall contain a `version` tag.

#### 2.2.1 Dependencies

> [!NOTE]
> List the dependencies of the system that are NOT stored in the configuration management tool.

XXX is dependent on the following components which are not managed in configuration:

- Windows xxx, version 1.2.3.4
- Linux yyy, version 1.2.3.4, kernel version 1.2.3.4
- JRE xxx version 1.2.3.4
- Msvcrt xxx version 1.2.3.4
- Libc xxx version 1.2.3.4
- PDF viewer xxx version 1.2.3.4
- <!-- TODO: Any other external dependencies -->

> [!TIP]
> You can also reference a `dependencies.json` file, `pom.xml`, or similar file, including `devDependencies` if relevant. For cybersecurity reasons, fix exact version numbers rather than using version ranges.

#### 2.2.2 Software Components Stored in the Configuration Management Tool

> [!NOTE]
> List the dependencies of the system that ARE stored in the configuration management tool. It is your choice to determine what is stored in the configuration tool and what is not. Usually, libraries linked to your software are stored; external software tools and operating systems may or may not be.
>
> Even if you use tools like npm to retrieve dependencies, a strict and safe configuration management rule is to copy all software dependencies for a release version to a location managed by you.

The following COTS libraries are stored in the configuration management tool:

- <!-- TODO: Foo.jar version 1.2.3.4 -->
- <!-- TODO: Bar.dll version 1.2.3.4 -->

> [!NOTE]
> If common components developed by your company are reused, list them below:

The following common components developed by xxxx (your company) are used by XXX software:

- <!-- TODO: MyFoo.lib version 1.2.3.4 -->
- <!-- TODO: MyBar.lib version 1.2.3.4 -->

### 2.3 Identification and Location of Software Bill of Materials – SBOM

> [!NOTE]
> Add a reference to your SBOM file. See NTIA SBOM minimal elements for the required content.
> Example: The SBOM for this version is located at <!-- TODO: path or URL to SBOM file -->.

> [!NOTE]
> **NTIA SBOM Minimal Elements**
> Refer to the NTIA document *The Minimum Elements For a Software Bill of Materials (SBOM)* for the required fields. The SBOM shall at minimum identify all components, their versions, and their suppliers.

### 2.4 Identification and Location of Master

> [!NOTE]
> Describe where the master of this released version can be found.
>
> Examples:
> - Network share: `//master-share/path/to/master/master-version-x.y.z`
> - USB stick: XXX is delivered on a USB Stick generated from the delivery space of the configuration management tool.
>   - USB Stick Identifier: USB-XXX Vx.x alpha/beta/final
>   - Identifier generation rule: <!-- TODO: explain your unique identifier generation rule -->

### 2.5 Delivery Generation Procedure

> [!NOTE]
> Describe how the delivery media is generated.
>
> This is a delivery generation process — do not mix it with a production process. The goal of the procedure is to produce a master. The production of series or uploading of the master to a point of delivery or use (production server, app store, etc.) is outside the scope of this document.
>
> Example steps:
> 1. Software configuration tool extraction of source code
> 2. Build of software (provide further details if the build is complex)
> 3. Build of install package
> 4. Sign software and package
> 5. Copy install package bundle with external tool into master location

The media is generated <!-- TODO: manually / automatically by script --> with the following steps:

1. <!-- TODO -->
2. <!-- TODO -->
3. <!-- TODO -->
4. <!-- TODO -->
5. <!-- TODO -->

### 2.6 Control of Private Keys

> [!NOTE]
> Explain how private keys are stored and kept secure.
> Examples:
> - Keys used to sign the software package
> - API keys used by the software at runtime

## 3. Use of Version

### 3.1 Version Content

> [!NOTE]
> Select ONE of the following statements and complete it. Remove the others.

> [!NOTE]
> **Guidance — select the applicable statement**
>
> **For a test version:**
> XXX implements the requirements of SRS xxx for tests.
>
> **For an intermediate version:**
> XXX implements the requirements of SRS xxx, except those in §xxx, and except requirement #xxx and #yyy.
>
> **For the final operational version:**
> XXX fully implements the requirements of SRS xxx.

> [!NOTE]
> State which requirements are implemented by this version.

### 3.2 Restrictions of Use

> [!NOTE]
> Select the applicable restriction statement(s) and remove the others.

> [!NOTE]
> **Guidance — select the applicable statement**
>
> - XXX is for testing purposes only.
> - XXX is for clinical investigation.
> - XXX is for research purposes only.
> - XXX shall not be used for clinical purposes as long as it has not obtained the CE Marking, FDA clearance, or any equivalent approval in each country.

> [!NOTE]
> State any restrictions on the use of this version.

### 3.3 Interface Compatibility

> [!NOTE]
> Describe and provide the version identification of any system in interface with this version.
> You can reference a document that contains this information.

### 3.4 Configuration Data

> [!NOTE]
> Describe any specific configuration data added to this version.
> This configuration data may be located in a branch in the configuration management tool.

> Example: `xxx` configuration file contains settings for use with `yyy` hardware. File is located in `xxx` of the configuration management tool.

### 3.5 Compatibility of Use

> [!NOTE]
> List the OS and any other external tools required to run this version.
> This list is an extract of §2.2.1 and §2.2.2.

- Windows xxx
- <!-- TODO: PDF reader yyy -->

### 3.6 Integrity Control

> [!NOTE]
> Provide checksum, SHA-256 hash, or any equivalent mechanism to verify the integrity of the software.
> You can also ensure authenticity by distributing signed software.

| Artifact | Hash Algorithm | Hash Value |
|---|---|---|
| installer-vx.x.exe | SHA-256 | 123456ABCDEF hash value |

### 3.7 Installation Procedure

> [!NOTE]
> Describe the installation procedure, or reference the installation/user manual.
>
> Example: See the installation manual [Rx].

### 3.8 Use

> [!NOTE]
> Provide any relevant information for use of this version.
>
> Example: See the user manual [Rx].

### 3.9 Uninstallation Procedure

> [!NOTE]
> Describe the uninstallation procedure, or reference the uninstallation/user manual.
>
> Uninstallation shall include provisions for secure disposal of software, data, and personal data.

## 4. Release Notes

> [!NOTE]
> These are internal release notes, intended for development and test teams. They can be used as a basis for writing public release notes with simplified content for end users.

### 4.1 Possible Problems

> [!NOTE]
> Describe any possible problems that could arise and how to detect, avoid, or resolve them.
> Note: a problem is not necessarily a software bug — it may be a behaviour of the software when it is used outside its operational context.
>
> Example (embedded software): When the accessory is unplugged, the electronic card sends a saturation signal and the software displays the maximum value. The problem is in the electronic card and will be resolved in a future version. Ignore the displayed value when the accessory is unplugged.

### 4.2 Known Bugs

> [!NOTE]
> List the known bugs in this version.
> An extract from your bug tracker (e.g. Jira, GitHub Issues) is sufficient.

| Bug ID | Title | Severity | Workaround |
|---|---|---|---|
| BUG-042 | Confidence score display rounds to zero for values below 0.5 % | Low | Not required — display is cosmetic only; underlying inference result is unaffected |
| <!-- TODO: BUG-001 --> | <!-- TODO: Brief description --> | <!-- TODO: Low / Medium / High / Critical --> | <!-- TODO: Workaround if any --> |

### 4.3 Fixed Bugs

> [!NOTE]
> List the bugs fixed between this version and the previous version.
> An extract from your bug tracker is sufficient.

| Bug ID | Title | Severity | Fixed in Version |
|---|---|---|---|
| BUG-035 | Image upload fails silently when file size exceeds 20 MB | Medium | V1.0.0 |
| <!-- TODO: BUG-000 --> | <!-- TODO: Brief description --> | <!-- TODO: Low / Medium / High / Critical --> | <!-- TODO: Vx.x --> |
