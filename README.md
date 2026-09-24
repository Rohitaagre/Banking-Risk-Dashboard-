# Banking Risk Dashboard – Power BI

An interactive Power BI dashboard analyzing a bank's loan portfolio 
across 102 loans and 30 customers, tracking key risk metrics such as 
default rate, outstanding balance, and portfolio distribution by risk 
category, geography, and customer demographics.

## Dataset
Relational dataset with three tables:
- **Loan_Fact** – loan-level transactional data (amount, EMI, status, default flag)
- **PROD** – loan product details (type, interest rate, risk category, tenure)
- **CUST** – customer demographics (age, gender, occupation, income band, credit score)

## Key KPIs Tracked
- Total Loan Portfolio: ₹270M
- Outstanding Balance: ₹89.2M
- Default Rate: 13%
- Active Loans: 102 | Customers: 30

## Key Insight
"High-risk category loans showed a default rate of X% roughly 
Nx higher than low-risk loans, Unsecured loans (Personal, Gold) showed higher default rates than secured loans (Home, LAP) — consistent with collateral reducing default risk. "]

## Tools Used
Power BI (Power Query for data transformation, data modeling across 
fact/dimension tables), Excel

## How to View
Download the .pbix file and open in Power BI Desktop, or view the 
screenshots above for a quick overview.
