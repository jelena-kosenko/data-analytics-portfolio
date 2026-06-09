# 📣 Marketing Attribution & A/B Test Analysis

**Dataset:** [Marketing Campaign Performance Dataset](https://www.kaggle.com/datasets/manishabhatt22/marketing-campaign-performance-dataset)  
**Records:** 200,000 marketing campaigns  
**Tools:** Python · pandas · scipy · matplotlib

## 🎯 Goal
Identify the best-performing marketing channel by Conversion Rate and ROI.  
Apply statistical testing to determine whether observed differences are significant or random.

## 🔍 Key Findings
- All 6 channels show identical Conversion Rate (~0.08) and ROI (~5.0)
- t-test p-value: 0.7382 → no significant difference between best and worst channel
- ANOVA p-value: 0.7159 → no significant difference across all 6 channels
- No statistical evidence to reallocate budget between channels

## 🛠️ Methods
- EDA: groupby aggregation, bar charts, boxplot
- t-test: Facebook vs Instagram (scipy.stats.ttest_ind)
- ANOVA: all 6 channels (scipy.stats.f_oneway)
