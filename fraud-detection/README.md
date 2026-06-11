# 🔍 Credit Card Fraud Detection

**Dataset:** [Credit Card Fraud Detection — Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
**Records:** 284,807 transactions · 31 features  
**Tools:** Python · pandas · scikit-learn · matplotlib

## 🎯 Goal
Detect fraudulent credit card transactions using anomaly detection (Isolation Forest).  
Real anonymized data from European cardholders (September 2013).

## 🔍 Key Findings
- Only 0.17% of transactions are fraudulent — extreme class imbalance
- Fraud median amount: $9 vs Normal: $22 — card testing pattern detected
- Isolation Forest (6 features): recall 20%
- Isolation Forest (all 30 features): recall 28%
- Honest result: unsupervised methods are limited — supervised models would perform better

## 🛠️ Methods
- EDA: class imbalance analysis, amount distribution
- Statistical comparison: mean vs median (normal vs fraud)
- Anomaly detection: Isolation Forest (scikit-learn)
- Model evaluation: precision, recall, F1-score
- Feature impact: 6 features vs all 30 features comparison

## 💡 Conclusion
Isolation Forest is valuable for detecting unknown fraud patterns (no labels needed).  
For known fraud, supervised models (Random Forest, XGBoost) perform significantly better.  
In production, anomaly detection serves as a first-pass filter, not a final decision.
