# Customer Retention & Churn Analysis
Dataset

RavenStack subscription data — 500 SaaS accounts across two years, including account details, subscription history, churn events, support tickets, and feature usage.

What the Dashboard Includes
KPI cards: Total Accounts, Churned Accounts, Churn Rate, Current MRR, Avg Tenure
Cohort retention matrix (signup quarter × months since signup, heatmapped)
Churn events over time, by month
Churn reasons breakdown
Churn rate by industry, referral source, and plan tier
Insights & recommendations summary

Key Insights
Overall churn rate is 22.0% (110 of 500 accounts), but churn is not evenly spread.
44% of all churned accounts left in the final quarter alone (Oct–Dec 2024) — every signup cohort dropped off sharply in that same window, not just new signups. This points to one company-wide trigger, not gradual customer aging.
DevTools churns at 31.0% vs. 16.0% for Cybersecurity; event-sourced signups churn at 30.2% vs. 14.6% for partner referrals — roughly 2x spread on both.
Plan tier is not a driver — Basic, Pro, and Enterprise all sit near 22% churn.
Support ticket volume and satisfaction score show no meaningful correlation with churn.
Top stated churn reasons are features and budget, together 36% of all churn events.
Retained accounts carry an estimated CLV ~37% higher than accounts that eventually churn.

Recommendations
Investigate the Oct–Dec 2024 event directly before acting on segment data — it's the single biggest lever.
Prioritize DevTools and event-channel accounts for proactive retention outreach.
Close the features gap; pilot a lower-commitment or usage-based tier for budget-driven churn.
Don't allocate retention budget by plan tier — it shows no meaningful difference in churn rate.
Files
retention_dashboard.pbix — full Power BI report
churn_analysis.py — Python script reproducing the churn, tenure, and cohort calculations behind the dashboard
ravenstack_accounts.csv, ravenstack_subscription.csv, ravenstack_churn_events.csv, ravenstack_support_tickets.csv, ravenstack_feature_usage.csv — source data
Tools

Power BI Desktop (Power Query, DAX), Python (pandas)

Author

Zakhele
