# Customer Churn Prediction 📉

## Overview
Built a machine learning model to predict customer churn for a telecom company. The model identifies customers at risk of leaving, enabling proactive retention strategies.

## Tools & Libraries
Python, pandas, numpy, matplotlib, scikit-learn

## Dataset
- Source: [IBM Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 7,043 customers, 21 features
- Churn rate: 26.6%

## Key EDA Findings
- Month-to-month contracts → 42.7% churn rate
- Electronic check payment → 45.3% churn rate
- Fiber optic internet → 41.9% churn rate
- New customers (0-10 months) churn most frequently

## Model Results

| Model | Accuracy | Precision (churn) | Recall (churn) | ROC-AUC |
|---|---|---|---|---|
| Logistic Regression | 0.787 | 0.62 | 0.52 | 0.832 |
| Random Forest | 0.790 | 0.63 | 0.48 | — |

Logistic Regression selected as final model — better recall on churn class.

## Business Impact
- 63 churners missed in test set
- Average monthly charge: $64.8
- **Monthly revenue at risk: $4,082**
- Estimated annual loss on full base: ~$245,000

## Files
- `customer_churn_prediction.ipynb` — full analysis notebook
