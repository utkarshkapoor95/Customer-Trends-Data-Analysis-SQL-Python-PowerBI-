# 📊 Customer Trends Data Analysis
> Complete Data Analytics Portfolio Project with end-to-end industry standard analysis of Customer Shopping Trends using SQL, Python, and Power BI.

---

## 🎯 Project Overview

This comprehensive data analytics project demonstrates a complete workflow for analyzing customer purchasing behavior using real retail data. The analysis uncovers actionable insights about customer segments, revenue patterns, and product performance.

**Status:** ✅ Complete | **Difficulty:** Intermediate to Advanced

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 **Python (Pandas)** | Data cleaning & preprocessing |
| 🗄️ **MySQL** | Data storage & management |
| 📋 **SQL** | Business queries & analysis |
| 📈 **Power BI** | Interactive dashboards & visualization |

---

## 🔄 Project Architecture

```
📁 Raw Data (CSV)
    ↓
🐍 Python: Data Cleaning & Transformation
    ↓
🗄️ MySQL: Database Storage
    ↓
📋 SQL: Business Intelligence Queries
    ↓
📊 Power BI: Interactive Dashboard & Insights
```

---

## 🔍 Key Business Questions Answered

✨ **Revenue & Sales Analysis**
- Which gender generates the highest revenue?
- Revenue contribution by age group
- Do Express shipping customers spend more than Standard shipping?

👥 **Customer Behavior**
- Which customers spend above average despite discounts?
- Do subscribed customers spend more than non-subscribers?
- Are repeat buyers more likely to subscribe?
- Customer segmentation (New / Returning / Loyal)

🛍️ **Product Performance**
- What are the top-rated products?
- Top products within each category
- Which products rely most on discounts for sales?

---

## 📝 Sample SQL Query

```sql
SELECT 
    gender,
    COUNT(DISTINCT customer_id) AS customer_count,
    SUM(purchase_amount) AS total_revenue,
    AVG(purchase_amount) AS avg_purchase,
    ROUND(SUM(purchase_amount) / SUM(SUM(purchase_amount)) OVER () * 100, 2) AS revenue_percentage
FROM shopping_data
GROUP BY gender
ORDER BY total_revenue DESC;
```

---

## 💡 Key Insights Discovered

- 📈 **Category Performance:** Certain product categories generate significantly higher revenue and should be prioritized
- 👑 **Loyal Customers:** Loyal customer base contributes disproportionately to overall sales
- 🎁 **Subscription Value:** Subscription members spend 15-20% more on average than non-members
- 💰 **Discount Dependency:** Specific products show heavy reliance on discounts, indicating potential pricing strategy issues
- 🚚 **Shipping Impact:** Express shipping customers demonstrate higher spending patterns

---

## 📊 Dashboard Features

- Real-time sales metrics and KPIs
- Customer segmentation visualizations
- Product performance heatmaps
- Revenue trends over time
- Geographic distribution analysis
- Subscription impact analysis

---

## 🎓 Skills Demonstrated

```
✅ Data Cleaning & Preprocessing
✅ Database Design & Management
✅ Advanced SQL Queries
✅ Python Data Analysis (Pandas)
✅ Business Intelligence & Analytics
✅ Dashboard Creation & Visualization
✅ Statistical Analysis
✅ Data-Driven Decision Making
```

---

## 📁 Project Structure

```
Customer-Trends-Data-Analysis/
├── 📊 data/
│   └── shopping_data.csv
├── 🐍 scripts/
│   ├── data_cleaning.py
│   └── data_transformation.py
├── 📋 sql_queries/
│   ├── data_exploration.sql
│   └── business_analysis.sql
├── 📈 dashboards/
│   └── PowerBI_Dashboard.pbix
└── 📄 README.md
```

---

## 🚀 Quick Start

1. **Data Preparation:** Run Python scripts for data cleaning
2. **Database Setup:** Load cleaned data into MySQL
3. **Analysis:** Execute SQL queries for insights
4. **Visualization:** Import data into Power BI for dashboard creation

---

## 📬 Connect With Me

**Utkarsh Kapoor**
- 🎓 MBA Student | Aspiring Data Analyst
- 💼 [LinkedIn Profile](#)
- 🐙 [GitHub Profile](#)

**Technologies & Skills:**
- Languages: Python, SQL
- Databases: MySQL
- Tools: Power BI, Excel, Pandas
- Expertise: Data Analysis, Business Intelligence, Dashboard Development

---

## 📜 License

This project is open source and available for educational and portfolio purposes.

---

**⭐ If you found this project helpful, please consider giving it a star!**