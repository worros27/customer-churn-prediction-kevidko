# 📦 Customer Churn Prediction for Kevidko

This project builds a **customer churn prediction system** based on real B2B sales data from **Kevidko**, a wholesale food distributor in Los Angeles. The system identifies potentially inactive customers and supports **proactive retention** efforts by the sales and operations team.

---

## 📌 Project Overview

Kevidko processes hundreds of repeat customer orders daily. However, some clients gradually reduce or stop ordering, indicating potential churn. To support data-driven intervention, this project was developed to:

- Segment customers based on purchasing behavior
- Detect signs of declining engagement
- Predict churn likelihood with classification models
- Prioritize high-risk customers for follow-up

---

## 🧠 Methodology

### 1. Feature Engineering
- Applied **RFM analysis**:
  - **Recency**: Days since last purchase  
  - **Frequency**: Number of orders  
  - **Monetary**: Total spend  

### 2. Labeling
- Customers inactive for 90+ days were labeled as **churned (1)**.

### 3. Handling Imbalanced Data
- Used **SMOTE** (Synthetic Minority Oversampling Technique) to balance the churn class.

### 4. Models & Evaluation
- **Models**: Logistic Regression, Random Forest, XGBoost
- **Validation**: 5-fold Stratified Cross-Validation
- **Metrics**: Confusion Matrix, ROC Curve, AUC Score

---

## 📈 Key Results

| Model              | Average AUC |
|-------------------|-------------|
| Logistic Regression | **1.000**     |
| Random Forest       | **1.000**     |
| XGBoost             | **0.9913**    |

- ✔️ **Churn prediction labels (0 or 1)**
- ✔️ **Churn probability for each customer**
- ✔️ **Risk-ranked customer list for sales team**

> The models showed excellent class separation. Despite the simplicity of features, the predictions aligned well with business expectations.

---

## 🗂 Output Files

- `customer_churn_flag.csv`: Cleaned, labeled training data  
- `predict_with_result.csv`: Final predictions with probabilities  
- `churn_modeling.ipynb`: Full modeling pipeline  
- `churn_prediction.ipynb`: Prediction + export pipeline  
- `README.md`: Project documentation

---

## 🛠 Tools & Libraries

- **Python**
  - `pandas`, `numpy`, `scikit-learn`, `xgboost`, `imbalanced-learn`, `matplotlib`
- **Jupyter Notebook**
  - For development and visualization
- **GitHub**
  - For version control and public showcase

---

## 📊 Optional Enhancements

- Tableau dashboard integration
- Streamlit for internal decision tool
- Time-series trend monitoring for advanced pattern recognition

---

