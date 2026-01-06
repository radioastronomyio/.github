<!--
---
title: "radioastronomyio Organization"
description: "Computational astronomy research using DESI and large spectroscopic surveys"
author: "VintageDon"
date: "2025-01-06"
status: "Published"
---
-->

# RadioAstronomy.io

<!-- Sponsors + License -->
[![Greptile](https://img.shields.io/badge/Greptile-Code_Review-4F46E5?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgZmlsbD0id2hpdGUiLz48L3N2Zz4=)](https://greptile.com)
[![Atlassian](https://img.shields.io/badge/Atlassian-Jira_|_Confluence-0052CC?logo=atlassian)](https://www.atlassian.com/software/views/open-source-license-request)
[![Snyk](https://img.shields.io/badge/Snyk-Security-4C4A73?logo=snyk)](https://snyk.io/plans/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

<!-- Tech Stack -->
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?logo=neo4j&logoColor=white)](https://neo4j.com/)
[![DragonflyDB](https://img.shields.io/badge/DragonflyDB-FF6B6B?logo=redis&logoColor=white)](https://www.dragonflydb.io/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Ollama](https://img.shields.io/badge/Ollama-000000?logo=ollama&logoColor=white)](https://ollama.ai/)
[![Proxmox](https://img.shields.io/badge/Proxmox-E57000?logo=proxmox&logoColor=white)](https://www.proxmox.com/)
[![RKE2](https://img.shields.io/badge/RKE2-326CE5?logo=kubernetes&logoColor=white)](https://docs.rke2.io/)
[![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)](https://www.ansible.com/)

![radioastronomyio-org-repo-banner](https://github.com/user-attachments/assets/4ed8b6e1-740f-46b9-a218-2b229bab8632)

**Computational astronomy research investigating galaxy evolution, cosmic large-scale structure, and quasar physics using DESI and modern spectroscopic surveys**

---

## 🔭 Mission

This organization produces research outputs in astronomy and data science, building analysis-ready datasets from large public sources. The methodology was validated through the [Steam Dataset 2025](https://github.com/vintagedon/steam-dataset-2025) — a multi-modal gaming analytics ARD with strong engagement on both [Kaggle](https://www.kaggle.com/datasets/vrfrex/steam-dataset-2025-multi-modal-gaming-analytics) and [Zenodo](https://zenodo.org/records/13894078) — and is now being applied to DESI DR1 spectroscopic surveys.

Current work spans galaxy evolution in different cosmic environments, AGN feedback mechanisms, and ML-driven spectral analysis. The research runs on purpose-built infrastructure that enables reproducibility at scale.

---

## 🤝 Open Source Sponsors

This organization benefits from open source programs that provide tooling to qualifying public repositories. These sponsorships aren't just logos — they enable workflows that would otherwise be impractical for an independent research operation.

| Sponsor | Provides | Impact |
|---------|----------|--------|
| [Greptile](https://greptile.com) | AI code review | PR review on every commit, enforcing git discipline across all repos |
| [Atlassian](https://www.atlassian.com/software/views/open-source-license-request) | Jira, Confluence (Standard) | Project tracking, milestone management, documentation |
| [Snyk](https://snyk.io/plans/) | Security scanning | Dependency vulnerability detection across the organization |

---

### Proxmox Astronomy Lab

![proxmox-astronomy-lab-repo-banner](https://github.com/user-attachments/assets/625a45ef-cdad-4189-956e-691da996d6d0)

The infrastructure foundation for all research workloads. A 7-Node Proxmox cluster with 144 cores and 700GB+ of RAM total, including a dedicated GPU node with an nvidia A4000 16GB. Documents the 7-node Proxmox cluster, VM inventory, network architecture, and automation patterns. This is the platform that enables reproducible, scalable research across all projects.

[View Repository →](https://github.com/radioastronomyio/proxmox-astronomy-lab)

---

## 🔬 Research Projects

### DESI Cosmic Void Galaxies

![desi-cosmic-void-galaxies](https://github.com/user-attachments/assets/8c99b694-c2a9-479f-98c7-f3f9b01008a3)

Analyzing galaxy populations within cosmic voids using DESI Data Release 1 to investigate environmental quenching mechanisms. This project serves as the Analysis-Ready Dataset (ARD) factory for the organization, joining 9 Value-Added Catalogs into enriched data products that feed downstream research.

[View Repository →](https://github.com/radioastronomyio/desi-cosmic-void-galaxies)

---

### DESI Quasar Outflows

![desi-quasar-outflows](https://github.com/user-attachments/assets/b46a07bc-56a2-42fc-8f33-1026b3ebf468)

Investigating AGN-driven outflows through semi-automated spectral fitting combined with Cloudy photoionization modeling. Developing automated pipelines to identify and characterize outflows in massive spectroscopic datasets.

[View Repository →](https://github.com/radioastronomyio/desi-quasar-outflows)

---

### DESI Anomalous Quasar Detection

![desi-qso-anomaly-detection](https://github.com/user-attachments/assets/f059e3a1-db39-422b-a4a6-a23edbe6041c)

ML-based anomaly detection across millions of quasar spectra. Implementing 1D convolutional variational autoencoders on Ray clusters to identify statistically unusual objects that may represent new physics or rare phenomena.

[View Repository →](https://github.com/radioastronomyio/desi-qso-anomaly-detection)

---

### RBH-1 Validation Reanalysis

![rbh-1-validation-repo-banner](https://github.com/user-attachments/assets/483e2834-dc3d-44ef-8328-2182e6f5ef41)

Independent validation and reanalysis of the RBH-1 hypervelocity SMBH candidate (van Dokkum et al. 2025) using Bayesian inference and GPU-accelerated computing.

[View Repository →](https://github.com/radioastronomyio/rbh1-validation-reanalysis)

---

## 📐 Methodology & Data

### Meshworks

![meshworks-repo-banner](https://github.com/user-attachments/assets/4766d258-dd35-4a3d-8694-a13435dba389)

Control plane that meshes VS Code Server, MetaMCP, and AI agents (Claude/Gemini) with audit-first ops. Centralizes agent orchestration and provides unified tooling across the research environment.

[View Repository →](https://github.com/radioastronomyio/meshworks) *(Coming soon)*

---

### Analysis-Ready Datasets

![analysis-ready-dataset-repo-banner](https://github.com/user-attachments/assets/90e4b391-95bf-42a0-b8f1-725bca189dc9)

Specification and methodology for building Analysis-Ready Datasets (ARDs) — pre-computed, enriched data products that eliminate repetitive preprocessing and enable immediate analysis. Domain-agnostic framework with reference implementations.

[View Repository →](https://github.com/radioastronomyio/analysis-ready-datasets)

---

### Astronomy RAG Corpus

![astronomy-rag-corpus-repo-banner](https://github.com/user-attachments/assets/dcf35968-da51-40fb-8e37-464a119b7d85)

A Federated Knowledge Core for astronomical research — decoupling semantic meaning from structural relationships to enable expert-level RAG and autonomous Deep Research agents.

[View Repository →](https://github.com/radioastronomyio/astronomy-rag-corpus)

---

## 🛠️ Tools & Cookbooks

### Claude Skills Cookbook

![claude-skills-cookbook-repo-banner](https://github.com/user-attachments/assets/a3f55096-00bd-4b0b-a1a1-e6336955e26a)

Tested recipes for Claude skills and hooks — methodology documentation, failure modes, and honest assessments. Not another awesome-list.

[View Repository →](https://github.com/radioastronomyio/claude-skills-cookbook)

---

### Docker Compose Cookbook

![docker-compose-cookbook-repo-banner](https://github.com/user-attachments/assets/fed5f96d-a91d-4ba1-b82a-8a4c5ec0f7c8)

A collection of Docker compose scripts centered around use in a home lab for learning IT technologies.

[View Repository →](https://github.com/radioastronomyio/docker-compose-cookbook)

---

### AI Models Wiki

![aimodels-repo-banner](https://github.com/user-attachments/assets/c8b71720-286c-411e-91e9-a7490f0f1fc0)

AI Model Wiki website presenting structured model card data for 160+ AI models, running on Astro, Tailwind and Typescript on Azure Static Web Apps.

[View Repository →](https://github.com/radioastronomyio/aimodels-wiki)

---

## 📦 Templates & Sandbox

### Project Template Repository

![project-template-repo-banner](https://github.com/user-attachments/assets/401ac3db-a713-4be7-98d6-37c7b1bb3520)

Repository standardizing the structure and layout for all repositories in the RadioAstronomy.io Github organization.

[View Repository →](https://github.com/radioastronomyio/project-template-repository)

---

### Year of Code 2026

![year-of-code-2026-repo-banner](https://github.com/user-attachments/assets/6a203d42-0ac7-4043-b585-9cf748b17d04)

2026 project sandbox covering AI, ML, agentic coding, RAG systems, cloud infrastructure, and the occasional side project. A space for experimentation and skill development across the full technology stack.

[View Repository →](https://github.com/radioastronomyio/year-of-code-2026)

---

### Firewall Defense RL

![firewall-defense-repo-banner](https://github.com/user-attachments/assets/1f3cf340-ab59-4ae8-8dc5-329574bf7159)

Grid Defense RL is a custom Gymnasium environment designed for training and visualizing reinforcement learning agents. A PPO agent via Stable-Baselines3 learns to place defensive walls on a 13×9 grid to block enemies moving toward a core.

[View Repository →](https://github.com/radioastronomyio/firewall-defense-agentic-gaming)

---

## 📊 Data Assets

Our research consumes DESI Data Release 1 Value-Added Catalogs, materialized through PostgreSQL and distributed as Parquet files.

### DESI DR1 Value-Added Catalogs

| VAC | Purpose | Scale |
|-----|---------|-------|
| [FastSpecFit](https://data.desi.lbl.gov/doc/releases/dr1/vac/fastspecfit/) | Stellar continuum modeling, emission line fluxes | 6.4M galaxies |
| [PROVABGS](https://data.desi.lbl.gov/doc/releases/edr/vac/provabgs/) | Bayesian SED fitting, stellar mass, SFH | BGS sample |
| [DESIVAST](https://data.desi.lbl.gov/doc/releases/dr1/vac/desivast/) | Void classifications (4 algorithms) | ~10.7K voids |
| [Gfinder](https://data.desi.lbl.gov/doc/releases/dr1/vac/gfinder/) | Group catalog, halo mass estimates | Group members |
| [AGN/QSO](https://data.desi.lbl.gov/doc/releases/dr1/vac/agnqso/) | Systemic redshifts, BAL flags, spectral classification | 1.4M QSOs |
| [CIV Absorber](https://data.desi.lbl.gov/doc/releases/dr1/vac/civ-absorber/) | Intervening CIV absorption systems | Absorber catalog |
| [MgII Absorber](https://data.desi.lbl.gov/doc/releases/dr1/vac/mgii-absorber/) | Intervening MgII absorption systems | Absorber catalog |
| [QMassIron](https://data.desi.lbl.gov/doc/releases/dr1/vac/qmassiron/) | Black hole masses, bolometric luminosity | QSO subset |
| [Stellar Mass/EmLine](https://data.desi.lbl.gov/doc/releases/dr1/vac/stellar-mass-emline/) | CIGALE stellar masses, emission line properties | Full sample |

### Data Pipeline

PostgreSQL serves as the materialization engine where VAC joins and derived computations occur. Final ARD products are exported to Parquet for distribution and analysis. The pipeline currently manages ~32GB of catalog data in PostgreSQL and ~108GB of spectral tiles in Parquet format.

---

## 🏗️ Platform Architecture

Production research platform running on a 7-node Proxmox cluster built from small form factor enterprise workstations.

| Resource | Value |
|----------|-------|
| Nodes | 7 |
| Total Cores | 144 |
| Total RAM | 704 GB |
| Total NVMe | 26 TB |
| Network Fabric | 10G LACP per node |
| GPU | RTX A4000 16GB |

![architecture-diagram](https://github.com/user-attachments/assets/3c73a798-8e7a-49b8-a05a-836e677cc094)

---

## 🌟 Open Science Philosophy

We practice open science and open methodology — our version of "showing your work":

![repository-hero-banner](https://github.com/user-attachments/assets/41059111-f7be-46dd-87ca-739f7eb1fb15)

- **Research methodologies** are fully documented and repeatable
- **Infrastructure configurations** are version-controlled and automated
- **Scripts and pipelines** are published so others can learn, adapt, or improve them
- **Learning processes** are captured and shared for community benefit

Our hope is that these materials help someone facing similar challenges, or inspire collaboration that helps us. All projects operate under open source licenses (primarily MIT) to ensure maximum reproducibility.

---

## 📄 License

Projects in this organization are licensed under MIT unless otherwise specified.

---

*Computational astronomy research through open data, reproducible workflows, and enterprise infrastructure*
