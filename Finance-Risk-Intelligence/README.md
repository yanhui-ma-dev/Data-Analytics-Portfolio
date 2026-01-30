# 🏦 Credit Risk Intelligence: Predictive Modeling & Benchmarking

> **Project Overview:** > This project focuses on building a robust credit scoring system using advanced machine learning techniques. Leveraging a dataset of **1,962 assessed customers** and **46 multi-dimensional attributes**, the goal is to accurately predict creditworthiness (Rating 1, 2, or 3) to minimize financial default risks.

---

## 🚀 Key Project Highlights

* **Multi-Algorithm Benchmarking:** Implemented and compared five different models: **Decision Tree, Random Forest, SVM (Tuned), Naive Bayes, and Logistic Regression**.
* **Performance Leadership:** The **Tuned SVM** model emerged as the top performer with a test accuracy of **61.88%**.
* **Deep Diagnostic Analysis:** Utilized **Self-Organizing Maps (SOM)** and **PCA Visualization** to identify significant class overlaps and non-linear feature interactions.
* **Business-Centric Evaluation:** Evaluated models not just on accuracy, but on **Precision, Recall, and Coverage** (MLP vs. Random Forest) to ensure real-world deployability.

---

## 📊 Model Performance Summary

| Model | Test Accuracy | Top Class Recognized |
| :--- | :--- | :--- |
| **SVM (Tuned)** | **61.88%** | Class 2 (Stable) |
| **Random Forest** | **61.37%** | Class 2 (Recall: 79.4%) |
| **Decision Tree** | **60.86%** | Class 2 (Recall: 78.2%) |
| **MLP (Optimized)** | **62.63%** | High Accuracy, but 20% Rejection |
| **Naive Bayes** | **53.82%** | Baseline Classifier |

---

## 🔍 Feature Engineering & Insights

Based on **Pearson Correlation** and **Logistic Regression coefficients**, the top 5 most significant predictors for credit risk were identified:
1.  **Functionary Status** (Occupation)
2.  **FI3O Credit Score**
3.  **Repayment History** (Recently overdrawn accounts)
4.  **Past Credit Refusals**
5.  **Years of Employment**

---

## 🛠️ Tech Stack & Methodology

* **Language:** R (v4.4.3)
* **Libraries:** `rpart`, `randomForest`, `e1071` (SVM), `pROC`, `caret`, `som`
* **Techniques:** * **Data Split:** 70/30 Train-Test split for robust validation.
    * **Hyperparameter Tuning:** Automated grid search for Random Forest (`ntree=900`, `mtry=18`) and SVM (`cost=1`, `gamma=0.01`).
    * **Evaluation:** ROC/AUC curves, Confusion Matrices, and Entropy/Information Gain calculations.

---

## 📁 Repository Structure
* `Finance-Risk-Intelligence/`
    * `*.R`: Source scripts for model training and optimization.
    * `Credit Risk Intelligence Predictive Modeling...pdf`: Comprehensive technical report.
    * `Model_Benchmarking_ROC_AUC_Evaluation.R`: Performance comparison scripts.
