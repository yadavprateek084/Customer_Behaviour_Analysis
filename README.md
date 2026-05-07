# 🛍️ Customer Behaviour Analysis Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge&logo=powerbi)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-SQL-blue?style=for-the-badge&logo=postgresql)
![Python](https://img.shields.io/badge/Python-Analysis-green?style=for-the-badge&logo=python)

---

# 📌 Project Overview

An end-to-end **Customer Behaviour Analysis Project** built using **SQL, Python, and Power BI** to analyze customer purchasing patterns, revenue trends, subscriptions, demographics, and product performance.

This project converts raw customer shopping data into actionable business insights through interactive dashboards and advanced SQL analysis.

---

# 🚀 Objectives

- Analyze customer purchase behavior
- Track revenue by category
- Study subscription impact
- Understand customer demographics
- Build an interactive Power BI dashboard
- Perform advanced SQL analytics

---

# 🛠️ Tech Stack

| Tool | Usage |
|---|---|
| PostgreSQL | Database & SQL Queries |
| Python (Pandas) | Data Cleaning |
| Power BI | Dashboard Visualization |

---

# 📂 Project Structure

```bash
Customer_Behaviour_Analysis/
│
├── Dataset/
├── SQL/
├── PowerBI/
├── Python/
├── Images/
└── README.md
```

---

# 📊 Dashboard Preview

<img width="100%" alt="Dashboard" src="https://github.com/yourusername/Customer_Behaviour_Analysis/assets/dashboard.png">

---

# 📈 Dashboard Features

## KPI Cards
- Total Customers
- Average Purchase Amount
- Average Review Rating

## Interactive Filters
- Gender
- Subscription Status
- Product Category
- Shipping Type

## Visualizations
- Revenue by Category
- Customer by Category
- Purchase by Age Group
- Subscription Analysis

---

# 🧠 Advanced SQL Queries

## 1️⃣ Top Products Purchased with Discounts

```sql
SELECT
    item_purchased,
    COUNT(customer_id) AS total_customers,
    DENSE_RANK() OVER(
        ORDER BY COUNT(customer_id) DESC
    ) AS ranking
FROM customer
WHERE discount_applied = 'Yes'
GROUP BY item_purchased
LIMIT 5;
```

---

## 2️⃣ Revenue by Category

```sql
SELECT
    category,
    SUM(purchase_amount) AS total_revenue
FROM customer
GROUP BY category
ORDER BY total_revenue DESC;
```

---

## 3️⃣ High Spending Customers

```sql
SELECT
    customer_id,
    purchase_amount
FROM customer
WHERE purchase_amount >
(
    SELECT AVG(purchase_amount)
    FROM customer
);
```

---

## 4️⃣ Customer Ranking by Purchase Amount

```sql
SELECT
    customer_id,
    purchase_amount,
    DENSE_RANK() OVER(
        ORDER BY purchase_amount DESC
    ) AS customer_rank
FROM customer;
```

---

## 5️⃣ Age Group Analysis

```sql
SELECT
    CASE
        WHEN age BETWEEN 18 AND 25 THEN 'Young Adult'
        WHEN age BETWEEN 26 AND 40 THEN 'Adult'
        WHEN age BETWEEN 41 AND 55 THEN 'Middle Aged'
        ELSE 'Senior'
    END AS age_group,
    COUNT(*) AS total_customers
FROM customer
GROUP BY age_group;
```

---

# 🐍 Python Operations

```python
✔ Data Cleaning
✔ Handling Missing Values
✔ Data Transformation
✔ Feature Engineering
✔ Exploratory Data Analysis
```

---

# 📊 Power BI Concepts Used

- DAX Measures
- KPI Cards
- Interactive Slicers
- Data Modeling
- Dashboard Design

---

<img width="843" height="502" alt="Screenshot 2026-05-07 221634" src="https://github.com/user-attachments/assets/7d73f9b8-24f9-4c7c-ac65-f9da089311de" />


# 🔍 Key Insights

- Clothing category generated highest revenue
- Young adults were the most active buyers
- Subscribed customers spent more on average
- Free shipping was the most preferred option
- Customer review ratings remained consistently high

---

# 🎯 Project Outcome

This project demonstrates how customer transaction data can be transformed into meaningful business insights using SQL, Python, and Power BI.

---

# 👨‍💻 Author

## Prateek Yadav
