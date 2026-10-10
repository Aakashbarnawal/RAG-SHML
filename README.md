<div align="center">

# RAG-SHML
### Self-Healing MLOps Platform with LLM-Based Incident Responder

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Credit%20Card%20Fraud%20Detection-blue?style=for-the-badge" alt="Domain" />
  <img src="https://img.shields.io/badge/Architecture-MLOps%20%2B%20RAG%20%2B%20LLM-purple?style=for-the-badge" alt="Architecture" />
  <img src="https://img.shields.io/badge/Status-Research%20%26%20Development-green?style=for-the-badge" alt="Status" />
</p>

<p align="center">
  <b>An automated, evidence-grounded machine learning operations platform designed to detect distribution shifts, investigate operational anomalies, and facilitate controlled remediation for critical fraud detection workloads.</b>
</p>

---

</div>

## 📌 Project Overview

Production machine learning systems deployed in adversarial, non-stationary environments—such as financial fraud detection—face continuous performance degradation due to evolving fraud patterns, concept drift, and data pipeline anomalies. Traditional MLOps workflows rely heavily on manual intervention to triage alerts, diagnose root causes, and execute model updates.

**RAG-SHML** investigates a closed-loop, self-healing MLOps framework that couples automated statistical drift monitoring with retrieval-augmented generation (RAG) and large language model (LLM) diagnostics. When anomalies or distribution shifts occur, the system records operational incidents, retrieves relevant domain procedures, synthesizes evidence-backed diagnostic reports, and supports governed model remediation.

---

## 🎯 High-Level Objectives

- **Continuous Distribution Monitoring**: Track feature-level and dataset-level distribution shifts between reference baselines and streaming production data.
- **Structured Incident Management**: Capture, categorize, and persist operational incidents when statistical anomalies or performance deviations exceed defined operating bounds.
- **Evidence-Grounded Diagnostics**: Utilize semantic retrieval across curated domain knowledge to provide context-aware, verifiable investigation summaries without relying on ungrounded model generations.
- **Controlled Self-Healing Remediation**: Support automated challenger model training, empirical quality gate evaluation, and safety-checked model lifecycle governance.
- **System Observability & Modularity**: Decouple monitoring, diagnosis, and operational serving into modular, maintainable services.

---

## 🚀 Key Capability Areas

### 1. Continuous Drift Monitoring & Anomaly Detection
- Multi-metric statistical distribution tracking against verified reference baselines.
- Feature-level and dataset-level shift identification across high-dimensional feature spaces.
- Real-time metric export and alert triggering for downstream operations.

### 2. Incident Persistence & Context Capture
- Systematic persistence of drift events, telemetry, and operational evidence.
- Structured schema validation to ensure reproducibility and traceability of production alerts.
- Filterable incident querying and lifecycle status tracking.

### 3. Retrieval-Augmented Knowledge & Investigation
- Persistent domain knowledge repository containing validated operational runbooks, schema specifications, and troubleshooting procedures.
- Dense vector representations and similarity-based retrieval to provide relevant technical context for incident triage.
- Strict verification boundaries separating established system facts from operational hypotheses.

### 4. Governed Model Lifecycle & Remediation
- Automated trigger mechanisms to train candidate challenger models on updated data distributions.
- Empirical quality-gate evaluation comparing champion and challenger models on holdout validation data.
- Deterministic safety verification preventing unverified or low-confidence model promotions.

---

## 🛠️ Technology Stack

| Component | Technologies |
| :--- | :--- |
| **Core Language** | Python 3.10+ |
| **Model Serving & APIs** | FastAPI, Uvicorn, Pydantic |
| **Machine Learning** | XGBoost, Scikit-learn |
| **Drift Monitoring** | Evidently AI, SciPy, NumPy, Pandas |
| **Experiment Tracking & Registry** | MLflow |
| **Vector Indexing & Embeddings** | FAISS, Sentence Transformers (`all-MiniLM-L6-v2`) |
| **LLM Diagnosis & Reasoning** | Google Gemini API |
| **Metrics & Infrastructure** | Prometheus Pushgateway, SQLite, Docker |

---

## 📊 Project Context & Status

- **Type**: Final Year Academic Project (FYP) / MLOps Research
- **Domain Focus**: Credit Card Fraud Detection
- **Current Milestone**: Active research and development, with core monitoring, incident persistence, structured knowledge base, and model validation modules implemented.

---

## ⚠️ Academic Showcase & Disclaimer

> **Note on Implementation Blueprint**:
> This repository serves as a public academic showcase and high-level project summary for **RAG-SHML**. Proprietary dataset samples, model weights, internal runbooks, internal prompts, experiment configurations, and production secrets are omitted to protect research originality and maintain deployment security.

---

<div align="center">
  <sub>Developed as part of Final Year Project (FYP) Research in Applied Machine Learning & MLOps Automation.</sub>
</div>
