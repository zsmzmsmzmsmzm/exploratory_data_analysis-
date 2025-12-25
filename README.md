# exploratory_data_analysis-
Exploratory Data Analysis (EDA) using SQL
🔍 Project Overview

This project performs Exploratory Data Analysis (EDA) on a sales data warehouse using SQL.
The goal is to understand the data structure, explore relationships between tables, and extract meaningful business insights related to sales performance and products.

🗂 Database Context

Database: DataWarehouseAnalytics

Schema style: Fact & Dimension tables

Main Tables Used

fact_sales

dim_products

(other related dimension tables)

🎯 Analysis Objectives

Explore available tables and data structure

Understand sales distribution across products

Analyze total sales performance

Identify top-performing products

Validate data consistency using joins

🛠 Tools & Techniques

SQL

Joins (Fact ↔ Dimension)

Aggregate Functions (SUM, COUNT)

Grouping & Sorting

Basic EDA best practices

📈 Key Analysis Performed

Overview of all database objects

Total sales by product

Product-level performance analysis

Data relationship validation using primary & foreign keys

Aggregated metrics for business understanding

Example query logic:

SELECT 
    p.product_name,
    SUM(f.sales_amount) AS total_sales
FROM fact_sales f
JOIN dim_products p
    ON p.product_key = f.product_key
GROUP BY p.product_name;

🧠 Insights

Sales are not evenly distributed across products

A small number of products generate the majority of revenue

Fact and dimension tables are well-structured for analytical queries

The data model supports scalable analysis

📁 Repository Structure
├── exploratory_analysis.sql
├── README.md

🚀 How to Run

Restore or connect to the DataWarehouseAnalytics database

Open the SQL script

Run queries step by step to explore results

🧩 Skills Demonstrated

Exploratory Data Analysis (EDA)

Data Warehousing Concepts

SQL Analytics

Business-Oriented Thinking

Query Structuring & Readability

👤 Author

Mohamed Asaad Elsayed 
Junior Data Analyst
🔗 LinkedIn: (https://www.linkedin.com/in/mohamed-asaad-159baa290/)

🔖 Tags

SQL EDA Data Analysis Data Warehouse Analytics
