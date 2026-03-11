# Customer Churn Prediction

## Overview
An end-to-end machine learning pipeline to predict customer churn using the IBM Telco Customer Churn dataset (7,043 records, 21 features). The project covers data cleaning, feature engineering, model training, and explainability using SHAP.

## Results
- **ROC-AUC Score: 0.84** using XGBoost
- **Accuracy: 80%** on held-out test set
- Key churn drivers identified: month-to-month contracts, low tenure, high monthly charges, and lack of online security

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, XGBoost, SHAP, Matplotlib, Seaborn

## Project Structure
```
churn-prediction/
│
├── churn_analysis.ipynb       # Main notebook
├── shap_feature_importance.png
├── shap_summary.png
├── churn_distribution.png
└── README.md
```

## Key Steps
1. **Data Cleaning** — Converted TotalCharges to numeric, handled nulls, encoded categorical variables
2. **Modelling** — Trained XGBoost classifier with 80/20 train-test split
3. **Evaluation** — Achieved 0.84 ROC-AUC with statistical validation
4. **Explainability** — Applied SHAP to identify and visualise key churn drivers

## Business Insight
Customers on month-to-month contracts churn at 43% — compared to just 3% on two-year contracts. Targeted retention strategies for this segment could significantly reduce revenue loss.

## Dataset
[IBM Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)