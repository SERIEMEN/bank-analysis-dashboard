# BANK ANALYSIS DASHBOARD PROJECT
This repo contains a bank analysis project done with Power BI and Excel
[https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/Screenshot%202026-08-24%20153606.png]
![dashboard](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/Screenshot%202026-08-24%20150751.png)
# Problem Statement: Bank Performance Analysis
Banks generate large volumes of customers, accounts, transactions, and loan data. Without effective analysis, management may struggle to understand customer behaviour, monitor transaction performance, identify loan risk, and compare branch performance.

This project focused on analyzing banking data to provide a consolidated view of customer demographics, account balances, transaction activity, loan exposure, default risk, and branch performance.

We used data analytics and visualization to answer key business questions and provide actionable insights to support customer management, operational monitoring, lending decisions, and branch-level performance evaluation.

## Technologies
+ Power BI — Dashboard development and data visualization
+ Power Query — Data cleaning and transformation
+ DAX — KPI and analytical measure creation
+ CSV — Source data format

**Skills Demonstrated**
- Data cleaning and preparation
- Data transformation
- Data modelling
- DAX calculations (Power BI)
- KPI development
- Exploratory data analysis
- Data visualization
- Business intelligence
- Insight generation
- Data storytelling

## Data Pipeline

Raw Banking Data
↓
Data Cleaning & Validation
↓
Data Transformation
↓
Data Modelling
↓
DAX Measures & KPIs
↓
Exploratory Data Analysis
↓
Power BI Dashboard
↓
Business Insights & Recommendations

## Methodology 
+ **Data Collection:** Five datasets were provided covering customers, accounts, branches, transactions, and loans.
- **Data Cleaning & Preparation:** The datasets were reviewed for data types, missing values, duplicates, inconsistent fields, and formatting issues, and were corrected accordingly.
- **Data Transformation:** The relevant fields were transformed and prepared for analysis, including transaction categories, account information, and loan status.
- **Data Modelling:** Relationships were established between customers, accounts, branches, transactions, and loans to create an integrated analytical model.
* **Measure & KPI Development:** Key metrics were created to evaluate customer volume, account balances, transaction activity, loan exposure, defaults, and branch performance.
* **Exploratory Analysis:** Customer, account, transaction, loan, and branch-level patterns were examined.
* Dashboard Development: The findings were presented through an interactive Power BI dashboard to allow users to explore the data across different business areas.
+ **Business Insight Generation:** The final stage involved interpreting the results and identifying areas requiring management attention.

## ANALYSIS
1. Customer Analysis
   - Customer Base: The bank has 500 customers across the available dataset.
   - Customer Demographics: The customer base is almost evenly distributed by gender:
      - Female: 254 customers (50.8%)
      - Male: 246 customers (49.2%)
   - The largest age group is customers aged 55 and above, with 145 customers.
   > *This indicates that the bank has a relatively mature customer base, which may have implications for product development, customer engagement, and financial-service offerings.*

2. Branch Account Distribution
   - Calabar Branch has the highest number of accounts, with 70 accounts.
   - Other branches with relatively high account volumes include Benin, Kano, Owerri, and Port Harcourt HQ.
   - Multiple-Account Customers: 202 customers, representing approximately 40.4% of the customer base, hold more than one account.
   - The highest number of accounts held by a single customer is 8.
     > *This indicates a substantial group of customers already using multiple banking products and represents a potential opportunity for deeper customer relationship management.*

2. Account Performance
 Total Account Balance
 - The combined balance across all accounts is approximately: ₦1.724 billion
Account Type Distribution
 - The dataset contains:
   - 248 Loan accounts — 35.4%
   - 231 Savings accounts — 33.0%
   - 221 Current accounts — 31.6%
 > Loan accounts represent the largest category in the supplied account data, although the distribution across the three categories is relatively balanced.
Branch Balances
- Calabar Branch records the highest aggregate account balance at approximately ₦173.94 million.
- This is consistent with its position as the branch with the highest account count and customer count.

3. Transaction Monitoring
  Transaction Volume
  - The dataset contains 10,000 transactions with a combined transaction value of approximately: ₦12.52 billion
  - Withdrawals represent the largest monetary transaction category, with approximately ₦6.29 billion in transaction value.

Deposits vs Withdrawals
- There were:
   - 2,502 deposits
   - 2,511 withdrawals
- By transaction count, activity is almost evenly balanced.
- However, the monetary value tells a different story:
   - Deposits: approximately ₦2.46 billion
   - Withdrawals: approximately ₦6.29 billion
- This gives a deposit-to-withdrawal value ratio of approximately 1:2.56.
> Therefore, although deposit and withdrawal transactions occur at similar frequencies, withdrawal values are substantially higher.

Transaction Trend

Transaction activity increased significantly from 2022 to 2024.

2024 recorded the highest activity among the complete years in the dataset, with approximately 3,346 transactions worth ₦4.24 billion.

The 2025 data should be interpreted cautiously because it does not represent a complete year.

Transaction Status

The transaction status distribution shows:

Completed: 33.06%
Failed: 33.47%
Pending: 33.47%

Therefore, approximately 66.94% of transactions are either failed or pending in the supplied dataset.

This is a major operational finding that warrants investigation.

Because the dataset is a practice dataset, this result should be treated as an analytical observation rather than assumed to represent actual banking-system performance.

4. Loan Risk & Exposure
Total Loan Exposure

The bank's total loan exposure is approximately:

₦726.48 million

Loan Volume by Branch

Owerri Branch issues the highest number of loans, with 27 loans.

However, loan volume and loan value produce different results.

- Highest Loan Exposure by Branch
 - Enugu Central has the highest aggregate loan value at approximately: ₦58.63 million

This demonstrates why branch performance should be evaluated using multiple KPIs rather than loan count alone.

Loan Status Distribution

The 300 loans are distributed as follows:

Approved: 112 (37.33%)
Pending: 99 (33.00%)
Defaulted: 89 (29.67%)
Default Risk

Defaulted loans represent approximately 29.67% of all loans.

The value of defaulted loans is approximately ₦218.06 million, representing about 30% of total loan exposure.

This indicates a significant level of credit risk within the dataset and should be a major area of management attention.

5. Branch Performance
Branch Customer Volume

Calabar Branch serves the highest number of unique customers, with 66 customers associated with its accounts.

Branch Account Volume

Calabar also records the highest account volume with 70 accounts.

Branch Loan Activity

There is a difference between the branch with the highest number of loans and the branch with the highest loan value:

Highest number of loans: Owerri Branch — 27
Highest loan value: Enugu Central — ₦58.63M
Revenue Analysis Limitation

Actual branch revenue could not be directly measured from the available data because the dataset does not contain a dedicated revenue, income, or profit field.

Transaction value and loan value can be used as indicators of business activity, but they should not be presented as revenue.

Results

The analysis produced several key findings:

Customer Insights
The bank has 500 customers.
Customer demographics are almost evenly split by gender.
Customers aged 55+ form the largest age group.
40.4% of customers hold multiple accounts.
Calabar Branch has the highest account and customer volume.

Account Insights

Total account balances amount to approximately ₦1.724 billion.
Calabar Branch holds the highest aggregate account balance at approximately ₦173.94 million.
Account types are relatively evenly distributed.

Transaction Insights
The dataset contains 10,000 transactions worth approximately ₦12.52 billion.
Withdrawals have substantially greater monetary value than deposits.
Transaction activity reached its highest complete-year level in 2024.
Failed and pending transactions together represent approximately 66.94% of transactions.

Loan Insights

Total loan exposure is approximately ₦726.48 million.
89 loans are classified as defaulted.
Defaulted loans represent approximately 29.67% of all loans and about ₦218.06 million in exposure.
Owerri leads in loan count, while Enugu Central leads in total loan value.

# Recommendations

1. Investigate Failed and Pending Transactions

The high proportion of failed and pending transactions should be investigated to identify whether the issue is caused by system failures, processing delays, payment-channel problems, or data-recording issues.

Management should monitor transaction success rates regularly and establish service-level targets for resolving pending transactions.

2. Strengthen Credit Risk Management

With approximately ₦218 million associated with defaulted loans, the bank should strengthen its credit-risk monitoring process.

Potential actions include:

+ Reviewing borrower risk profiles
+ Monitoring repayment behaviour
+ Strengthening credit assessment
+ Introducing early-warning indicators
+ Prioritizing high-value default exposures

3. Leverage Multi-Account Customers

More than 40% of customers hold multiple accounts.

The bank could use customer behaviour and account information to identify opportunities for:

+ Cross-selling
+ Personalized product recommendations
+ Customer retention
+ Relationship management
  
4. Investigate High Withdrawal Values

Withdrawals are substantially higher in value than deposits.

The bank should monitor the underlying reasons for this pattern and evaluate whether it reflects normal customer behaviour, specific customer segments, particular branches, or periods of unusually high withdrawals.

5. Benchmark Branches Using Multiple KPIs

Branch performance should not be evaluated using account count alone.

A more comprehensive branch scorecard could include:

* Number of customers
* Number of accounts
* Total account balance
* Transaction value
* Transaction success rate
* Loan volume
* Loan exposure
* Default rate

This would provide management with a more balanced view of branch performance.

6. Improve Revenue Data Collection

Because the current dataset does not contain a revenue field, future analysis should incorporate revenue-related data such as:

- Account fees
- Transaction fees
- Loan interest income
- Service charges
- Other banking income

This would allow actual branch profitability and revenue contribution to be measured.

Overall Business Conclusion

The analysis provides a consolidated view of the bank's customer base, account balances, transaction activity, loan exposure, and branch performance.

The strongest opportunities identified are improving transaction reliability, strengthening credit-risk management, leveraging multi-account customers, and developing more comprehensive branch-performance metrics.

Calabar stands out for customer and account activity, while the loan analysis highlights a significant level of default exposure that requires attention.

Overall, the project demonstrates how Power BI can transform raw banking data into an interactive decision-support tool that enables management to move from simply viewing data to identifying patterns, risks, opportunities, and areas requiring action.

## What I learned

## Preview
