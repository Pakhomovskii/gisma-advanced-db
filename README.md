### Final assessment for M605 Advanced Databases module

[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14-orange.svg)](https://www.postgresql.org/)

This project focuses on the design and normalization of a database for an online shop. It keeps track of customers, products, and orders. I've made sure everything has a unique ID and linked the tables so I can easily see what customers ordered. To make things run faster, I've added shortcuts for finding things and set up rules to keep the data accurate.

- **init_db.sql** script with SQL commands to create DB, tables, roles, etc.

- **insert.sql** insertion sample data in DB

- **reporting.sql** DML commands to see specific reports 

### ER Diagram

<img width="1290" alt="Screenshot 2024-07-01 at 08 37 53" src="https://github.com/Pakhomovskii/gisma-advanced-db/assets/69305661/39b9cc69-f0c3-4176-a3fb-75ef388d53ec">


you can try it with (It is my private server):
```bash
psql -h 34.133.15.56 -U readonly_user -d online_shop
```
password: 12345
