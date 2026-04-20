# Customer Trends Data Analysis
> End-to-end data analytics project: 3,900 customer transactions analyzed using Python, MySQL, SQL, and Power BI.

---

## Project Overview

Analyzes real retail shopping data to uncover actionable patterns in customer spending, product performance, and loyalty behavior. Full pipeline: raw CSV → Python cleaning → MySQL storage → SQL analysis → Power BI dashboard.

**Status:** ✅ Complete | **Stack:** Python · MySQL · SQL · Power BI

---

## Tech Stack

| Tool | Purpose |
|---|---|
| 🐍 **Python (Pandas)** | Data cleaning & feature engineering |
| 🗄️ **MySQL + SQLAlchemy** | Database storage & management |
| 📋 **SQL** | Business intelligence queries (CTEs, window functions) |
| 📈 **Power BI** | Interactive dashboards & KPI cards |

---

## Project Architecture

```
Raw CSV (3,900 records, 18 columns)
    ↓
Python: Cleaning + Feature Engineering (age_group, purchase_frequency_days)
    ↓
MySQL: shopping_data table (customer_behavior DB)
    ↓
SQL: 10 Business Intelligence Queries
    ↓
Power BI: Interactive Dashboard
```

---

## Key Business Questions Answered

**Revenue & Sales**
- Which gender generates the highest revenue?
- Revenue contribution by age group
- Do Express shipping customers spend more than Standard?

**Customer Behavior**
- Which customers spend above average despite using discounts?
- Do subscribed customers spend more than non-subscribers?
- Are repeat buyers (5+ purchases) more likely to subscribe?
- Customer segmentation: New / Returning / Loyal

**Product Performance**
- Top 5 products by average review rating
- Top 3 products within each category (window function)
- Which products are most discount-dependent?

---

## Key Insights (from the data)

- **Gender Split:** 2,652 male (68%) vs 1,248 female (32%) customers by transaction volume
- **Subscription Premium:** Subscribed customers spend 15–20% more on average
- **Loyal Customer Value:** Customers with 10+ previous purchases drive disproportionate revenue
- **Discount Dependency:** Several products show 40%+ of sales requiring discounts — a margin risk signal
- **Shipping Insight:** Express shipping customers demonstrate higher average purchase amounts than Standard

---

## SQL Highlights

10 business-driven queries including:
- `ROW_NUMBER() OVER (PARTITION BY category)` for category rankings
- CTEs for multi-step customer segmentation logic
- Correlated subqueries for above-average discount user identification
- Age group revenue contribution using engineered `age_group` column

See [`mysql_customer_behavior_queries.sql`](mysql_customer_behavior_queries.sql) for all queries with explanation comments.

---

## Files

| File | Description |
|---|---|
| `Customer_Shopping_Behavior.csv` | Raw dataset (3,900 records, 18 columns) |
| `customer_behavior_analysis.ipynb` | Python: cleaning, feature engineering, MySQL load |
| `mysql_customer_behavior_queries.sql` | 10 SQL business intelligence queries |
| `customer_behavior_dashboard.pbix` | Power BI interactive dashboard |
| `Customer Shopping Behavior Analysis.pdf` | Full analysis report |
| `Customer-Shopping-Behavior-Analysis.pptx` | Business presentation deck |
| `Business Problem Document.pdf` | Problem framing & objectives |

---

## Quick Start

```bash
# 1. Install dependencies
pip install pandas sqlalchemy pymysql python-dotenv

# 2. Configure MySQL credentials
cp .env.example .env
# Edit .env → set MYSQL_USER and MYSQL_PASSWORD

# 3. Run the notebook (clean data + load to MySQL)
jupyter notebook customer_behavior_analysis.ipynb

# 4. Run SQL queries in MySQL Workbench
# Open: mysql_customer_behavior_queries.sql

# 5. Open Power BI dashboard
# Open: customer_behavior_dashboard.pbix
```

---

## Connect

**Utkarsh Kapoor** — MBA | Operations → Data Analytics & AI

- [LinkedIn](https://linkedin.com/in/utkarsh-kapoor-618256203)
- [GitHub](https://github.com/utkarshkapoor95)

---

*Open source — available for educational and portfolio use.*
