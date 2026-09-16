# Transaction Fraud Detection System

An end-to-end machine learning system designed to identify and prevent fraudulent financial transactions using supervised classification algorithms on tabular data.

---

## 📌 Overview
Financial fraud detection presents a classic machine learning challenge: extreme class imbalance, where legitimate transactions vastly outnumber fraudulent ones. Standard accuracy metrics fail in this domain. 

This project implements a complete machine learning pipeline—from raw data ingestion and feature engineering to imbalance handling and model evaluation—focused strictly on optimizing **Precision**, **Recall**, and **F1-Score**.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Data Processing & Analysis:** pandas, NumPy
* **Machine Learning:** scikit-learn
* **Environment:** Jupyter Notebook

---

## 🚀 Key Pipeline Steps

### 1. Data Preprocessing & Cleaning
* Cleaned raw transaction logs by removing duplicate records and handling missing values.
* Scaled numeric features (e.g., transaction amounts) using robust scaling to mitigate outlier impact.

### 2. Feature Engineering
* Extracted temporal features from transaction timestamps (hour, day of week, peak vs. off-peak hours).
* Engineered aggregations and behavioral indicators to highlight anomalous spending patterns.

### 3. Class Imbalance Mitigation
* Addressed severe target class skew using specialized resampling techniques (e.g., SMOTE / Random Undersampling / Class Weighting).
* Enforced strict train/test splitting prior to resampling to prevent data leakage.

### 4. Model Training & Evaluation
* Trained and benchmarked multiple supervised classifiers (e.g., Logistic Regression, Random Forest, Gradient Boosting).
* Prioritized performance evaluation around **Precision, Recall, F1-Score, and PR-AUC** over raw accuracy.

---

## 📊 Evaluation Focus

| Metric | Target Goal in Fraud Detection |
| :--- | :--- |
| **Precision** | Minimize false positives (avoid freezing legitimate users' accounts). |
| **Recall** | Maximize true positives (catch as many fraudulent transactions as possible). |
| **F1-Score** | Balance precision and recall for optimal overall fraud strategy. |

---

