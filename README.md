📊 Customer Shopping Behavior Analysis

An end-to-end data analytics project that explores customer shopping behavior using Python, SQL (MySQL), and Power BI.
The goal is to derive insights into spending patterns, customer segments, subscription trends, and product performance to support data-driven business decisions.

📁 Project Overview

This project analyzes 3,900 purchase transactions across multiple product categories.
It includes:

1. Python-based data cleaning & feature engineering
2. SQL-based business analysis using PostgreSQL
3. Interactive Power BI dashboard
4. Actionable business recommendations

🧰 Technologies Used

1. Python (Pandas, NumPy)	Data cleaning, preprocessing, feature engineering
2. MySQL	Business analysis using SQL queries
3. Power BI	Dashboard & data visualization
4. Jupyter Notebook	EDA documentation

📊 Dataset Summary

1. Rows: 3,900
2. Columns: 18
3. Key Features:

  1. Age, Gender, Location
  2. Item purchased, Category, Purchase amount
  3. Discount applied, Promo code usage
  4. Subscription status
  5. Previous purchase history
  6. Review ratings
  7. Shipping type

4. Missing Values:

  1. 37 missing values in Review Rating, handled via category-wise median imputation

🧹 1. Data Cleaning & Feature Engineering (Python)

Key steps:

  1. Loaded dataset with Pandas and explored structure
  2. Handled missing ratings using median per product category
  3. Standardized column names to snake_case
  4. Created new features:
    age_group (binned ages)
    purchase_frequency_days
  5. Checked redundancy between discount_applied and promo_code_used
  6. Loaded cleaned dataset into PostgreSQL for advanced analysis

🧮 2. SQL Analysis (PostgreSQL)

Used SQL to answer real business questions:

  1. Revenue comparison by gender
  2. Highest-spending customers using discounts
  3. Top 5 products by average review rating
  4. Standard vs. express shipping behavior
  5. Subscribers vs non-subscribers revenue
  6. Products most dependent on discounts
  7. Customer segmentation:
    New
    Returning
    Loyal
  8. Top 3 products in each category
  9. Repeat buyers & subscription correlation
  10. Revenue contribution by age groups
      
SQL scripts are included in the /sql/ folder.

📈 3. Power BI Dashboard

  1. The dashboard highlights:
  2. Total revenue & KPIs
  3. Customer segments
  4. Category performance
  5. Discount usage impact
  6. Age group & gender insights
  7. Shipping type comparison
  8. Product ratings overview

A .pbix file is included in the repository.

💡 Business Insights & Recommendations

  1. Boost subscription programs with exclusive benefits
  2. Reward loyal customers to improve retention
  3. Optimize discount strategy for margin control
  4. Promote top-rated products in campaigns
  5. Target high-value age groups
  6. Encourage express shipping users through incentives

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

4️⃣ Load Data into MySQL
Use the SQL scripts in the /sql/ folder.

5️⃣ Open Power BI Dashboard
Open the .pbix file from the /dashboard/ folder.

🧑‍💻 Author

Sunil Biriya
Data Analyst | SQL | Power BI | Python
