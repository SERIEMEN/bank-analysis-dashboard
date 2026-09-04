# BANK ANALYSIS DASHBOARD PROJECT
This repo contains a bank analysis project done with Power BI and Excel

![dashboard](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-08-24%20153606.png)

## Table of Contents

- [Problem Statement](#problem-statement)
- [Technologies](#technologies)
- [Skills demonstrated](#skills-demonstrated)
- [Methodology](#methodology)
  - [Data Pipeline Overview](#data-pipeline-overview)
  - [Data Collection](#data-collection)
    - [About the Dataset](#about-the-dataset)
  - [Data Cleaning & Preparation](#data-cleaning--preparation)
  - [Data Transformation](#data-transformation)
  - [Data Modelling](#data-modelling)
  - [Measure & KPIs used](#measure--kpis-used)
  - [Exploratory Analysis](exploratory-analysis)
  - [Dashboard Development](#dashboard-development)
  - [Insight Generation](#insight-generation)
- [Analysis](#analysis)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)
- [Dashboard](#dashboard)
- [Conclusion](#conclusion)

# Problem Statement
Banks generate large volumes of customers, accounts, transactions, and loan data. Without effective analysis, management may struggle to understand customer behaviour, monitor transaction performance, identify loan risk, and compare branch performance.

This project focused on analyzing banking data to provide a consolidated view of customer demographics, account balances, transaction activity, loan exposure, default risk, and branch performance.

We used data analytics and visualization to answer key business questions and provide actionable insights to support customer management, operational monitoring, lending decisions, and branch-level performance evaluation.

## Technologies
+ Power BI — Dashboard development and data visualization
+ Power Query — Data cleaning and transformation
+ DAX — KPI and analytical measure creation
+ CSV — Source data format

## Skills Demonstrated
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

## Methodology 

### Data Pipeline Overview

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

+ ### Data Collection
   Five datasets were provided covering accounts, customers, transactions, loans, and branches.
   #### About the Dataset
    - Accounts: (700 rows). Each account belongs to a customer with an ID, at a specific branch, an account type(loans, savings, current), and a balance.
    - Customers: (500 rows). It contains necessary information of the customers (name, age, gender, address, phone number, email, and their identification number).
    - Transactions: (10000 rows). A transaction identification number for each transaction for effective tracking of customer IDs and account IDs, respectively, for accuracy, which transaction type was made (deposit, withdrawal, and bill payment), and the amount.
    - Loans: (300 rows). A loan ID is allocated to each customer who took out a loan, along with the branch it was taken from, how much they took, and the interest rate for each of them, the status of the loan, and whether it has been approved, pending, or defaulted.
    - Branches: (15 rows). 15 branches located at Lagos, Calabar, Port-Harcourt, Abuja, Kaduna, Enugu, Kano, Ibadan, Benin, Jos, Maiduguri, Owerri, Abeokuta, Asaba, and Ilorin.

- ### Data Cleaning & Preparation
   The datasets were reviewed for data types, missing values, duplicates, inconsistent fields, and formatting issues, and were corrected accordingly.
- ### Data Transformation
   The relevant fields were transformed and prepared for analysis, including transaction categories, account information, and loan status.
  
  #### Date table created
  ![datetable](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-09-02%20073802.png)

  Age distribution column created to understand which age grade performs more transactions at the bank

  ![age distribution](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-09-02%20065924.png)
  
- ### Data Modelling
    Relationships were established between customers, accounts, branches, transactions, and loans to create an integrated analytical model.

  #### Relationship between the tables

  ![modelling](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-08-28%20133941.png)

- ### Measure & KPIs used

  ![dax creation](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-09-02%20074525.png)

- ### Exploratory Analysis
  Customer, account, transaction, loan, and branch-level patterns were examined.
- ### Dashboard Development
  The findings were presented through an interactive Power BI dashboard to allow users to explore the data across different business areas.
- ### Insight Generation
  The final stage involved interpreting the results and identifying areas requiring management attention.

   
## ANALYSIS
### 1. Customer Analysis

![dashboard](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-08-28%20165536.png)

   #### a.	How many customers does the bank have?
         - Customer Base: The bank has 500 customers across the available dataset.
   #### b.	What is the customer demographic distribution (age, gender)?
       Customer Demographics: The customer base is almost evenly distributed by gender:
        - Female: 254 customers (50.8%)
        - Male: 246 customers (49.2%)
        - The largest age group is customers aged 55 and above, with 145 customers.
       > This indicates that the bank has a relatively mature customer base, which may have implications for product development, customer engagement, and financial-service offerings.

   #### c.	Which branches have the most accounts
        - Calabar Branch has the highest number of accounts, with 70 accounts.
        - Other branches with relatively high account volumes include Benin, Kano, Owerri, and Port Harcourt HQ.

   #### d.	Which customers have multiple accounts?
       - Multiple-Account Customers: 202 customers, representing approximately 40.4% of the customer base, hold more than one account.
       - The highest number of accounts held by a single customer is 8.
       > This indicates a substantial group of customers already using multiple banking products and represents a potential opportunity for deeper customer relationship management.

 
### 2. Account Performance

  #### a.	What is the total balance across all accounts?
       The combined balance across all accounts is approximately ₦1.724 billion

  #### b.	Which account type is most popular?
      The dataset contains:
       - 248 Loan accounts — 35.4%
       - 231 Savings accounts — 33.0%
       - 221 Current accounts — 31.6%
    > Loan accounts represent the largest category in the supplied account data, although the distribution across the three categories is relatively balanced.

 #### c.	Which branches hold the highest deposits?
     - Calabar Branch records the highest aggregate account balance at approximately ₦173.94 million.
     - This is consistent with its position as the branch with the highest account count and customer count.
    
### 3. Transaction Monitoring

![dashboard](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-08-24%20150751.png)

 #### a. What is the total transaction volume?
    - The dataset contains 10,000 transactions with a combined transaction value of approximately ₦12.52 billion
    - Withdrawals represent the largest monetary transaction category, with approximately ₦6.29 billion in transaction value.

 #### b.	What is the deposit-to-withdrawal ratio?
      - There were:
       - 2,502 deposits
       - 2,511 withdrawals
     - By transaction count, activity is almost evenly balanced. However, the monetary value tells a different story:
         - Deposits: approximately ₦2.46 billion
         - Withdrawals: approximately ₦6.29 billion
     - This gives a deposit-to-withdrawal value ratio of approximately 1:2.56.
       > Therefore, although deposit and withdrawal transactions occur at similar frequencies, withdrawal values are substantially higher.

  #### c.	How do transactions change over time?
    - Transaction activity increased significantly from 2022 to 2024. 2024 recorded the highest activity among the complete years in the dataset, with approximately 3,346 transactions worth ₦4.24 billion.
    - The 2025 data should be interpreted cautiously because it does not represent a complete year.

#### d.	What percentage of transactions fail or remain pending?
    The transaction status distribution shows:
       - Completed: 33.06%
     	 - Failed: 33.47%
       - Pending: 33.47%
     Therefore, approximately 66.94% of transactions are either failed or pending in the supplied dataset. This is a major operational finding that warrants investigation. Because the dataset is a practice dataset, this result should be treated as an analytical observation rather than assumed to represent actual banking-system performance.

### 4. Loan Risk & Exposure

![dashboard](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/images/Screenshot%202026-08-28%20165557.png)

   #### a.	What is the total loan exposure of the bank?
       The bank's total loan exposure is approximately ₦726.48 million

   #### b.	Which branches issue the most loans?
       Owerri Branch issues the highest number of loans, with 27 loans.

      However, loan volume and loan value produce different results.
            - Highest Loan Exposure by Branch
            - Enugu Central has the highest aggregate loan value at approximately ₦58.63 million
    > This demonstrates why branch performance should be evaluated using multiple KPIs rather than loan count alone.

   #### c.	What is the loan status distribution (active, defaulted)?
           The 300 loans are distributed as follows:
           - Approved: 112 (37.33%)
           - Pending: 99 (33.00%)
           - Defaulted: 89 (29.67%)

   #### d.	What is the default risk level?
    - Defaulted loans represent approximately 29.67% of all loans.
    - The value of defaulted loans is approximately ₦218.06 million, representing about 30% of total loan exposure.
    - This indicates a significant level of credit risk within the dataset and should be a major area of management attention.

### 5. Branch Performance

  #### a.	Which branches generate the most revenue?
       Calabar Branch generates the most revenue, with about ₦441 million in completed transaction value—roughly 17% above Benin, the second-highest.

  #### b.	Which branches handle the most customers?
       Calabar Branch serves the highest number of unique customers, with 66 customers associated with its accounts. Calabar records the highest account volume with 70 accounts.

  #### c. Which branches issue the highest loan amounts?
      There is a difference between the branch with the highest number of loans and the branch with the highest loan value:
      - Highest number of loans: Owerri Branch — 27
      - Highest loan value: Enugu Central — ₦58.63M

## Key Findings

The analysis produced several key findings:

### Customer Insights

- The bank has 500 customers.
- Customer demographics are almost evenly split by gender.
- Customers aged 55+ form the largest age group.
- 40.4% of customers hold multiple accounts.
- Calabar Branch has the highest account and customer volume.

### Account Insights

- Total account balances amount to approximately ₦1.724 billion.
- Calabar Branch holds the highest aggregate account balance at approximately ₦173.94 million.
- Account types are relatively evenly distributed.

### Transaction Insights

- The dataset contains 10,000 transactions worth approximately ₦12.52 billion.
- Withdrawals have substantially greater monetary value than deposits.
- Transaction activity reached its highest complete-year level in 2024.
- Failed and pending transactions together represent approximately 66.94% of transactions.

### Loan Insights

- Total loan exposure is approximately ₦726.48 million.
- 89 loans are classified as defaulted.
- Defaulted loans represent approximately 29.67% of all loans and about ₦218.06 million in exposure.
- Owerri leads in loan count, while Enugu Central leads in total loan value.

## Recommendations

1. Investigate Failed and Pending Transactions

    The high proportion of failed and pending transactions should be investigated to identify whether the issue is caused by system           failures, processing delays, payment-channel problems, or data-recording issues.\
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
   
    More than 40% of customers hold multiple accounts. The bank could use customer behaviour and account information to identify opportunities for:
     + Cross-selling
     + Personalized product recommendations
     + Customer retention
     + Relationship management
  
4. Investigate High Withdrawal Values
      Withdrawals are substantially higher in value than deposits. The bank should monitor the underlying reasons for this pattern and evaluate whether it reflects normal customer behaviour, specific customer segments, particular branches, or periods of unusually high withdrawals.

5. Benchmark Branches Using Multiple KPIs
   
   Branch performance should not be evaluated using account count alone. A more comprehensive branch scorecard could include:
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

## Dashboard
 [Dashboard link](https://github.com/SERIEMEN/bank-analysis-dashboard/blob/main/power%20BI%20practice1.pbix)

## CONCLUSION 
1. The analysis provides a consolidated view of the bank's customer base, account balances, transaction activity, loan exposure, and         branch performance.
2. The strongest opportunities identified are improving transaction reliability, strengthening credit-risk management, leveraging multi-     account customers, and developing more comprehensive branch-performance metrics.
3. Calabar stands out for customer and account activity, while the loan analysis highlights a significant level of default exposure that     requires attention.
4. Overall, the project demonstrates how Power BI can transform raw banking data into an interactive decision-support tool that enables      management to move from simply viewing data to identifying patterns, risks, opportunities, and areas requiring action.
