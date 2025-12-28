<!--
---
title: "radioastronomyio Organization"
description: "Computational astronomy research using DESI and large spectroscopic surveys"
author: "VintageDon"
date: "2025-12-28"
status: "Published"
---
-->

# RadioAstronomy.io

![repository-hero-banner](https://github.com/user-attachments/assets/41059111-f7be-46dd-87ca-739f7eb1fb15)

**Computational astronomy research investigating galaxy evolution, cosmic large-scale structure, and quasar physics using DESI and modern spectroscopic surveys**

---

## 🔭 Mission

This organization produces research outputs in astronomy and data science, building analysis-ready datasets from large public sources. The methodology was validated through the [Steam Dataset 2025](https://github.com/vintagedon/steam-dataset-2025) — a multi-modal gaming analytics ARD with strong engagement and downloads on both [Kaggle](https://www.kaggle.com/datasets/vrfrex/steam-dataset-2025-multi-modal-gaming-analytics) and [Zenodo](https://zenodo.org/records/13894078) — and is now being applied to DESI DR1 spectroscopic surveys.

Current work spans galaxy evolution in different cosmic environments, AGN feedback mechanisms, and ML-driven spectral analysis. The research runs on purpose-built infrastructure that enables reproducibility at scale, and the entire system functions as a skill multiplier across systems engineering, DevOps, security, and machine learning.

---

## 📦 Repositories

| Repository | Domain | Description | Status |
|------------|--------|-------------|--------|
| [proxmox-astronomy-lab](https://github.com/radioastronomyio/proxmox-astronomy-lab) | Infrastructure | Platform documentation, VM inventory, network architecture | Production |
| [desi-cosmic-void-galaxies](https://github.com/radioastronomyio/desi-cosmic-void-galaxies) | Research | ARD factory + environmental quenching in cosmic voids | Active |
| [desi-quasar-outflows](https://github.com/radioastronomyio/desi-quasar-outflows) | Research | AGN outflow spectral fitting and Cloudy modeling | Planned |
| [desi-qso-anomaly-detection](https://github.com/radioastronomyio/desi-qso-anomaly-detection) | Research | ML anomaly detection for quasar spectra | Planned |
| [rbh1-validation-reanalysis](https://github.com/radioastronomyio/rbh1-validation-reanalysis) | Research | Independent reanalysis of RBH-1 hypervelocity SMBH candidate | Active |
| [year-of-code-2026](https://github.com/radioastronomyio/year-of-code-2026) | Development | 2026 project sandbox: AI, ML, agentic coding, cloud infrastructure | Active |
| [.github](https://github.com/radioastronomyio/.github) | Meta | Organization profile and templates | — |

---

## 🔬 Active Repositories

### Proxmox Astronomy Lab

![proxmox-astronomy-lab-repo-banner](https://github.com/user-attachments/assets/625a45ef-cdad-4189-956e-691da996d6d0)

The infrastructure foundation for all research workloads. Documents the 7-node Proxmox cluster, VM inventory, network architecture, and automation patterns. This is the platform that enables reproducible, scalable research across all projects.

### DESI Cosmic Void Galaxies

![desi-cosmic-void-galaxies](https://github.com/user-attachments/assets/8c99b694-c2a9-479f-98c7-f3f9b01008a3)

Analyzing galaxy populations within cosmic voids using DESI Data Release 1 to investigate environmental quenching mechanisms. This project serves as the Analysis-Ready Dataset (ARD) factory for the organization, joining 9 Value-Added Catalogs into enriched data products that feed downstream research.

### DESI Quasar Outflows

![desi-quadar-outflows](https://github.com/user-attachments/assets/b46a07bc-56a2-42fc-8f33-1026b3ebf468)

Investigating AGN-driven outflows through semi-automated spectral fitting combined with Cloudy photoionization modeling. Developing automated pipelines to identify and characterize outflows in massive spectroscopic datasets.

### DESI Anomalous Quasar Detection

![desi-qad](https://github.com/user-attachments/assets/f059e3a1-db39-422b-a4a6-a23edbe6041c)

ML-based anomaly detection across millions of quasar spectra. Implementing 1D convolutional variational autoencoders on Ray clusters to identify statistically unusual objects that may represent new physics or rare phenomena.

### RBH-1 Validation Reanalysis

![rbh-1-validation-repo-banner](https://github.com/user-attachments/assets/483e2834-dc3d-44ef-8328-2182e6f5ef41)

Independent validation and reanalysis of the RBH-1 hypervelocity SMBH candidate (van Dokkum et al. 2025) using Bayesian inference and GPU-accelerated computing.

### Year of Code 2026

![year-of-code-2026-repo-banner](https://github.com/user-attachments/assets/6a203d42-0ac7-4043-b585-9cf748b17d04)

2026 project sandbox covering AI, ML, agentic coding, RAG systems, cloud infrastructure, and the occasional side project. A space for experimentation and skill development across the full technology stack.

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

Production research platform running on a 7-node Proxmox cluster built from small form factor enterprise workstations. The cluster provides dedicated database servers, GPU compute, and Kubernetes orchestration for containerized workloads.

### Cluster Specifications

| Resource | Value |
|----------|-------|
| Nodes | 7 |
| Total Cores | 144 |
| Total RAM | 704 GB |
| Total NVMe | 26 TB |
| Network Fabric | 10G LACP per node |
| GPU | RTX A4000 16GB |

### Node Inventory

| Node | CPU | Cores | RAM | Role |
|------|-----|-------|-----|------|
| node01 | i9-12900H | 20 | 96 GB | Compute (K8s) |
| node02 | i5-12600H | 16 | 96 GB | Light compute + 6TB storage |
| node03 | i9-12900H | 20 | 96 GB | Compute (K8s) |
| node04 | i9-12900H | 20 | 96 GB | Compute (K8s) |
| node05 | i5-12600H | 16 | 96 GB | Light compute + 6TB storage |
| node06 | i9-13900H | 20 | 96 GB | Heavy compute (databases) |
| node07 | AMD 5950X | 32 | 128 GB | GPU compute |

### VM Inventory

Research workloads run on dedicated VMs with role-specific resource allocation.

| VM | IP | vCPU | RAM | Purpose |
|----|-----|------|-----|---------|
| radio-k8s01 | 10.25.20.4 | 12 | 48G | Kubernetes primary node |
| radio-k8s02 | — | 12 | 48G | Kubernetes worker |
| radio-k8s03 | — | 12 | 48G | Kubernetes worker |
| radio-gpu01 | 10.25.20.10 | 12 | 48G | GPU worker (A4000) + K8s |
| radio-pgsql01 | 10.25.20.8 | 8 | 32G | Research PostgreSQL (pgvector, PostGIS) |
| radio-pgsql02 | 10.25.20.16 | 4 | 16G | Application PostgreSQL |
| radio-neo4j01 | 10.25.20.21 | 6 | 24G | Graph database |
| radio-fs02 | 10.25.20.15 | 4 | 6G | SMB file server (spectral data) |
| radio-agents01 | 10.25.20.20 | 8 | 32G | AI agents, monitoring stack |

### Architecture Diagram

![architecture-diagram](https://github.com/user-attachments/assets/3c73a798-8e7a-49b8-a05a-836e677cc094)

### Platform Capabilities

- **Hybrid Kubernetes + VM Architecture**: RKE2 orchestration with strategic static VMs for databases and persistent services
- **Enterprise Security Baseline**: CIS Controls implementation with research workflow accommodations
- **Secure Remote Access**: Entra ID hybrid identity with Cloudflare ZTNA
- **Open Source Toolchain**: GitOps automation, container orchestration, scientific computing workflows

---

## 🧪 Technology Stack

### Languages & Frameworks

[![Python](https://img.shields.io/badge/Python-3.12-3776ab?logo=python)](https://www.python.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?logo=typescript)](https://www.typescriptlang.org/)
[![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash)](https://www.gnu.org/software/bash/)

### Databases

[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql)](https://www.postgresql.org/)
[![Neo4j](https://img.shields.io/badge/Neo4j-008cc1?logo=neo4j)](https://neo4j.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb)](https://www.mongodb.com/)
[![DragonflyDB](https://img.shields.io/badge/DragonflyDB-fd4d4d?logo=redis)](https://www.dragonflydb.io/)

### AI/ML

[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch)](https://pytorch.org/)
[![LangChain](https://img.shields.io/badge/LangChain-yellow?logo=langchain)](https://www.langchain.com/)
[![Ollama](https://img.shields.io/badge/Ollama-222?logo=ollama)](https://ollama.ai/)
[![MLflow](https://img.shields.io/badge/MLflow-020230?logo=mlflow)](https://mlflow.org/)

### Infrastructure

[![Proxmox](https://img.shields.io/badge/Proxmox-E57000?logo=proxmox)](https://www.proxmox.com/)
[![RKE2](https://img.shields.io/badge/RKE2-326ce5?logo=kubernetes)](https://docs.rke2.io/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker)](https://www.docker.com/)
[![Ansible](https://img.shields.io/badge/Ansible-000000?logo=ansible)](https://www.ansible.com/)

### Observability

[![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus)](https://prometheus.io/)
[![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana)](https://grafana.com/)
[![Loki](https://img.shields.io/badge/Loki-4a8bdb?logo=grafana)](https://grafana.com/oss/loki/)

---

## 🤝 OSS Program Support

This organization benefits from open source programs that provide tooling to qualifying public repositories.

### Active Programs

| Program | Provides | Use Case |
|---------|----------|----------|
| [CodeRabbit](https://coderabbit.ai) | AI code review (Pro tier) | PR review, CLI integration with agentic coding tools |
| [Atlassian](https://www.atlassian.com/software/views/open-source-license-request) | Jira, Confluence (Standard) | Project tracking, documentation |

### Available for Future Use

| Program | Provides | Planned Use |
|---------|----------|-------------|
| [Snyk](https://snyk.io/plans/) | Security scanning | Dependency vulnerability detection |
| [SonarCloud](https://www.sonarsource.com/open-source-editions/) | Code quality | Static analysis |
| [Sentry](https://sentry.io/for/open-source/) | Error tracking | Runtime monitoring |
| [Datadog](https://www.datadoghq.com/partner/open-source/) | Observability | Metrics, logs, APM |

---

## 🌟 Open Science Philosophy

We practice open science and open methodology — our version of "showing your work":

- **Research methodologies** are fully documented and repeatable
- **Infrastructure configurations** are version-controlled and automated
- **Scripts and pipelines** are published so others can learn, adapt, or improve them
- **Learning processes** are captured and shared for community benefit

Our hope is that these materials help someone facing similar challenges, or inspire collaboration that helps us. All projects operate under open source licenses (primarily MIT) to ensure maximum reproducibility.

---

## 📚 Documentation

- **Documentation Hub**: [docs.radioastronomy.io](https://docs.radioastronomy.io)
- **GitHub Discussions**: Technical discussions and collaboration
- **Issue Tracking**: Project-specific development milestones

---

## 📄 License

Projects in this organization are licensed under MIT unless otherwise specified.

---

*Computational astronomy research through open data, reproducible workflows, and enterprise infrastructure*
