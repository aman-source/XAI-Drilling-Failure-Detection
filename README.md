# 🛠️ XAI-Based Drilling Failure Detection

This project uses machine learning and explainable AI (XAI) to predict drilling failures and specific failure modes in synthetic industrial drilling operations. Built with real-world-inspired data, the pipeline demonstrates how AI can enhance decision-making and reliability in oil & gas and manufacturing sectors.

## 🔍 Project Objectives

- **Binary classification**: Predict whether a drilling operation will result in failure (`Main Failure`).
- **Multi-label classification**: Identify specific failure types:
  - BEF: Build-up Edge Failure
  - CCF: Compression Chips Failure
  - FWF: Flank Wear Failure
  - WDF: Wrong Drill Bit Failure
- **Explainability**: Use SHAP to interpret model predictions and build trust in AI outcomes.

---

## 📁 Dataset

- **Name**: [XAI Drilling Dataset](https://www.kaggle.com/datasets/raphaelwallsberger/xai-drilling-dataset)
- **Source**: Kaggle (synthetic data based on real machining parameters)
- **Samples**: 20,000 records
- **Features**: Cutting speed, spindle speed, feed rate, power, material type, cooling %, drill bit type, etc.

---

## ⚙️ Technologies Used

- Python (Pandas, NumPy, Scikit-learn)
- XGBoost (for binary and multi-label classification)
- SHAP (for model explainability)
- Matplotlib / SHAP plots for visualization

---

## ✅ Results

### 🎯 Binary Classification (`Main Failure`)
- Accuracy: **99.85%**
- F1-score (Failure): **98.5%**
- ROC AUC: **0.9999**

### 🔁 Multi-Label Failure Mode Classification
- F1-score for all failure types: **1.0**
- Model perfectly predicted all failure labels (BEF, CCF, FWF, WDF)

### 📊 SHAP Explainability
- Key failure drivers identified:
  - High feed rate
  - High cutting speed
  - Drill bit type N
  - Low cooling %

---

## 📌 Features

- Full ML pipeline: preprocessing, scaling, one-hot encoding
- Imbalance handling using class weights
- Multi-output XGBoost classification
- Global and local interpretability using SHAP plots (summary, waterfall)
- Clean and modular Jupyter Notebook structure

---

