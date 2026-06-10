# 🏦 Bank Marketing Campaign Analysis

**Dataset:** [Bank Marketing — UCI ML Repository](https://www.kaggle.com/datasets/henriqueyamahata/bank-marketing)  
**Records:** 41,188 clients · 21 features  
**Tools:** Python · pandas · scipy · matplotlib

## 🎯 Goal
Identify which client segments are most likely to subscribe to a term deposit
to focus campaign budget and improve conversion rate.

## 🔍 Key Findings
- Overall conversion: 11.3% — strong class imbalance
- Best segment: retired (25%) and students (31%) — 3–4x higher than blue-collar (7%)
- Age 60+ converts at 46% — 5x higher than 41–50 (9%)
- Call duration: subscribers talk 2.5x longer, p-value ≈ 0 ⚠️ correlation, not causation
- High conversion in March/December explained by targeting strategy, not seasonality (selection bias)

## 🛠️ Methods
- EDA: segmentation by job, age group, month
- pd.cut() for age binning
- A/B test: scipy.stats.ttest_ind (call duration vs outcome)
- Selection bias detection: conversion rate vs call volume by month

## 💡 Recommendation
Focus on retired clients aged 60+ in autumn/winter months.
Avoid mass calling in May — high volume, low return.
