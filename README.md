<p align="center">
  <a href="https://www.fenith.org/">
    <img src="fenith-logo.png" alt="FENITH" width="300">
  </a>
</p>

<h1 align="center">FENITH</h1>

<p align="center">
  <strong>Federated Learning in Ambienti Dinamici ed Eterogenei per la Sanità Digitale Europea:<br>Dal Framework Teorico all'Implementazione negli Ospedali Italiani</strong>
</p>

<p align="center">
  PhD Thesis — Fabio Liberti<br>
  <a href="https://www.fenith.org/">www.fenith.org</a>
</p>

---

## Overview

This repository serves as the central hub for the PhD research project on **Federated Learning (FL)** applied to the **European Health Data Space (EHDS)**. It aggregates all research artifacts — experimental platforms, domain-specific applications, governance frameworks, foundational studies, published papers, and thesis documents — into a single, structured meta-repository.

---

## Repository Structure

```
FENITH/
├── platforms/           # Experimental FL platforms
├── applications/        # Domain-specific FL applications
├── governance/          # Governance, policy, and ethical frameworks
├── foundations/         # Foundational research and educational materials
└── docs/
    ├── thesis/          # Thesis documents and outlines
    ├── papers/          # Published and submitted papers
    └── questionnaire/   # Survey research materials
```

---

## Platforms

| Repository | Description | Stack |
|---|---|---|
| [flopbg](https://github.com/FabioLiberti/flopbg) | FL research platform — Universitas Mercatorum & Ospedale Pediatrico Bambino Gesù. 12 FL algorithms, 11 datasets (5 benchmark + 6 clinical). | Python, Flask, TensorFlow, React |
| [BLEKFL2](https://github.com/FabioLiberti/BLEKFL2) | FL research platform — Blekinge Institute of Technology (Sweden) & Universitas Mercatorum. 17+ FL algorithms, Flower framework. | Python, Flask, PyTorch, Flower |
| [FL-EHDS-FLICS2026](https://github.com/FabioLiberti/FL-EHDS-FLICS2026) | FL + EHDS governance framework. 17 FL algorithms, 19 healthcare datasets, differential privacy, secure aggregation. | Python |

## Applications

| Repository | Description | Domain |
|---|---|---|
| [Questionnaire_FL](https://github.com/FabioLiberti/Questionnaire_FL) | Research questionnaire on FL adoption in Italian hospitals. 34 questions, systematic literature review. | Healthcare Adoption |
| [CIDE](https://github.com/FabioLiberti/CIDE) | Federated Learning Health Data Platform - OMOP/FHIR business models for European digital health research networks (EHDS). | Digital Health / Business Models |
| [CIDE2](https://github.com/FabioLiberti/CIDE2) | Explainable Federated Learning for secure telemedicine — privacy-preserving deepfake detection in digital health platforms. | Digital Health / XAI |
| [FedHR5.0](https://github.com/FabioLiberti/FedHR5.0) | Privacy-preserving Federated Learning framework for Human Resource Management in Industry 5.0. | HR / Industry 5.0 |
| [CRISTAIN2025](https://github.com/FabioLiberti/CRISTAIN2025) | FA-FedAvg — Forensic-Aware Federated Averaging for law enforcement inter-agency collaboration. | Criminal Justice |

## Governance

| Repository | Description | Focus |
|---|---|---|
| [AI-DIGOSA](https://github.com/FabioLiberti/AI-DIGOSA) | Multidimensional framework analyzing tensions between norms, ethics, and innovation in distributed AI healthcare. | Ethics & Regulation |
| [icsis2026](https://github.com/FabioLiberti/icsis2026) | FL as policy data infrastructure for territorial healthcare planning in aging European regions (EHDS). | Health Policy |
| [ICID2026](https://github.com/FabioLiberti/ICID2026) | Three-layered reference architecture for deploying FL within EHDS — IDSA, Data Mesh, hierarchical FL. | Architecture & Standards |

## Foundations

| Repository | Description | Type |
|---|---|---|
| [DHFLPL2](https://github.com/FabioLiberti/DHFLPL2) | Foundational paper — MDPI Applied Sciences 2024 (21 citations). Systematized evolution of the FL research platform. | Seminal · P-M |
| [DHFLPL](https://github.com/FabioLiberti/DHFLPL) | Original repo referenced in the published paper (v1). | Legacy · P-M |
| [Heterogeneous_Federated_Learning](https://github.com/FabioLiberti/Heterogeneous_Federated_Learning) | Curated collection of educational materials on heterogeneous FL (2020+). | Educational |
| tesi_fl_2025 | Thesis core repository. | Private |
| HFEDL_Project | Heterogeneous FL research project. | Private |

---

## Publications

| Code | Title / Conference | Year | Repository |
|---|---|---|---|
| P-M | MDPI Applied Sciences (21 citations) | 2024 | [DHFLPL2](https://github.com/FabioLiberti/DHFLPL2) · ([v1](https://github.com/FabioLiberti/DHFLPL)) |
| P-IS | ISM 2025 | 2025 | [FedHR5.0](https://github.com/FabioLiberti/FedHR5.0) |
| P-CR | CRISTAIN 2025 | 2025 | [CRISTAIN2025](https://github.com/FabioLiberti/CRISTAIN2025) |
| P-C1 | CIDE 2025 (FL) | 2025 | [CIDE](https://github.com/FabioLiberti/CIDE) |
| P-C2 | CIDE 2025 (FL + XAI DeepFake) | 2025 | [CIDE2](https://github.com/FabioLiberti/CIDE2) |
| P-IT | ITAIS 2025 | 2025 | [AI-DIGOSA](https://github.com/FabioLiberti/AI-DIGOSA) |
| IFKAD | IFKAD 2026 (FedHR5.0) | 2026 | *Repo TBD* |
| ICID | ICID 2026 | 2026 | [ICID2026](https://github.com/FabioLiberti/ICID2026) |
| ICSIS | ICSIS 2026 | 2026 | [icsis2026](https://github.com/FabioLiberti/icsis2026) |
| FLICS | FLICS 2026 (FL + EHDS) | 2026 | [FL-EHDS-FLICS2026](https://github.com/FabioLiberti/FL-EHDS-FLICS2026) |

---

## Getting Started

This meta-repository uses **Git submodules** to link all component repositories.

```bash
# Clone with all submodules
git clone --recurse-submodules https://github.com/FabioLiberti/FENITH.git

# If already cloned, initialize submodules
git submodule update --init --recursive
```

> **Note:** Some submodules (`tesi_fl_2025`, `HFEDL_Project`) are private repositories. Access requires appropriate GitHub permissions.

---

## License

This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

Individual submodules may have their own licenses — refer to each repository for details.

---

## Author

**Fabio Liberti**
PhD Candidate — Universitas Mercatorum, Rome, Italy

---
