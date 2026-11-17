# Credit-card-financial-analytics 

## Project Overview

This project focuses on analyzing credit card transactions, customer demographics, and financial performance using PostgreSQL, SQL, and Power BI.

The objective is to transform raw customer and transaction data into meaningful business insights. The dashboards provide an overview of revenue, transaction activity, customer characteristics, card categories, and spending patterns.

The project consists of two Power BI reports: a **Credit Card Customer Report** and a **Credit Card Transaction Report**.

## Business Objectives

- Monitor overall credit card revenue and transaction performance.
- Understand customer demographics and spending behaviour.
- Compare financial performance across different card categories.
- Analyze revenue by expenditure type and customer occupation.
- Evaluate quarterly revenue and transaction trends.
- Examine customer income, satisfaction, and credit utilization.
- Identify patterns that support business decision-making.

## Tools & Technologies

- **Power BI:** Dashboard development, data visualization, and business reporting.
- **PostgreSQL:** Database creation, table management, and data handling.
- **SQL:** Database operations and analytical data preparation.
- **CSV:** Source data storage and management.

## Repository Structure

```text
credit-card-financial-analytics/
│
├── data/
│   ├── credit_card.csv
│   ├── customer.csv
│   └── cust_add.csv
│
├── sql/
│   └── creditcard_dashboard.sql
│
├── reports/
│   ├── customer_dashboard.pdf
│   └── transaction_dashboard.pdf
│
├── screenshots/
│   ├── customer_dashboard.png
│   └── transaction_dashboard.png
│
├── Credit_Card_Financial_Dashboard.pbix
│
├── .gitignore
│
└── README.md
```

## Dataset Description

The project uses three CSV datasets:

| Dataset | Description |
|---|---|
| `credit_card.csv` | Credit card transactions, card categories, annual fees, credit limits, transaction amounts, and interest earned. |
| `customer.csv` | Customer demographics, income, education, employment, marital status, and satisfaction scores. |
| `cust_add.csv` | Additional customer records containing customer demographic and profile information. |

The customer datasets can be combined using `Client_Num` as the customer identifier.

## Data Preparation

The datasets were inspected and prepared for analysis.

The preparation process includes:

1. Reviewing dataset structures and column names.
2. Checking missing values and duplicate records.
3. Standardizing column names and data types.
4. Combining the main and additional customer datasets.
5. Preparing customer and transaction data for analysis.
6. Connecting customer and transaction information through `Client_Num`.

## SQL & Database

PostgreSQL is used for database management and SQL-based data handling.

The project includes two database tables:

- **cc_detail:** Stores credit card transaction and financial information.
- **cust_detail:** Stores customer demographic and profile information.

The two tables are related through the `Client_Num` field.

## Power BI Dashboards

The project contains two reports designed to provide different perspectives on credit card financial performance.

### 1. Credit Card Customer Report

This dashboard focuses on customer demographics, income, and financial contributions.

**Key metrics and analysis:**

- Total Revenue
- Total Income
- Total Interest
- Customer Satisfaction Score
- Revenue by Gender
- Revenue by Customer Job
- Revenue by Education Level
- Revenue by Marital Status
- Revenue by Age Group
- Revenue by State
- Revenue by Salary Group
- Revenue by Dependent Count

![Credit Card Customer Dashboard](screenshots/customer_dashboard.png)

[View Customer Dashboard (PDF)](reports/customer_dashboard.pdf)

### 2. Credit Card Transaction Report

This dashboard focuses on transaction performance, card categories, and customer spending patterns.

**Key metrics and analysis:**

- Total Revenue
- Transaction Count
- Transaction Amount
- Total Interest
- Revenue by Expenditure Type
- Revenue by Card Category
- Revenue by Customer Job
- Revenue by Transaction Method
- Quarterly Revenue and Transaction Count
- Customer Acquisition Cost by Card Category

![Credit Card Transaction Dashboard](screenshots/transaction_dashboard.png)

[View Transaction Dashboard (PDF)](reports/transaction_dashboard.pdf)

## Key Business Metrics

The following metrics are displayed in the Power BI reports:

| Metric | Reported Value |
|---|---:|
| Total Revenue | 55.4M |
| Transaction Count | 657K |
| Transaction Amount | 45M |
| Total Interest | 7.9M |
| Total Income | 577M |
| Customer Satisfaction Score | 3.19 |

*Values are taken from the dashboard reports and retain their original units and formatting.*

## Key Business Insights

The dashboards provide insights into:

- Revenue contribution across different credit card categories.
- Customer spending patterns across expenditure categories.
- Revenue distribution across customer occupations and income groups.
- Quarterly changes in revenue and transaction activity.
- Customer demographics and their relationship with financial performance.
- Transaction preferences across chip, swipe, and online payment methods.

## How to Use This Project

1. Clone or download this repository.
2. Navigate to the `data` folder to access the datasets.
3. Create a PostgreSQL database.
4. Execute the SQL scripts in the `sql` folder after configuring the data import paths.
5. Load the datasets into Power BI Desktop.
6. Open the `.pbix` file to explore the interactive dashboards.
7. Use the available filters to analyze customer segments, card categories, quarters, and other business dimensions.

## Skills Demonstrated

- Data Analysis
- SQL
- PostgreSQL
- Data Preparation
- Data Modeling
- Power BI
- Dashboard Development
- Business Intelligence
- Data Visualization
- Financial Analytics
- Customer Analytics

Author: 
Rabiya Khatun
