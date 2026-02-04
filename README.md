**🏦 Banana Bank – Unstructured Banking Data Analytics Project**

A complete end-to-end banking analytics project built on a large unstructured transactional dataset to identify fraud exposure, operational risks, customer churn signals and abnormal behaviour patterns.

This project simulates how real banking analytics teams clean messy production data and convert it into actionable business insights.

📌 Project Overview

Project Name: Banana Bank – Banking Risk & Operations Analytics
Dataset Size: 100,000 transactions
Columns: 18
Data Type: Synthetic but intentionally unstructured (messy & inconsistent)

The project focuses on:

fraud risk exposure

operational performance

customer experience & churn risk

KYC compliance impact

abnormal customer behaviour detection

🎯 Business Objective

To help Banana Bank identify:

hidden fraud leakages

unreliable transaction channels

high-risk merchants and devices

customers likely to churn

abnormal customer behaviour patterns

and support data-driven decisions for:

risk teams

compliance teams

operations and IT teams

customer retention teams

📂 Dataset Description

The dataset contains unstructured and inconsistent fields such as:

mixed date formats

mixed categorical labels (gender, KYC, device)

missing values

mixed fraud risk representations

negative balances

incomplete KYC information

Main columns used in analysis

transaction_id

customer_id

age

gender

city

account_type

account_balance

transaction_amount

transaction_type

channel

device

ip_address

merchant

transaction_time

transaction_status

kyc_completed

fraud_risk_score

remarks

🧹 Data Preparation & Quality Checks

Before any analysis, the following preprocessing steps were performed:

standardised city, gender and KYC fields

converted mixed fraud risk values into numeric scores

parsed mixed date formats into unified timestamps

converted age and balance fields into numeric values

removed invalid and missing categorical values

created derived features such as:

transaction hour

transaction date

risk and failure flags

This ensures that business KPIs are computed on clean and reliable data.

🔍 Business Problems Solved

The following real-world banking problems were analysed.

1️⃣ Which transactions have high fraud risk but still succeeded?

Identifies transactions with fraud risk score ≥ 0.8 that were still approved, representing direct fraud exposure and rule-engine gaps.

2️⃣ Which customers are generating repeated failed transactions?

Detects customers facing repeated failures, indicating poor customer experience and high churn risk.

3️⃣ Which cities contribute the highest transaction value but also the highest failure rate?

Identifies operational risk hotspots where high business volume coincides with unreliable transaction processing.

4️⃣ Is digital channel (Mobile App / Web) really performing better than Branch & ATM?

Compares digital and physical channels using success rate and failure rate to support digital investment decisions.

5️⃣ Which merchants are most associated with suspicious or high-risk transactions?

Ranks merchants based on the proportion of suspicious transactions to support merchant monitoring and compliance reviews.

6️⃣ Are KYC-incomplete customers more risky than KYC-completed customers?

Evaluates fraud and failure behaviour across KYC status to assess onboarding and regulatory risk.

7️⃣ Which devices and platforms show higher fraud risk and failure rate?

Identifies risky platforms and devices requiring application security and monitoring enhancements.

8️⃣ Which customer segments have negative balances and high transaction activity?

Segments customers by:

Age group + Account type

to identify segments with high overdraft and credit exposure.

9️⃣ Do certain transaction types (UPI, ATM, Card, IMPS, NEFT) create more failures or disputes?

Evaluates transaction rails based on failure rate and operational dispute load.

🔟 Which customers show abnormal transaction behaviour patterns?

Uses multi-signal behavioural indicators such as:

unusually high transaction volume

activity across many cities

multiple devices

frequent high-risk transactions

to identify abnormal customers for monitoring and investigation.

🧠 Methodology

The project follows a professional analytics workflow:

Raw data
→ data cleaning & standardisation
→ data validation
→ feature engineering
→ KPI construction
→ business-driven analysis
→ visualization
→ investigation-ready outputs

Robust, percentile-based thresholds were used instead of fixed hard-coded limits for abnormal behaviour detection.

📊 Visualisation

All visualisations were created using:

Matplotlib

Seaborn

Charts include:

success and failure rate comparisons

merchant and channel risk distributions

customer segment risk views

abnormal behaviour score distributions

All plots use consistent colour palettes for professional presentation.

🛠️ Tools & Technologies

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

📁 Recommended Project Structure

Banana-Bank-Analytics/
│
├── data/
│   ├── Banana_Bank_Unstructured_Dataset_100k.csv
│   └── Banana_Bank_Cleaned_Dataset.csv
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_business_questions_analysis.ipynb
│
├── outputs/
│   └── charts/
│
└── README.md

⚠️ Disclaimer

This dataset is synthetically generated for educational and portfolio purposes.
It does not contain any real customer or financial data.

👤 Author

Saurav Chauhan

Data Analytics & Business Intelligence Enthusiast

⭐ Key Takeaway

This project demonstrates how unstructured banking data can be transformed into operational, fraud-risk and customer-experience insights using professional analytics workflows suitable for real financial institutions.
