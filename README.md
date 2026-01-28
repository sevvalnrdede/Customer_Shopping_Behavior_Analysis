# 🛍️ Customer Shopping Behavior Analysis
### End-to-End Data Analytics Project (Python | MS SQL Server | Power BI)

## 📌 Project Overview
This project analyzes a retail dataset to identify customer segments, shopping habits, and the impact of loyalty programs. It covers the entire data lifecycle: from automated ETL with Python to advanced T-SQL querying and interactive business intelligence reporting.

## 🎯 Project Objectives
* **Customer Segmentation:** Classifying customers based on their purchase frequency.
* **Product Analytics:** Identifying top-performing items and categories by rating and volume.
* **Behavioral Analysis:** Examining the influence of subscription status and discounts on total spending.
* **Shipping & Payment Trends:** Analyzing preferred shipping methods and payment types across different demographics.

---

## 🛠️ Tech Stack
* **Python (Pandas, SQLAlchemy):** For data cleaning and automated ETL to MS SQL Server.
* **MS SQL Server (T-SQL):** For complex analytical queries and window functions.
* **Power BI:** For data modeling and interactive dashboard visualization.

---

## 💡 Key Business Insights (Based on SQL Analysis)

### 👥 Customer Segmentation
* **Loyal Customers:** Significant portion of the revenue comes from customers with **10+ previous purchases**.
* **New Members:** Identified a growing segment of first-time buyers particularly in the **Clothing** category.

### 📦 Product & Category Performance
* **Top 3 Products:** Identified the highest-ranking items within each category using `ROW_NUMBER()` window functions.
* **Rating Trends:** Specific categories like **Accessories** show higher average review ratings despite lower sales volume.

### 💳 Shipping & Subscriptions
* **Express Shipping:** Customers choosing Express Shipping tend to have a higher average purchase amount compared to Standard shipping.
* **Subscription Impact:** Subscribed members show a higher frequency of purchase, providing a steady revenue stream.

---

## 📂 Project Structure
* 📄 `Customer_ Shopping_Behavior_Analysis.ipynb`: Python notebook for data cleaning and SQL migration.
* 📄 `customer_behavior.sql`: T-SQL scripts for segmentation, rankings, and KPI calculations.
* 📄 `Customer_Behavior_Dashboard.pbix`: The interactive Power BI report.
* 📄 `customer_shopping_behavior.csv`: The raw dataset.


## 📜 License
This project is licensed under the **MIT License** — feel free to fork, star, and use it in your portfolio!

