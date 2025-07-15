# 📦 Customer Churn Prediction for Kevidko

This project builds a churn prediction system using actual B2B sales data from Kevidko, a wholesale food distributor. It identifies potentially inactive customers and supports proactive retention strategies for the sales team.

## 📌 Project Overview

In Kevidko's daily operations, hundreds of orders are placed by repeat customers. However, some clients gradually reduce or stop ordering, indicating possible churn. This project uses data-driven methods to:

- Segment customers based on purchase behavior
- Predict churn likelihood
- Support targeted outreach and retention

## 🧠 Methodology

- **Feature Engineering**: RFM model (Recency, Frequency, Monetary)
- **Handling Imbalanced Data**: SMOTE oversampling
- **Model**: Logistic Regression
- **Evaluation Metrics**: Confusion Matrix, ROC Curve, AUC Score

## 📈 Key Results

- **Accuracy**: ~97%
- **AUC Score**: 1.00 (excellent model separation)
- **Output**:
  - Churn prediction (0 or 1)
  - Churn probability for each customer
  - Ranked customer list by risk level

## 🛠 Tools & Libraries

- **Python**: `pandas`, `scikit-learn`, `imbalanced-learn`, `matplotlib`
- **Jupyter Notebook**: for end-to-end development
