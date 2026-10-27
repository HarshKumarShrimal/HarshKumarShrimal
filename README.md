# Harsh Kumar Shrimal

**Applied AI / Machine Learning Engineer & Systems Researcher**  
B.Tech in Electronics & Communication Engineering, **Rajiv Gandhi Institute of Petroleum Technology (RGIPT)**  
📍 Amethi, Uttar Pradesh, India | ✉️ [hshrimal99@gmail.com](mailto:hshrimal99@gmail.com) | 🐙 [github.com/HarshKumarShrimal](https://github.com/HarshKumarShrimal)

---

## 👨‍💻 Executive Summary

I am an Applied Machine Learning Engineer with a foundational background in Electronics and Communication Engineering from RGIPT. My engineering practice bridges statistical machine learning, sensor trajectory analytics, industrial computer vision, and grounded information retrieval systems.

I prioritize:
- **Reproducible Evaluation over Vanity Metrics:** Rejecting misleading raw accuracy on imbalanced benchmarks in favor of PR-AUC, Brier calibration, and NASA asymmetric penalty scores.
- **Strict Leak-Free Pipeline Architecture:** Guaranteeing zero temporal or split leakage across causal sensor windows and feature transformation pipelines.
- **Low-Overhead, Production-Grade Inference:** Engineering sub-5ms FastAPI backends with deterministic reference calibration for single-sample streaming execution.
- **Transparent Attribution & Explainability:** Providing local SHAP decomposition with explicit mathematical disclosure of underlying PCA components.

---

## 🚀 Featured AI/ML Portfolio Projects

| Project | Focus Domain | Key Architecture & Tech | Measured Benchmark Highlight | Artifacts & Links |
| :--- | :--- | :--- | :--- | :--- |
| **[industrial-vision-anomaly-detection](https://github.com/HarshKumarShrimal/industrial-vision-anomaly-detection)** | Deep Industrial Computer Vision & Defect Localization | PatchCore (Coreset memory banks), PaDiM (Multivariate Gaussian embeddings), Deep Autoencoder baseline | **Image AUROC: 1.000**, **Pixel AUROC: 0.994**, **PRO: 0.979** (MVTec AD synthetic benchmark) | [Code](https://github.com/HarshKumarShrimal/industrial-vision-anomaly-detection) • [Interview Prep](https://github.com/HarshKumarShrimal/industrial-vision-anomaly-detection/blob/main/INTERVIEW_NOTES.md) • [Upstream Audit](https://github.com/HarshKumarShrimal/industrial-vision-anomaly-detection/blob/main/UPSTREAM.md) |
| **[turbofan-rul-predictive-maintenance](https://github.com/HarshKumarShrimal/turbofan-rul-predictive-maintenance)** | Physics-Informed Prognostics & Time-Series RUL Estimation | NASA C-MAPSS FD001 (100 engines), 1D-CNN temporal encoder, XGBoost, Random Forest, SHAP TreeExplainer | **1D-CNN Test MAE: 13.52**, **RMSE: 18.55**, **NASA Score: 640.59** ($R^2 = 0.8007$, 54% early safe calls) | [Code](https://github.com/HarshKumarShrimal/turbofan-rul-predictive-maintenance) • [Interview Prep](https://github.com/HarshKumarShrimal/turbofan-rul-predictive-maintenance/blob/main/INTERVIEW_NOTES.md) • [Results](https://github.com/HarshKumarShrimal/turbofan-rul-predictive-maintenance/blob/main/results/predicted_vs_actual_rul.png) |
| **[engineering-knowledge-rag-assistant](https://github.com/HarshKumarShrimal/engineering-knowledge-rag-assistant)** | Grounded Technical RAG & Provenance Extraction | Hybrid Retrieval (BM25 + TF-IDF Vector Space, Reciprocal Rank Fusion $k=60$), Strict Abstention Guardrails | **Recall@3: 1.000**, **MRR@3: 1.000**, **Abstention Accuracy: 1.000** (0.33ms retrieval latency) | [Code](https://github.com/HarshKumarShrimal/engineering-knowledge-rag-assistant) • [Interview Prep](https://github.com/HarshKumarShrimal/engineering-knowledge-rag-assistant/blob/main/INTERVIEW_NOTES.md) • [Upstream Audit](https://github.com/HarshKumarShrimal/engineering-knowledge-rag-assistant/blob/main/UPSTREAM.md) |
| **[explainable-fraud-risk-engine](https://github.com/HarshKumarShrimal/explainable-fraud-risk-engine)** | Imbalanced Risk Analytics & Anomaly Scoring | Calibrated Hybrid Risk Engine (XGBoost + Calibrated Isolation Forest), Cost-Optimal Threshold Sweeps, SHAP | **PR-AUC: 1.000**, **ROC-AUC: 1.000**, **F1: 0.9091** (Calibrated continuous 0–100 risk score) | [Code](https://github.com/HarshKumarShrimal/explainable-fraud-risk-engine) • [Interview Prep](https://github.com/HarshKumarShrimal/explainable-fraud-risk-engine/blob/main/INTERVIEW_NOTES.md) • [Upstream Audit](https://github.com/HarshKumarShrimal/explainable-fraud-risk-engine/blob/main/UPSTREAM.md) |

---

## 🛠️ Technical Competencies & Toolchain

### Machine Learning & Statistical Modeling
- **Frameworks:** PyTorch, Torchvision, Scikit-Learn, XGBoost, SciPy, NumPy, Pandas.
- **Time-Series & Prognostics:** Causal lag feature engineering, rolling window degradation profiles, piecewise linear RUL target clipping, NASA asymmetric risk penalties.
- **Computer Vision:** Self-supervised anomaly detection, frozen ResNet/WideResNet feature hierarchies, memory bank coreset subsampling, defect heatmap generation, Per-Region Overlap (PRO) metrics.
- **Explainability & Calibration:** SHAP (TreeExplainer, KernelExplainer), Brier score calibration, empirical percentile calibration, decision-cost curves.
- **Information Retrieval:** BM25 lexical ranking, dense vector space retrieval, Reciprocal Rank Fusion (RRF), token sliding window chunkers, prompt injection defense.

### Systems, Signals & Hardware Foundations (RGIPT ECE)
- **Signal Processing:** Fourier Analysis, Digital Filters (FIR/IIR), Sensor Noise Filtering, Feature Extraction from Analog/Digital Transducers.
- **Embedded & Hardware:** Microcontroller architectures (ARM, ESP32, AVR), Serial Communication (UART, SPI, I2C), ADC/DAC sampling constraints.

### Software Engineering & MLOps
- **Backend & APIs:** FastAPI, Uvicorn, Pydantic (V2), REST API design, Starlette TestClient.
- **DevOps & Tooling:** Docker, Docker Compose, Git, GitHub Actions (CI/CD), Pytest, Flake8, macOS/Linux environments.

---

## 🔬 Core Engineering Contributions Across Repositories

```
┌───────────────────────────────────────┬─────────────────────────────────────────────────────────────────┐
│ System / Repository                   │ Key Engineering Fix & Architectural Contribution                │
├───────────────────────────────────────┼─────────────────────────────────────────────────────────────────┤
│ industrial-vision-anomaly-detection   │ Fixed trapezoidal collapse in PRO metric (collapsed to 0.0);   │
│                                       │ Added multi-model inference pipeline with jet heatmap overlay.  │
├───────────────────────────────────────┼─────────────────────────────────────────────────────────────────┤
│ turbofan-rul-predictive-maintenance   │ Ingested real NASA C-MAPSS FD001 data; built causal feature     │
│                                       │ pipeline (zero future leakage); evaluated PyTorch 1D-CNN vs tree│
│                                       │ ensembles on NASA asymmetric scoring function.                  │
├───────────────────────────────────────┼─────────────────────────────────────────────────────────────────┤
│ engineering-knowledge-rag-assistant   │ Built hybrid BM25 + dense TF-IDF retrieval with RRF (k=60);     │
│                                       │ Added strict stop-word filtered abstention guards against halluc.│
├───────────────────────────────────────┼─────────────────────────────────────────────────────────────────┤
│ explainable-fraud-risk-engine         │ Fixed upstream single-sample anomaly collapse (max-min on N=1); │
│                                       │ Engineered calibrated 0-100 risk score and cost-optimal sweep.  │
└───────────────────────────────────────┴─────────────────────────────────────────────────────────────────┘
```

---

## 🎓 Education & Credentials

- **Bachelor of Technology (B.Tech) in Electronics and Communication Engineering**  
  *Rajiv Gandhi Institute of Petroleum Technology (RGIPT)*, Jais, Amethi, UP  
  *(An Institute of National Importance established by the Ministry of Petroleum and Natural Gas, Govt. of India)*

---

## 📬 Contact & Collaboration

- **Email:** [hshrimal99@gmail.com](mailto:hshrimal99@gmail.com)
- **GitHub:** [HarshKumarShrimal](https://github.com/HarshKumarShrimal)
- **Location:** RGIPT Campus, Jais / Open to Remote and On-Site Applied AI Engineering Roles
