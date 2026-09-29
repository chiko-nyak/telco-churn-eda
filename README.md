# telco-churn-eda
## Business Question
Do month-to-month contracts and lack of tech support predict churn more than monthly charges do?

## Method
Exploratory data analysis in R (dplyr, ggplot2, tidyr) on the Kaggle Telco Customer Churn
dataset (7,043 customers). Churn rates were cross-tabulated against contract type, tech
support subscription, payment method, and tenure, then visualized to identify which
attributes separate churners from retained customers most clearly.

## Findings
1. **Contract type** is the strongest driver of churn: month-to-month customers churn at
   ~42%, compared to ~11% for one-year contracts and under 3% for two-year contracts — a
   roughly 15x gap between the extremes.
2. **Tech support** shows a similar pattern: customers without tech support churn at ~42%,
   nearly 3x the rate of customers who have it (~15%).
3. **Tenure and churn are inversely related** — churned customers cluster at low tenure,
   suggesting risk is highest early in the customer relationship.

## So What
Retention efforts should prioritize month-to-month customers without tech support,
especially early in their tenure. Bundling free tech support for that segment in their
first few months is likely to reduce churn more effectively than a price discount would —
the pattern points to service gaps, not price sensitivity, as the bigger risk factor.

[View the full analysis](analysis.html)
