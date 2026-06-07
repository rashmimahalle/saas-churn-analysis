
# SaaS Customer Churn Analysis

## Business Problem
A SaaS company with 5,000 subscriptions across 5 industries and 7 countries 
is experiencing 9.72% churn rate — above the industry benchmark of 5-7%. 
This analysis identifies the root causes of churn and provides actionable 
recommendations to reduce revenue loss.

## Dataset
- 5,000 subscription records
- 27 features including plan tier, tenure, usage events, MRR, ARR, industry, country
- Monthly churn trend data (2023-2024)

## Tools Used
- Python, Pandas, Matplotlib, Seaborn
- Google Colab

## Key Findings

### 1. Tenure is the #1 Churn Predictor (Correlation: -0.684)
- 100% of churned customers left before 13 months
- After 13 months churn rate drops to just 0.35%
- Critical danger zone: First 6 months of subscription

### 2. Enterprise Revenue at Serious Risk
- Enterprise plan accounts for 78% of all churned MRR ($926K out of $1.17M)
- Churned customers have HIGHER average MRR ($2,426) than active customers ($2,251)
- The company is losing its highest value customers disproportionately

### 3. Usage Does NOT Predict Churn
- Churned and active customers show almost identical usage patterns
- Problem is not product engagement — points to onboarding or expectation mismatch

### 4. Geography Matters
- France: highest churn at 11.85%
- India: lowest churn at 6.63%
- 5.22% gap suggests localization or support quality issues in certain markets

## Business Recommendations

| # | Recommendation | Impact |
|---|---------------|--------|
| 1 | Build 90-day onboarding program with check-ins at Day 30, 60, 90 | Reduce early tenure churn |
| 2 | Assign dedicated CSM to Enterprise accounts in first 6 months | Protect $926K MRR at risk |
| 3 | Create early warning system for Enterprise accounts with tenure < 6 months | Proactive retention |
| 4 | Investigate France market — exit interviews, localization review | Reduce 11.85% churn rate |
| 5 | Reframe success metrics from usage to tenure milestones | Better churn prediction |

## Project Structure
- `SaaS_Churn_Analysis.ipynb` — Main analysis notebook
- `subscriptions_enriched_copy.csv` — Main dataset
- `monthly_churn.csv` — Monthly churn trends
- `churn_dashboard.png` — Visual dashboard
- `usage_analysis.png` — Usage behaviour charts
- `monthly_trend.png` — Monthly trend chart

## Key Metric Summary
| Metric | Value |
|--------|-------|
| Total Subscriptions | 5,000 |
| Overall Churn Rate | 9.72% |
| Total MRR | $11,338,747 |
| MRR Lost to Churn | $1,179,139 |
| Revenue Churn Rate | 10.40% |
| Avg Tenure at Churn | 2.93 months |
