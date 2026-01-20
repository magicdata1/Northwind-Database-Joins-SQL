# Northwind Database SQL Analysis

This project contains SQL queries used to analyze the Northwind database. It covers everything from basic table joins to complex data aggregations.

## Database Structure (ERD)

I analysed the Northwind schema to understand the relationships between tables like Customers, Orders, and Products.

![schema](https://github.com/magicdata1/Northwind-Database-SQL/blob/main/images/shcema.png)

## 1. INNER JOIN Examples

This shows basic INNER JOIN operations:
- Join **Customers → Orders**
- Join **Orders → Employees**
- Join **Products → Suppliers**
- Retrieve related information from multiple tables
 
![1](https://github.com/magicdata1/Northwind-Database-Joins-SQL/blob/main/images/1.png)

---

## 2. LEFT / RIGHT / CROSS JOIN + COUNT()

- **RIGHT JOIN** to find *employees with no orders*
- **CROSS JOIN** to generate Cartesian products
- **COUNT()** for Customers and Orders
- **GROUP BY** to count customers by country/city

![2](https://github.com/magicdata1/Northwind-Database-Joins-SQL/blob/main/images/2.png)

---

# 3. Filtering with WHERE + INNER JOIN

This screenshot focuses on combining filtering and INNER JOIN operations.

- Filtering suppliers using `WHERE SupplierName = 'G'day, Mate'`  
- Joining Employees → Orders  
- Joining Orders → Shippers  
- Joining Products → Categories  
- Listing products along with their categories  
- Listing order quantities using a join with Order_Details  

![3](https://github.com/magicdata1/Northwind-Database-Joins-SQL/blob/main/images/3.png)

---

# 4. Multi‑Table JOINs + Finding Missing Records

This section shows more advanced JOIN usage, especially for identifying missing/non-matching rows.

- 3‑table join: **Orders + Order_Details + Products**  
- LEFT JOIN to find customers **with or without** orders  
- RIGHT JOIN to find employees **with no orders**  
- Using `WHERE orderid IS NULL` to detect missing matches  
- CROSS JOIN  
- Using COUNT() and GROUP BY on customers  

![4](https://github.com/magicdata1/Northwind-Database-Joins-SQL/blob/main/images/4.png)

---

## 5. Aggregations (SUM, COUNT) + GROUP BY

This includes:
- SUM of product quantities  
- COUNT of orders per shipper  
- Total sales per product (`SUM(quantity * price)`)
- Customer counts per country  
- Category totals (Products + Categories + Order_Details)

![5](https://github.com/magicdata1/Northwind-Database-Joins-SQL/blob/main/images/5.png)

---


## 6. Employee and Category Aggregations

This demonstrates summary analysis using JOINs and GROUP BY:

- Total quantity handled by each employee using `SUM()`
- Number of orders processed by each employee using `COUNT()`
- Category-level total quantities using multi-table JOINs (Products + Categories + Order_Details)

![6](https://github.com/magicdata1/Northwind-Database-Joins-SQL/blob/main/images/6.png)

---


## Technical Skills Demonstrated

### 🔹 SQL Querying and Data Retrieval
- Extracting data using SELECT statements  
- Using column aliases for readability  
- Filtering data with WHERE, comparison operators, and pattern matching  

### 🔹 Relational Joins
- INNER JOIN for matching related records  
- LEFT JOIN / RIGHT JOIN for identifying missing data  
- CROSS JOIN for Cartesian results  
- Multi‑table joins (Orders + Order_Details + Products)

### 🔹 Data Filtering and Conditions
- Filtering suppliers, employees, customers, and products  
- Using WHERE with strings, numbers, and dates  
- Detecting missing relationships with `IS NULL`  

### 🔹 Aggregation and Grouping
- Using COUNT(), SUM(), AVG() for analysis  
- Grouping by employee, category, country, city, and shipper  
- Calculating total sales using `SUM(quantity * price)`  

### 🔹 Data Analysis and Reporting
- Counting customers by region  
- Identifying employees with no orders  
- Summarising product performance  
- Category‑level analysis using multi‑table joins  

### 🔹 Database Understanding (ERD Analysis)
- Understanding table relationships (PK/FK)  
- Translating ERD structure into SQL queries  
- Working with normalized relational schemas  

