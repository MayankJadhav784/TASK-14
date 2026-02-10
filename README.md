# TASK-14
INTERNSHIP DAY 14

# Task 14: ETL Mini Pipeline

 Overview
This project demonstrates a mini ETL (Extract - Transform - Load) pipeline using Python and Pandas.  
Dataset used: Customer Churn Dataset (CSV uploaded in Google Colab).

The goal is to practice how ETL works in analytics workflows by cleaning raw data, transforming it into structured tables, and loading outputs into CSV and SQLite.

 Steps

 1. Extract
- Loaded raw dataset ('customer_churn.csv') from Kaggle into Google Colab.
- Created folder structure:  
  - 'raw/' → original dataset  
  - 'processed/' → cleaned CSV outputs  
  - 'output/' → SQLite database  

2. Transform
- Removed duplicates and handled missing values.
- Standardized column names (lowercase, underscores).
- Converted datatypes (e.g., tenure → int, monthly charges → float).
- Created derived columns:
  - 'churn_flag' (binary indicator for churn).
  - 'total_charges_calc' (calculated spend based on tenure × monthly charges).

 3. Split
Separated dataset into logical tables:
- Customers → demographics + churn info  
- Services → subscription details + usage metrics  
- Billing → financial + interaction history  

 4. Load
- Exported processed tables into CSV files:
  - 'customers.csv'
  -'services.csv'
  - 'billing.csv'
- Loaded all tables into a SQLite database ('database.sqlite').

5. Validate
- Verified row counts before and after transformations.
- Checked schema consistency across CSVs and SQLite tables.




