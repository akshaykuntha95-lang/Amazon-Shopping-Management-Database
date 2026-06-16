# Amazon Shopping Management Database

## Overview

A SQL-based e-commerce database inspired by Amazon, designed to manage customers, sellers, products, orders, payments, and reviews. The project demonstrates database design, normalization, data integrity, and business analytics using SQL.

## Features

* Customer Management
* Seller & Product Catalog
* Order Processing System
* Payment Tracking
* Product Reviews & Ratings
* Inventory Management
* Business Intelligence Queries

## Database Schema

The database consists of 7 relational tables:

* **Customer**
* **Seller**
* **Product**
* **Orders**
* **Order_Details**
* **Payment**
* **Review**

Relationships are maintained using **Primary Keys** and **Foreign Keys** to ensure data integrity.

## SQL Concepts Used

* CREATE TABLE
* PRIMARY KEY & FOREIGN KEY
* JOINs
* GROUP BY & HAVING
* Aggregate Functions
* Subqueries
* Constraints
* ORDER BY & LIMIT

## Business Insights

* Identify high-value customers.
* Monitor low-stock products.
* Analyze revenue by payment method.
* Calculate average product ratings.
* Track order and sales performance.

## Sample Queries

### Top Customers

```sql
SELECT customer_name,
       SUM(total_amount) AS total_spent
FROM orders
GROUP BY customer_name
ORDER BY total_spent DESC;
```

### Low Inventory Products

```sql
SELECT product_name, stock_quantity
FROM product
WHERE stock_quantity < 10;
```

## Project Structure

```text
Amazon-Shopping-Management-Database/
│
├── SQL Scripts/
├── ER Diagram/
├── Screenshots/
└── README.md
```

## Learning Outcomes

* Relational Database Design
* Database Normalization
* SQL Query Writing
* Data Integrity Management
* Business Analytics using SQL

## Author

**Akshay Kuntha**

SQL | Python | Data Analytics | Machine Learning
