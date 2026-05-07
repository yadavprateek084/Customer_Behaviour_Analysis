<div align="center">

# 🚀 Customer Behaviour Analysis  
### End-to-End Data Analyst Project

<img src="https://img.shields.io/badge/Role-Data_Analyst-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/SQL-Advanced-success?style=for-the-badge&logo=postgresql">
<img src="https://img.shields.io/badge/Python-Pandas-yellow?style=for-the-badge&logo=python">
<img src="https://img.shields.io/badge/Power_BI-Dashboard-orange?style=for-the-badge&logo=powerbi">
<img src="https://img.shields.io/badge/Project-End_to_End-red?style=for-the-badge">

### 📊 Transforming Raw Customer Data into Business Insights

</div>

---

# 📌 Project Summary

This project is a complete **End-to-End Data Analytics Solution** developed to analyze customer purchasing behavior, spending patterns, subscription impact, customer demographics, and category-wise business performance.

The project follows the complete workflow of a real-world **Data Analyst role**:

### ✔ Data Collection  
### ✔ Data Cleaning  
### ✔ Data Transformation  
### ✔ SQL Analysis  
### ✔ Business Insights Generation  
### ✔ Dashboard Development  
### ✔ Data Visualization  

---

# 🎯 Business Objective

Businesses often struggle to understand:

- Which customers generate the highest revenue
- Which categories perform best
- How subscriptions affect purchases
- Customer buying patterns
- Revenue trends across demographics

This dashboard helps stakeholders make data-driven business decisions through interactive analytics and visualization.

---

# 🛠️ Tools & Technologies Used

| Technology | Purpose |
|---|---|
| PostgreSQL | Database Management |
| SQL | Data Analysis & Querying |
| Python (Pandas) | Data Cleaning & Processing |
| Power BI | Interactive Dashboard |
| Excel/CSV | Dataset Source |

---

# 🔄 End-to-End Workflow

## 📥 1. Data Collection
- Imported customer shopping dataset
- Structured raw transactional data

## 🧹 2. Data Cleaning using Python
Performed:
- Missing value handling
- Duplicate removal
- Data formatting
- Feature engineering
- Data preprocessing

## 🗄️ 3. SQL Data Analysis
Used advanced SQL techniques:
- Window Functions
- Aggregate Functions
- Ranking Functions
- Subqueries
- CASE Statements
- Grouping & Filtering

## 📊 4. Dashboard Development
Built an interactive Power BI dashboard with:
- KPI Cards
- Dynamic Charts
- Slicers & Filters
- Business Visualizations

## 📈 5. Business Insight Generation
Generated actionable insights for business decision-making.

---

# 📊 Dashboard Preview

<div align="center">

<img width="843" height="502" alt="Screenshot 2026-05-07 221634" src="https://github.com/user-attachments/assets/0feac134-0e2e-43a1-b2d0-c1aed4899762" />


</div>

---

# 🔥 Dashboard Features

### 📌 KPI Metrics
- Total Customers
- Average Purchase Amount
- Average Review Rating

### 📌 Interactive Filters
- Gender
- Subscription Status
- Product Category
- Shipping Type

### 📌 Visual Analysis
- Revenue by Category
- Customers by Category
- Purchase by Age Group
- Subscription Distribution
- Customer Segmentation

---

# 🧠 Advanced SQL Queries Used

## 🏆 Top Products Purchased with Discounts

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

## 💰 Revenue Analysis by Category

```sql
SELECT
    category,
    SUM(purchase_amount) AS total_revenue
FROM customer
GROUP BY category
ORDER BY total_revenue DESC;
```

---

## 👑 High Spending Customers

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

## 📈 Customer Ranking using Window Functions

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

## 👥 Customer Age Group Analysis

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

# 🐍 Python Skills Demonstrated

```python
✔ Pandas
✔ Data Cleaning
✔ Handling Missing Values
✔ Data Transformation
✔ Feature Engineering
✔ Exploratory Data Analysis
```

---

# 📊 Power BI Skills Demonstrated

- Data Modeling
- DAX Measures
- Interactive Slicers
- KPI Cards
- Dashboard Designing
- Business Storytelling
- Visual Analytics

---

# 🔍 Key Business Insights

✅ Clothing category generated highest revenue  

✅ Young adults were the most active buyers  

✅ Subscription customers spent more on average  

✅ Free shipping was the most preferred shipping option  

✅ Customer review ratings showed strong customer satisfaction  

---

# 📈 Project Outcome

Successfully transformed raw customer transaction data into an interactive business intelligence dashboard capable of generating meaningful insights for strategic decision-making.

This project highlights:
- Real-world Data Analytics workflow
- Strong SQL problem-solving
- Dashboard development skills
- Business understanding
- Data storytelling ability

---

# 👨‍💻 Author

## Prateek Yadav


<div align="center">

# ⭐ Star this repository if you found it useful!

</div>
