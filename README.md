<p align="center">
  <a href="https://www.fenith.org/">
    <img src="fenith-logo.png" alt="FENITH" width="300">
  </a>
</p>

<h1 align="center">FENITH</h1>

<p align="center">
  <strong>Federated Learning in Dynamic and Heterogeneous Environments for European Digital Healthcare:<br>From Theoretical Framework to Implementation in Italian Hospitals</strong>
</p>

<details align="center">
<summary><em>Titolo originale (IT)</em></summary>
<p><strong>Federated Learning in Ambienti Dinamici ed Eterogenei per la Sanità Digitale Europea:<br>Dal Framework Teorico all'Implementazione negli Ospedali Italiani</strong></p>
</details>

<p align="center">
  PhD Thesis — Fabio Liberti<br>
  <a href="https://www.fenith.org/">www.fenith.org</a>
</p>

<p align="center">
  <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg" alt="License"></a>
  <img src="https://img.shields.io/badge/Submodules-16-blue" alt="Submodules">
  <img src="https://img.shields.io/badge/Papers-10-green" alt="Papers">
  <img src="https://img.shields.io/github/last-commit/FabioLiberti/FENITH2" alt="Last Commit">
</p>

---

## Overview

This repository serves as the central hub for the PhD research project on **Federated Learning (FL)** applied to the **European Health Data Space (EHDS)**. It aggregates all research artifacts — experimental platforms, domain-specific applications, governance frameworks, foundational studies, published papers, and thesis documents — into a single, structured meta-repository.

---

## Research Questions

| | Question | Cluster |
|---|---|---|
| **RQ1** | **Technological Framework** — How to design Federated Learning architectures capable of handling the high statistical, infrastructural, and participation heterogeneity of hospital nodes, while ensuring scalability, efficiency, and reliability of distributed training? | Platforms |
| **RQ2** | **Multidimensional Governance** — Which governance models can balance technological innovation, regulatory compliance (GDPR/EHDS), economic sustainability, and socio-ethical principles, enabling federated trust networks in healthcare? | Governance |
| **RQ3** | **Practical Adoption** — What are the main barriers and enabling conditions for the effective adoption of Federated Learning in Italian hospitals, in technological, organizational, and cultural terms? | Applications |
| **RQ4** | **EHDS Interoperability** — How can Federated Learning be integrated with international healthcare standards (HL7/FHIR, OMOP/OHDSI) to ensure full compatibility with the European Health Data Space? | Platforms · Governance |

<details>
<summary><em>Research Questions (IT)</em></summary>

| | Domanda | Cluster |
|---|---|---|
| **RQ1** | **Framework Tecnologico** — Come progettare architetture di Federated Learning in grado di gestire l'elevata eterogeneità statistica, infrastrutturale e di partecipazione dei nodi ospedalieri, assicurando scalabilità, efficienza e affidabilità del training distribuito? | Platforms |
| **RQ2** | **Governance Multidimensionale** — Quali modelli di governance possono bilanciare innovazione tecnologica, conformità normativa (GDPR/EHDS), sostenibilità economica e principi etico-sociali, abilitando reti federate di fiducia nel contesto sanitario? | Governance |
| **RQ3** | **Adozione Pratica** — Quali sono le principali barriere e condizioni abilitanti per l'adozione effettiva del Federated Learning negli ospedali italiani, in termini tecnologici, organizzativi e culturali? | Applications |
| **RQ4** | **Interoperabilità EHDS** — In che modo il Federated Learning può essere integrato con gli standard sanitari internazionali (HL7/FHIR, OMOP/OHDSI) per garantire la piena compatibilità con l'EHDS? | Platforms · Governance |

</details>

---

> See the full [architecture diagram](docs/architecture.md) for a visual overview.

<p align="center">
  <img src="FENITH_Diagram.png" alt="FENITH Diagram" width="48%">
  &nbsp;
  <img src="FENITH_Infographic.png" alt="FENITH Infographic" width="48%">
</p>

<p align="center">
  <em>Left: Research architecture — mapping of platforms, applications, governance, and foundations.<br>
  Right: Project infographic — timeline, publications, and key contributions overview.</em>
</p>

---

## At a Glance

| | |
|---|---|
| **FL Algorithms** | 30+ implemented across 3 platforms (FedAvg, FedProx, SCAFFOLD, ...) |
| **Datasets** | 35 total — 5 benchmark, 6 clinical imaging, 19 healthcare (+ 5 shared) |
| **Experiments** | 6,000+ (FL-EHDS-FLICS2026 alone) |
| **Publications** | 10 papers — 1 published (21 citations), 3 presented, 2 pending, 4 submitted |
| **Conferences** | MDPI, ISM, CRISTAIN, CIDE, ITAIS, FLICS, ICSIS, ICID, IFKAD |
| **Submodules** | 16 repositories (14 public + 2 private) |
| **Frameworks** | TensorFlow, PyTorch, Flower, Flask, React |

---

## Timeline

```mermaid
gantt
    title FENITH Research Timeline
    dateFormat YYYY-MM
    axisFormat %b %Y

    section Foundations
    Heterogeneous FL study           :done, 2023-10, 2024-06
    P-M MDPI Applied Sciences        :done, pm, 2024-06, 2024-09
    DHFLPL platform (v1)             :done, 2024-03, 2024-09
    DHFLPL2 systematization          :done, 2024-09, 2025-03

    section 2025 Conferences
    P-IT ITAIS 2025                  :done, 2025-03, 2025-06
    P-IS ISM 2025 (Malta)            :done, 2025-06, 2025-11
    P-CR CRISTAIN 2025 (CHItaly)     :done, 2025-06, 2025-10
    P-C1 CIDE 2025 (Ploiesti)       :done, 2025-07, 2025-10
    P-C2 CIDE 2025 (XAI DeepFake)   :active, 2025-07, 2025-10
    Questionnaire FL Italian Hospitals :done, 2024-11, 2025-07

    section Platforms
    flopbg (Bambino Gesù)            :done, 2024-09, 2026-03
    BLEKFL2 (Blekinge)               :done, 2025-07, 2026-03
    FL-EHDS-FLICS2026                :done, 2026-01, 2026-03

    section 2026 Submissions
    FLICS 2026 (Valencia, IEEE)      :active, 2026-01, 2026-06
    ICSIS 2026 (Valencia)            :active, 2026-01, 2026-06
    ICID 2026 (Ulaanbaatar, Springer):active, 2026-01, 2026-05
    IFKAD 2026 (Budapest)            :active, 2026-01, 2026-07

    section Thesis
    FENITH meta-repo                 :active, 2026-03, 2026-09
    PhD Thesis writing               :active, 2026-03, 2026-12
```

---

## Datasets

<details>
<summary><strong>35 datasets across 3 platforms</strong> (click to expand)</summary>

### Benchmark (5) — shared across flopbg & BLEKFL2

| Dataset | Samples | Classes | Format |
|---|---|---|---|
| MNIST | 70,000 | 10 | 28x28 grayscale |
| Fashion-MNIST | 70,000 | 10 | 28x28 grayscale |
| CIFAR-10 | 60,000 | 10 | 32x32 RGB |
| CIFAR-100 | 60,000 | 100 | 32x32 RGB |
| SVHN | 99,289 | 10 | 32x32 RGB |

### Clinical Imaging (6) — flopbg

| Dataset | Domain | Classes | Platform |
|---|---|---|---|
| Brain Tumor MRI | Neuro-imaging | 4 (glioma, meningioma, pituitary, no tumor) | flopbg |
| ISIC Skin Lesion | Dermatology | 9 (melanoma, nevus, BCC, ...) | flopbg |
| Chest X-Ray | Radiology | 2 (normal, pneumonia) | flopbg |
| Diabetic Retinopathy | Ophthalmology | 5 (no DR — proliferative) | flopbg |
| Skin Cancer | Dermatology | 2 (benign, malignant) | flopbg |
| Brain Tumor (Alt.) | Neuro-imaging | 4 | flopbg |

### Healthcare (19) — FL-EHDS-FLICS2026

**Primary evaluated (8)**

| Dataset | Domain | Samples | Compliance |
|---|---|---|---|
| PTB-XL ECG | Cardiology | 21,799 | 52 EU sites |
| Cardiovascular Disease | Cardiology | 70,000 | — |
| Diabetes 130-US Hospitals | Endocrinology/EHR | 101,766 | ICD-9 |
| Heart Disease UCI | Cardiology | 920 | 4 hospitals |
| Breast Cancer Wisconsin | Oncology | 569 | — |
| Chest X-Ray | Radiology | 5,856 | DICOM |
| Brain Tumor MRI | Neuro-imaging | 7,023 | DICOM |
| Skin Cancer (ISIC) | Dermatology | 3,297 | DICOM |

**Additionally supported (11)**

| Dataset | Domain | Samples | Compliance |
|---|---|---|---|
| Stroke Prediction | Neurology | 5,110 | — |
| CDC Diabetes BRFSS | Epidemiology | 253,680 | — |
| CKD UCI | Nephrology | 400 | — |
| Cirrhosis Mayo | Hepatology | 418 | — |
| Synthea FHIR R4 | Synthetic EHR | 1,180 | FHIR R4 |
| SMART Bulk FHIR | EHR Standards | 120 | FHIR |
| FHIR R4 Synthetic | Synthetic | configurable | FHIR R4 |
| OMOP-CDM Harmonized | Clinical Data Model | configurable | OMOP v5.4 |
| Diabetic Retinopathy | Ophthalmology | 35,126 | — |
| Brain Tumor MRI (Alt.) | Neuro-imaging | 3,264 | — |
| ISIC Skin Lesions | Dermatology | 2,357 | — |

</details>

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

| Code | Title | Venue | Year | Status | Repository |
|---|---|---|---|---|---|
| P-M | Federated Learning in Dynamic and Heterogeneous Environments: Advantages, Performances, and Privacy Problems | MDPI Applied Sciences · [DOI](https://doi.org/10.3390/app14188490) | 2024 | Published (21 cit.) | [DHFLPL2](https://github.com/FabioLiberti/DHFLPL2) · ([v1](https://github.com/FabioLiberti/DHFLPL)) |
| P-IS | FedHR5.0: Privacy-Preserving HR Management in Industry 5.0 | ISM 2025 — Univ. of Malta | 2025 | -- | [FedHR5.0](https://github.com/FabioLiberti/FedHR5.0) |
| P-CR | FA-FedAvg: Forensic-Aware Federated Averaging for Law Enforcement | CRISTAIN 2025 — CHItaly | 2025 | -- | [CRISTAIN2025](https://github.com/FabioLiberti/CRISTAIN2025) |
| P-C1 | Transforming Clinical Silos into Economic Assets: Business Models for European Digital Health Research Networks | CIDE 2025 — Ploiesti | 2025 | Presented | [CIDE](https://github.com/FabioLiberti/CIDE) |
| P-C2 | Explainable Federated Learning for Secure Telemedicine: Privacy-Preserving Deepfake Detection | CIDE 2025 — Ploiesti | 2025 | -- | [CIDE2](https://github.com/FabioLiberti/CIDE2) |
| P-IT | AI Distribuita e Governance Sanitaria: Analisi Multidimensionale delle Tensioni tra Norme, Etica e Innovazione | ITAIS 2025 | 2025 | Presented | [AI-DIGOSA](https://github.com/FabioLiberti/AI-DIGOSA) |
| FLICS | FL + EHDS Governance Framework: Differential Privacy and Secure Aggregation | FLICS 2026 — Valencia · IEEE | 2026 | Submitted | [FL-EHDS-FLICS2026](https://github.com/FabioLiberti/FL-EHDS-FLICS2026) |
| ICSIS | FL as Policy Data Infrastructure for Territorial Healthcare Planning | ICSIS 2026 — Valencia | 2026 | Submitted | [icsis2026](https://github.com/FabioLiberti/icsis2026) |
| ICID | Three-Layered Reference Architecture for FL within EHDS | ICID 2026 — Ulaanbaatar · Springer | 2026 | Submitted | [ICID2026](https://github.com/FabioLiberti/ICID2026) |
| IFKAD | FedHR5.0: Federated Learning for Knowledge Asset Dynamics in Industry 5.0 | IFKAD 2026 — Budapest | 2026 | Submitted | *Repo TBD* |

---

## Getting Started

This meta-repository uses **Git submodules** to link all component repositories.

```bash
# Clone with all submodules
git clone --recurse-submodules https://github.com/FabioLiberti/FENITH2.git

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

[![Website](https://img.shields.io/badge/Web-fabioliberti.com-blue)](https://www.fabioliberti.com/)
[![ORCID](https://img.shields.io/badge/ORCID-0000--0003--3019--5411-A6CE39)](https://orcid.org/0000-0003-3019-5411)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Fabio_Liberti-4285F4)](https://scholar.google.com/citations?user=ce_iUyEAAAAJ&hl=it)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-Fabio_Liberti-00CCBB)](https://www.researchgate.net/profile/Fabio-Liberti)

---

## Keywords

`federated-learning` · `european-health-data-space` · `ehds` · `privacy-preserving` · `differential-privacy` · `secure-aggregation` · `digital-healthcare-governance` · `heterogeneous-environments` · `dynamic-environments` ·`omop-OHDSI` · `hl7-fhir` · `data-mesh` · `industry-5-0`

---
