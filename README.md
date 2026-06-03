# 🛒 E-Commerce Sales Analysis Using SQL

## 📌 Project Overview
This project performs end-to-end data analysis on an 
Online Retail dataset using SQL. The goal is to extract 
meaningful business insights such as top customers, 
revenue by country, bulk orders, and product performance 
using structured queries in SQLite.

## 🗃️ Dataset
- **Source:** [Online Retail Dataset - Kaggle]
- **Tool Used:** SQLite with DB Browser for SQLite
- **Total Rows:** 541,909 transactions
- **Columns:** InvoiceNo, StockCode, Description, Quantity, 
               InvoiceDate, UnitPrice, CustomerID, Country

## 🗄️ Database Structure
The flat CSV was normalized into 3 relational tables:

| Table | Columns |
|---|---|
| customers | CustomerID, Country |
| products | StockCode, Description, UnitPrice |
| orders | InvoiceNo, CustomerID, StockCode, Quantity, InvoiceDate |

## 📊 Queries & Business Insights

| Query | Title | Insight |
|---|---|---|
| 1 | NULL Value Check | Identified missing CustomerIDs and invalid descriptions |
| 2 | High Quantity Orders | Found bulk purchase transactions sorted by date |
| 3 | Revenue by Country | United Kingdom is the highest revenue generating market |
| 4 | Inner Join Order Details | Complete view of transactions with product and location |
| 5 | Left Join Inactive Customers | Identified customers with no orders for marketing |
| 6 | Subquery High Volume Buyers | Customers buying above average quantity |
| 7 | Top 10 Customers by Revenue | VIP customer list ranked by total spending |
| 8 | High Value Customers View | Reusable view of customers who spent over £1000 |
| 9 | Index Optimization | Added indexes on CustomerID, StockCode, InvoiceDate |

## 📸 Screenshots
All query outputs are available in the /screenshots folder.

## 🛠️ Tools Used
- SQLite
- DB Browser for SQLite
- Kaggle (Dataset Source)

