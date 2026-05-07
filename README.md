# 🛍️ Customer Behaviour Analysis Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge&logo=powerbi)
![SQL](https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge&logo=postgresql)
![Python](https://img.shields.io/badge/Python-Data%20Analysis-green?style=for-the-badge&logo=python)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)

---

# 📌 Project Overview

This **Customer Behaviour Analysis** project is an end-to-end data analytics solution designed to analyze customer purchasing patterns, subscription behavior, product preferences, revenue trends, and customer demographics.

The project combines:

- **SQL** for data querying and transformation
- **Python (Pandas)** for data cleaning & preprocessing
- **Power BI** for interactive dashboard visualization

The dashboard provides valuable business insights that help understand:

- Customer purchasing habits
- Revenue contribution by category
- Age-group behavior
- Subscription trends
- Product category performance
- Shipping preferences

---

# 🚀 Project Objectives

✔ Analyze customer purchase behavior  
✔ Identify high-performing product categories  
✔ Understand subscription impact on sales  
✔ Track customer demographics and ratings  
✔ Build an interactive business dashboard  
✔ Generate data-driven business insights  

---

# 🧠 Business Questions Solved

### Customer Insights
- Total number of customers?
- Average purchase amount?
- Average customer review rating?
- Which age group purchases the most?

### Revenue Analysis
- Which category generates the highest revenue?
- Revenue contribution by product category
- Impact of subscription on purchases

### Behaviour Analysis
- Customer distribution across categories
- Preferred shipping types
- Subscription vs non-subscription comparison
- Purchase trend by age group

---

# 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| PostgreSQL | Database Management |
| SQL | Data Analysis Queries |
| Python | Data Cleaning & Preprocessing |
| Pandas | Data Manipulation |
| Power BI | Dashboard Visualization |
| Excel/CSV | Dataset Source |

---

# 📂 Project Structure

```bash
Customer_Behaviour_Analysis/
│
├── dataset/
│   └── customer_shopping_data.csv
│
├── sql/
│   └── customer_behaviour_queries.sql
│
├── powerbi/
│   └── customer_behaviour_dashboard.pbix
│
├── images/
│   └── dashboard.png
│
├── notebooks/
│   └── data_cleaning.ipynb
│
└── README.md
```

---

# 📊 Dashboard Features

## KPI Cards
- Total Customers
- Average Purchase Amount
- Average Review Rating

## Interactive Filters
- Subscription Status
- Gender
- Product Category
- Shipping Type

## Visualizations
- Revenue by Category
- Customers by Category
- Purchase by Age Group
- Customers by Age Group
- Subscription Status Breakdown

---

# 📸 Dashboard Preview

## Customer Behaviour Dashboard

<img width="100%" src="images/dashboard.png">

---

# 🔍 Key Insights

### 📈 Revenue Insights
- Clothing category generates the highest revenue
- Accessories category contributes significantly to repeat purchases

### 👥 Customer Insights
- Young adults are the most active buyers
- Subscription users show higher purchasing frequency

### ⭐ Review Analysis
- Average review rating remains consistently high
- Positive ratings indicate good customer satisfaction

### 🚚 Shipping Insights
- Free shipping is the most preferred shipping method
- Express delivery users generally spend more per purchase

---

# ⚙️ SQL Concepts Used

```sql
SELECT
GROUP BY
ORDER BY
CTE
WINDOW FUNCTIONS
DENSE_RANK()
CASE WHEN
JOINS
AGGREGATE FUNCTIONS
SUBQUERIES
```

---

# 🐍 Python Concepts Used

```python
Pandas
Data Cleaning
Handling Missing Values
Feature Engineering
Data Transformation
Exploratory Data Analysis
```

---

# 📊 Power BI Concepts Used

- Data Modeling
- DAX Measures
- KPI Cards
- Interactive Slicers
- Custom Visualizations
- Dashboard Design
- Data Relationships

---

# 📈 Example SQL Query

```sql
-- Revenue by Category

SELECT
    category,
    SUM(purchase_amount) AS total_revenue
FROM customer_data
GROUP BY category
ORDER BY total_revenue DESC;
```

---

# 🎯 Project Outcome

This project demonstrates how raw customer data can be transformed into actionable business insights using modern data analytics tools.

The dashboard helps businesses:
- Improve customer targeting
- Optimize product categories
- Increase customer retention
- Enhance marketing decisions
- Improve sales strategy

---

# 💡 Future Improvements

- Add predictive analytics using Machine Learning
- Build customer segmentation model
- Deploy dashboard online
- Add real-time data updates
- Create automated reporting system

---

# 🧑‍💻 Author

## Prateek Yadav

- B.Tech CSE Student
- Data Analytics Enthusiast
- SQL | Python | Power BI

---

# ⭐ If You Like This Project

Give this repository a ⭐ on GitHub and support the project.

---

# 📬 Contact

Feel free to connect for collaboration, learning, or project discussions.

```bash
Email: your_email@gmail.com
LinkedIn: your_linkedin_profile
GitHub: https://github.com/yourusername
```

---

# 🏆 Final Result

An interactive end-to-end Customer Behaviour Analytics solution capable of transforming customer data into meaningful business intelligence and actionable insights.
