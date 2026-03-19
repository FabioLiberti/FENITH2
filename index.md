---
layout: default
title: FENITH
description: Federated Learning in Dynamic and Heterogeneous Environments for European Digital Healthcare
---

# FENITH

**Federated Learning in Dynamic and Heterogeneous Environments for European Digital Healthcare: From Theoretical Framework to Implementation in Italian Hospitals**

PhD Thesis — [Fabio Liberti](https://www.fabioliberti.com/) · [ORCID](https://orcid.org/0000-0003-3019-5411) · [Google Scholar](https://scholar.google.com/citations?user=ce_iUyEAAAAJ&hl=it)

---

## Overview

This repository serves as the central hub for the PhD research project on **Federated Learning (FL)** applied to the **European Health Data Space (EHDS)**. It aggregates all research artifacts — experimental platforms, domain-specific applications, governance frameworks, foundational studies, published papers, and thesis documents — into a single, structured meta-repository.

## Research Questions

| | Question | Cluster |
|---|---|---|
| **RQ1** | **Technological Framework** — How to design FL architectures capable of handling heterogeneity of hospital nodes? | Platforms |
| **RQ2** | **Multidimensional Governance** — Which governance models balance innovation, compliance, and ethics? | Governance |
| **RQ3** | **Practical Adoption** — What are the barriers and enablers for FL adoption in Italian hospitals? | Applications |
| **RQ4** | **EHDS Interoperability** — How to integrate FL with HL7/FHIR, OMOP/OHDSI standards? | Platforms · Governance |

## At a Glance

| | |
|---|---|
| **FL Algorithms** | 38 unique across 3 platforms |
| **Datasets** | 35 total — benchmark, clinical imaging, healthcare |
| **Publications** | 10 papers — 1 published (21 citations), 3 presented, 2 accepted, 4 submitted |
| **Submodules** | 16 repositories (14 public + 2 private) |
| **Frameworks** | TensorFlow, PyTorch, Flower, Flask, React |

## Repository Clusters

### Platforms

| Repository | Description | Stack |
|---|---|---|
| [flopbg](https://github.com/FabioLiberti/flopbg) | FL platform — Universitas Mercatorum & OPBG | Python, TensorFlow, React |
| [BLEKFL2](https://github.com/FabioLiberti/BLEKFL2) | FL platform — BTH & Universitas Mercatorum | Python, PyTorch, Flower |
| [FL-EHDS-FLICS2026](https://github.com/FabioLiberti/FL-EHDS-FLICS2026) | FL + EHDS governance framework | Python |

### Applications

| Repository | Description | Domain |
|---|---|---|
| [Questionnaire_FL](https://github.com/FabioLiberti/Questionnaire_FL) | FL adoption questionnaire — Italian hospitals | Healthcare Adoption |
| [CIDE](https://github.com/FabioLiberti/CIDE) | OMOP/FHIR business models for EHDS | Digital Health |
| [CIDE2](https://github.com/FabioLiberti/CIDE2) | XAI deepfake detection in telemedicine | XAI |
| [FedHR5.0](https://github.com/FabioLiberti/FedHR5.0) | FL for HR Management in Industry 5.0 | HR |
| [CRISTAIN2025](https://github.com/FabioLiberti/CRISTAIN2025) | FA-FedAvg for law enforcement | Criminal Justice |

### Governance

| Repository | Description | Focus |
|---|---|---|
| [AI-DIGOSA](https://github.com/FabioLiberti/AI-DIGOSA) | Norms, ethics, and innovation tensions | Ethics & Regulation |
| [icsis2026](https://github.com/FabioLiberti/icsis2026) | FL for territorial healthcare planning | Health Policy |
| [ICID2026](https://github.com/FabioLiberti/ICID2026) | Three-layered FL architecture for EHDS | Architecture |

### Foundations

| Repository | Description | Type |
|---|---|---|
| [DHFLPL2](https://github.com/FabioLiberti/DHFLPL2) | Foundational paper — MDPI 2024 (21 citations) | Seminal |
| [DHFLPL](https://github.com/FabioLiberti/DHFLPL) | Original published paper repo (v1) | Legacy |
| [Heterogeneous_FL](https://github.com/FabioLiberti/Heterogeneous_Federated_Learning) | Educational materials on heterogeneous FL | Educational |

## Publications

| Code | Title | Venue | Year | Status |
|---|---|---|---|---|
| P-M | Federated Learning in Dynamic and Heterogeneous Environments | MDPI Applied Sciences · [DOI](https://doi.org/10.3390/app14188490) | 2024 | Published |
| P-IS | FedHR5.0: Privacy-Preserving HR Management in Industry 5.0 | ISM 2025 | 2025 | Accepted |
| P-CR | FA-FedAvg: Forensic-Aware Federated Averaging | CRISTAIN 2025 | 2025 | Accepted |
| P-C1 | Business Models for European Digital Health Research Networks | CIDE 2025 | 2025 | Presented |
| P-C2 | Explainable FL for Secure Telemedicine | CIDE 2025 | 2025 | Presented |
| P-IT | AI Distribuita e Governance Sanitaria | ITAIS 2025 | 2025 | Presented |
| FLICS | FL + EHDS Governance Framework | FLICS 2026 — IEEE | 2026 | Submitted |
| ICSIS | FL as Policy Data Infrastructure | ICSIS 2026 | 2026 | Submitted |
| ICID | Three-Layered Reference Architecture for FL within EHDS | ICID 2026 — Springer | 2026 | Submitted |
| IFKAD | FedHR5.0: FL for Knowledge Asset Dynamics | IFKAD 2026 | 2026 | Submitted |

## Getting Started

```bash
git clone --recurse-submodules https://github.com/FabioLiberti/FENITH2.git
git submodule update --remote --merge
```

## Citation

If you use this work, please cite:

> Liberti, F.; Berardi, D.; Martini, B. *Federated Learning in Dynamic and Heterogeneous Environments.* Applied Sciences 2024, 14(18), 8490. [DOI: 10.3390/app14188490](https://doi.org/10.3390/app14188490)

---

[View full README on GitHub](https://github.com/FabioLiberti/FENITH2) · [www.fenith.org](https://www.fenith.org/) · License: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
