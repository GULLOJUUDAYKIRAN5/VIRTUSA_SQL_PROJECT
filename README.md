📊 Online Retail Sales Analysis Database
📌 Project Overview

This project focuses on designing and implementing a relational database for an online retail system. The goal is to efficiently store and analyze sales data to generate meaningful business insights. Using SQL, the project performs various analytical queries to understand customer behavior, product performance, and revenue trends.

🎯 Objectives
Design a structured relational database
Store customer, product, and order-related data
Perform data analysis using SQL queries
Generate insights to support business decisions
🗂️ Database Schema
🔹 1. Client Information (client_info)

Stores customer details.

Column Name	Data Type	Description
client_id	INT	Unique ID of the customer
client_name	VARCHAR	Name of the customer
location	VARCHAR	City of the customer
🔹 2. Product Catalog (item_catalog)

Stores product details.

Column Name	Data Type	Description
item_id	INT	Unique product ID
item_name	VARCHAR	Product name
item_group	VARCHAR	Category of product
unit_price	DECIMAL	Price per unit
🔹 3. Order Log (order_log)

Stores order-level information.

Column Name	Data Type	Description
order_id	INT	Unique order ID
client_id	INT	Customer who placed the order
order_date	DATE	Date of order
🔹 4. Order Details (order_details)

Stores product-level details for each order.

Column Name	Data Type	Description
order_id	INT	Order reference
item_id	INT	Product reference
quantity	INT	Quantity ordered
🔗 Relationships
A customer can place multiple orders (1:N)
An order can contain multiple products (1:N)
Products can appear in multiple orders (M:N via order_details)
📊 Key SQL Queries Implemented
🔹 1. Top-Selling Products

Identifies products with the highest sales quantity.

🔹 2. Most Valuable Customers

Finds customers who have spent the most.

🔹 3. Monthly Revenue Analysis

Calculates total revenue generated per month.

🔹 4. Category-wise Sales

Analyzes sales performance based on product categories.

🔹 5. Inactive Customers

Identifies customers who have not placed any orders.

🛠️ Tools & Technologies
Database: Oracle SQL
Language: SQL
Interface: SQL*Plus / Oracle Live SQL
📈 Sample Insights
Helps identify high-performing products
Tracks customer spending behavior
Provides monthly revenue trends
Highlights inactive users for re-engagement strategies
🚀 How to Run the Project
Create all tables using provided SQL scripts
Insert sample data into each table
Execute analytical queries
Observe results for insights
💡 Conclusion

This project demonstrates how structured databases and SQL queries can be used to extract valuable insights from retail data. It highlights the importance of proper database design and query optimization in real-world applications.

