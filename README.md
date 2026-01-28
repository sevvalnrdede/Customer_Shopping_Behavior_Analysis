# Customer_Shopping_Behavior_Analysis

Project Overview
This project focuses on analyzing retail customer data to uncover shopping patterns, evaluate marketing efficiency (discounts/subscriptions), and visualize key performance indicators (KPIs). The workflow involves a full ETL process using Python, deep-dive statistical analysis using MS SQL Server, and interactive reporting via Power BI.




Tech Stack

Data Processing: Python (Pandas, SQLAlchemy)

Database Management: MS SQL Server (T-SQL)

Data Visualization: Power BI

Dataset: customer_shopping_behavior.csv 

Project Structure & Workflow


1. Data Cleaning & ETL (Python)

Using the Python, the raw data was prepared for the database:

Column Standardization: Fixed inconsistent naming conventions and stripped whitespace for SQL compatibility.

Null Handling: Analyzed and treated missing values in critical columns like Review Rating.

Automated Loading: Utilized SQLAlchemy to automate the data transfer from a Pandas DataFrame directly into an MS SQL Server table named customer.


2. SQL Analysis

The customer_behavior.sql file contains complex queries designed to answer business questions:

Customer Segmentation: Used CASE statements to categorize customers into 'New', 'Returning', and 'Loyal' based on purchase history.

Ranking & Window Functions: Applied ROW_NUMBER() and PARTITION BY to find the top 3 most purchased items within every product category.

Subscription Analytics: Compared revenue and average spend between subscribed and non-subscribed members.

Shipping Impact: Analyzed if shipping types (Standard vs. Express) correlate with higher purchase amounts.


3. Interactive Dashboard
   
The Customer_Behavior_Dashboard.pbix provides a visual layer to the SQL findings:

Sales Overview: Tracking Total Revenue, Average Rating, and Purchase Frequency.

Demographic Insights: Breakdowns by Gender, Age Group, and Location.

Behavioral Filters: Slicers for Subscription Status and Discount usage to observe real-time data shifts.


Key Insights

Loyalty Wins: "Loyal" customers (10+ purchases) contribute significantly more to the total revenue compared to new acquisitions.

Category Performance: While some categories have higher sales volume, others lead in customer satisfaction (Review Ratings), suggesting areas for inventory optimization.

Discount Efficiency: Analysis shows whether customers using promo codes actually spend more than the average order value.


How to Run

Database: Create a database in MS SQL Server.

ETL: Run the Jupyter Notebook to clean the CSV and push data to your SQL instance.

Analysis: Execute customer_behavior.sql in SSMS to generate insights.

Reporting: Open the .pbix file and refresh the data source to see the dashboard.


License

MIT — feel free to fork, star, and use in your portfolio.

