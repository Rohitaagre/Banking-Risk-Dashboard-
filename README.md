# Banking Risk Analytics Dashboard (Power BI)

An interactive two-page Power BI dashboard built to monitor loan portfolio health and quantify credit risk exposure across branches, credit-score segments, and loan types — using a synthetic banking dataset of 150 loan applications across 30 customers and 8 branches.

## Overview

This dashboard was designed to move beyond basic portfolio reporting and answer real risk-management questions: which branches carry the most exposure, which credit-score segments default most often, and how default rates trend over time. It combines KPI cards, trend analysis, and risk-segmented breakdowns into a single, filterable view.

## Dashboard Pages

### Page 1 — Portfolio Overview
![Portfolio Overview](screenshots/page1-portfolio-overview.png)

Tracks the overall loan book: total loan amount, outstanding balance, default rate, active loans, and customer count, broken down by occupation, age bracket, gender, customer segment, loan status, and loan type.

### Page 2 — Risk Analytics
![Risk Analytics](screenshots/page2-risk-analytics.png)

Focused entirely on risk: amount at risk by branch, default rate by credit-score band, default rate by loan type, default rate trend over time, and portfolio distribution by risk category.

## Key Insights

- Tracked a **$270M+ loan portfolio** across 102 active loans, using custom DAX measures to quantify default rate, exposure, and risk across branches, credit scores, and loan types.
- Uncovered a **16.7% peak default rate** within the "Fair" credit-score segment and **$3.6M+ exposure** concentrated in a single branch, enabling targeted, data-driven risk mitigation decisions.
- Identified default rate spikes exceeding **20%** in specific months (May, September) and seasonal risk patterns across the loan portfolio, enabling proactive monitoring through an interactive trend-analysis view.

## Key DAX Measures

| Measure | Purpose |
|---|---|
| `Default Rate` | Defaults ÷ total loans, overall and by segment |
| `Amount at Risk` | Sum of outstanding balance on defaulted loans |
| `% Portfolio at Risk` | Amount at Risk ÷ Total Loan Amount |
| `CreditScoreBand` | Buckets raw credit scores into Poor / Fair / Good / Excellent |
| `MonthStart` | Normalizes application dates to enable accurate month-over-month trend analysis |

## Tools Used

- **Power BI Desktop** — data modeling, DAX measures, visualization
- **DAX** — custom measures for risk and default metrics
- **Excel** — source data (loan facts, product/loan-type reference, customer demographics)

## Data Note

This project uses a synthetic/sample banking dataset created for portfolio and learning purposes — it does not represent real customer or loan data.
