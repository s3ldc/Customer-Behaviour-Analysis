📊 Customer Shopping Behavior Analysis

An end-to-end data analytics project that explores customer shopping behavior using Python, SQL (PostgreSQL), and Power BI.
The goal is to derive insights into spending patterns, customer segments, subscription trends, and product performance to support data-driven business decisions.

📁 Project Overview

This project analyzes 3,900 purchase transactions across multiple product categories.
It includes:

Python-based data cleaning & feature engineering

SQL-based business analysis using PostgreSQL

Interactive Power BI dashboard

Actionable business recommendations

🧰 Technologies Used
Tool	Purpose
Python (Pandas, NumPy)	Data cleaning, preprocessing, feature engineering
PostgreSQL	Business analysis using SQL queries
Power BI	Dashboard & data visualization
Matplotlib / Seaborn	Exploratory data analysis plots
Jupyter Notebook	EDA documentation
📊 Dataset Summary

Rows: 3,900

Columns: 18

Key Features:

Age, Gender, Location

Item purchased, Category, Purchase amount

Discount applied, Promo code usage

Subscription status

Previous purchase history

Review ratings

Shipping type

Missing Values:

37 missing values in Review Rating, handled via category-wise median imputation

🧹 1. Data Cleaning & Feature Engineering (Python)

Key steps:

Loaded dataset with Pandas and explored structure

Handled missing ratings using median per product category

Standardized column names to snake_case

Created new features:

age_group (binned ages)

purchase_frequency_days

Checked redundancy between discount_applied and promo_code_used

Loaded cleaned dataset into PostgreSQL for advanced analysis

🧮 2. SQL Analysis (PostgreSQL)

Used SQL to answer real business questions:

Revenue comparison by gender

Highest-spending customers using discounts

Top 5 products by average review rating

Standard vs. express shipping behavior

Subscribers vs non-subscribers revenue

Products most dependent on discounts

Customer segmentation:

New

Returning

Loyal

Top 3 products in each category

Repeat buyers & subscription correlation

Revenue contribution by age groups

SQL scripts are included in the /sql/ folder.

📈 3. Power BI Dashboard

The dashboard highlights:

Total revenue & KPIs

Customer segments

Category performance

Discount usage impact

Age group & gender insights

Shipping type comparison

Product ratings overview

A .pbix file is included in the repository.

💡 Business Insights & Recommendations

Boost subscription programs with exclusive benefits

Reward loyal customers to improve retention

Optimize discount strategy for margin control

Promote top-rated products in campaigns

Target high-value age groups

Encourage express shipping users through incentives

📂 Project Structure
📦 Customer-Shopping-Behavior-Analysis
│
├── data/
│   └── customer_shopping_data.csv
│
├── notebooks/
│   └── EDA.ipynb
│
├── sql/
│   └── business_queries.sql
│
├── dashboard/
│   └── shopping_behavior_dashboard.pbix
│
├── images/
│   └── dashboard_screenshots.png
│
└── README.md

🚀 How to Run the Project
1️⃣ Clone the Repo
git clone https://github.com/s3ldc/Customer-Behaviour-Analysis.git

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run the Jupyter Notebook
jupyter notebook

4️⃣ Load Data into PostgreSQL

Use the SQL scripts in the /sql/ folder.

5️⃣ Open Power BI Dashboard

Open the .pbix file from the /dashboard/ folder.

🧑‍💻 Author

Sunil Biriya
Data Analyst | SQL | Power BI | Python
