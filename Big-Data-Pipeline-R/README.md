# 📊 Advanced Data Mining Portfolio: Feature Engineering to Predictive Modeling

> **Executive Summary:** > This comprehensive portfolio integrates **Big Data Spatiotemporal Analytics** and **Financial Risk Predictive Modeling**. It demonstrates the end-to-end data science lifecycle—from orchestrating 21.8 million records of raw GPS data to benchmarking complex machine learning architectures for credit risk assessment.

---

## 🚖 Project 1: Rome Taxi Spatiotemporal Data Orchestration
**Focus:** Large-scale telemetry data processing, noise filtering, and driver activity modeling.

### 🛠️ Technical Implementations
* **Big Data Orchestration:** Processed a massive dataset of **21,817,851 GPS points** collected from 320 taxi drivers in Rome, Italy.
* **Advanced Data Cleaning:** Engineered a multi-tier filtering system to remove **Outliers** (based on Roman city boundaries 41.65°N-42.05°N) and **Noise** (GPS speed jumps > 200 km/h).
* **Activity Performance Modeling:** Developed an algorithm to quantify driver activity, identifying a global average activity duration of **631.64 hours** per month.
* **Trajectory Analytics:** Applied the **Haversine formula** to calculate precise driving distances; notably, Taxi ID 261 covered **2,573.96 km** during the 30-day period.

---

## 🏦 Project 2: Financial Credit Risk Intelligence & Benchmarking
**Focus:** Exploratory Data Analysis (EDA), Supervised learning, and algorithm performance optimization.

### 🚀 Model Benchmarking & Performance
| Model Type | Optimization Strategy | Key Results |
| :--- | :--- | :--- |
| **SVM (Tuned)** | RBF Kernel + Cost/Gamma Tuning | **61.88% Accuracy** (Top Performer). |
| **MLP Model** | 402040 Confidence Strategy | **62.63% Accuracy** with 79.96% Coverage. |
| **Random Forest** | Ensembled 700 trees, mtry=10 | **99.15% Coverage** & stable robustness. |
| **Decision Tree** | Baseline Path Analysis | **60.86% Accuracy** on test set. |

### 🔍 Diagnostic Insights
* **Feature Significance:** Identified the top critical risk predictors—**Functionary Status, FI30 Credit Score, Repayment History, and Past Credit Refusals**—through Pearson Correlation and significance testing.
* **Unsupervised Diagnostics:** Utilized **Self-Organizing Maps (SOM)** and **PCA Visualization** to identify class overlap, proving that 100% accuracy is unattainable due to fuzzy class boundaries.

---

## 🛠️ Tech Stack & Methodology
* **Language:** R (v4.4.3).
* **Key Libraries:** `randomForest`, `e1071` (SVM & NB), `rpart`, `pROC`, `caret`, `som`, `ggplot2`.
* **Methodologies:** Haversine Distance, Entropy/Information Gain Calculation, ROC/AUC Evaluation, and 70/30 Train-Test Validation.

---
*Developed by **Yanhui Ma** *
