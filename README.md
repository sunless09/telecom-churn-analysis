# Telecom Customer Churn Analysis

Exploratory Data Analysis of customer churn using a real telecom dataset (7,032 customers).  
Tools: Python, pandas, matplotlib, seaborn.

## Business Question
Which customers are most likely to churn, and why?

## Key Findings

### 1. Contract type is the strongest predictor of churn
- Month-to-month customers churn at a dramatically higher rate than annual/biannual customers
- Reason: low barrier to exit — no financial penalty for leaving
- **Business recommendation:** incentivize customers to switch to longer contracts via cashback or bonuses

### 2. Churned customers pay more
- Average monthly charge: **$74.4** (churned) vs **$61.3** (retained)
- The difference holds even after controlling for contract type (no confounding)
- Reason: higher-paying customers are more demanding and more likely to compare alternatives
- **Business recommendation:** prioritize retention efforts for high-value customers

### 3. Early churn is critical — the first 10 months are decisive
- Median tenure of churned customers: **10 months**
- 50% of all churned customers left within the first 10 months
- Customers who survive past ~12 months show dramatically lower churn probability
- **Business recommendation:** invest heavily in onboarding experience during the first 3–6 months

## Dataset
[IBM Telco Customer Churn](https://github.com/IBM/telco-customer-churn-on-icp4d)  
7,043 customers · 21 features · binary churn label

## Structure
```
telecom-churn-analysis/
│
└── notebook.ipynb   # Full analysis with visualizations
```
