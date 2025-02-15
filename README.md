### Final assessment for M605 Advanced Databases module

[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14-orange.svg)](https://www.postgresql.org/)

This project focuses on the design and normalization of a database for an online shop. The goal is to analyze the requirements provided by ABC Company, create the database schema, populate it with test data, and demonstrate its functionality with SQL queries. While the final application may use an ORM (Object-Relational Mapping) system, this project will focus exclusively on SQL.

- **init_db.sql** script with SQL commands to create DB, tables, roles, etc.

- **insert.sql** insertion sample data in DB

- **reporting.sql** DML commands to see specific reports

- **corrections.sql** I've made some improvements

### ER Diagram (new version)

<img width="1338" alt="Screenshot 2024-07-11 at 07 36 39" src="https://github.com/Pakhomovskii/gisma-advanced-db/assets/69305661/7c9b1b2c-93ea-40bb-b0d4-b0b8ad5df99a">

### ER Diagram (old version)

<img width="1290" alt="Screenshot 2024-07-01 at 08 37 53" src="https://github.com/Pakhomovskii/gisma-advanced-db/assets/69305661/39b9cc69-f0c3-4176-a3fb-75ef388d53ec">


you can try it with (It is my private server):
```bash
psql -h 34.133.15.56 -U readonly_user -d online_shop
```
password: 12345
```sql
-- Information about suppliers and the number of products they provide:	
SELECT * FROM View_SupplierProductCount;
-- Top 10 best-selling products with the total amount sold and their supplier:	
SELECT * FROM View_Top10SellingProducts;
-- List of customers and their total purchases:	
SELECT * FROM View_CustomerTotalPurchases;
-- List of returned items:	
SELECT * FROM View_ReturnedItems;
-- List of products in the fashion category that were sold last month:	
SELECT * FROM View_FashionProductsSoldLastMonth;
```
