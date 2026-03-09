# Customer-Trends-Data-Analysis-SQL-Python-PowerBI-
Complete Data Analytics Portfolio Project with end-to-end industry standard Data Analysis of Customer Shopping Trends from Retail Data using SQL, Python and Power BI.

Customer Shopping Behavior Analysis
Overview

This project analyzes customer purchasing behavior using a retail dataset.
The analysis focuses on identifying revenue patterns, customer segments, product performance, and purchasing trends.

The project demonstrates an end-to-end data analytics workflow using Python, SQL, and Power BI.

Tools Used

Python (Pandas) – Data cleaning and preprocessing

MySQL – Data storage and SQL analysis

SQL – Business queries and insights

Power BI – Data visualization and dashboard

Project Workflow
Dataset (CSV)
     ↓
Python Data Cleaning
     ↓
MySQL Database
     ↓
SQL Business Analysis
     ↓
Power BI Dashboard
Key Business Questions

The analysis answers questions such as:

Which gender generates the highest revenue?

Which customers spend above the average even with discounts?

What are the top-rated products?

Do Express shipping customers spend more than Standard shipping?

Do subscribed customers spend more?

Which products rely most on discounts?

Customer segmentation (New / Returning / Loyal)

Top products within each category

Are repeat buyers more likely to subscribe?

Revenue contribution by age group

Example SQL Query
SELECT gender, SUM(purchase_amount) AS revenue
FROM shopping_data
GROUP BY gender;
Key Insights

Certain product categories generate the highest revenue.

Loyal customers contribute significantly to overall sales.

Subscription members tend to spend more on average.

Some products depend heavily on discounts for purchases.

Author

Utkarsh Kapoor
MBA Student | Aspiring Data Analyst

Skills demonstrated:

Python | SQL | MySQL | Power BI | Data Analysis
