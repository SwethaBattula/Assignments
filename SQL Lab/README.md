🗄️ SQL Labs Portfolio – From Basics to Advanced Queries
📌 Overview

This repository contains a comprehensive collection of SQL lab exercises covering fundamental to advanced database concepts, including:

Basic SQL queries (SELECT, WHERE)
Filtering and data manipulation
JOIN operations
GROUP BY and aggregations
Subqueries and nested queries
Common Table Expressions (CTEs)

These labs demonstrate practical problem-solving using real-world database scenarios such as employee management, orders, departments, and salary analysis.

📂 Included Labs
🔹 1. SQL Basics Lab (SELECT & WHERE)

📄 Source:

Focuses on foundational SQL operations:

SELECT queries (all columns, specific columns)
DISTINCT values
Column aliases
Arithmetic operations
String concatenation
WHERE clause filtering:
AND, OR, NOT
BETWEEN, IN
LIKE (pattern matching)
NULL handling

📊 Example:

Finding employees in IT department
Filtering salaries above a threshold
Pattern-based name filtering
🔹 2. SQL JOIN & GROUP BY Lab

📄 Source:

Covers relational database operations:

INNER JOIN, LEFT JOIN, SELF JOIN
GROUP BY with aggregate functions
HAVING clause
Multi-table joins
Data aggregation and reporting

📊 Key Exercises:

Employees with department names
Customers with order counts (including NULL cases)
Revenue calculation by product category
Monthly order analysis (2024 data)

📌 Database includes:

Employees, Departments
Customers, Orders
Products, Order Details
🔹 3. Advanced SQL Queries Lab

📄 Source:

Focuses on complex SQL logic:

Nested subqueries
Ranking problems (2nd highest, 3rd highest)
Date-based filtering
Yearly aggregation reports
Conditional logic without ORDER BY
Multi-level nested queries

📊 Example Problems:

2nd highest salary in Finance
Employees working in a department during a time range
Year with highest employee joining count
Department-wise yearly salary cost
🔹 4. CTE and Joins Lab

📄 Source:

Introduces Common Table Expressions (CTEs) for modular queries:

Breaking complex queries into readable parts
Reusing intermediate results
Advanced filtering and comparisons

📊 Key Tasks:

Highest salaried employee in Finance
Current department managers
Salary comparison between managers and employees
Pattern-based filtering using LIKE
Date difference calculations
🧠 Concepts Covered
✅ SQL Fundamentals
SELECT, DISTINCT, aliases
WHERE filtering techniques
✅ Intermediate SQL
JOIN operations (INNER, LEFT, SELF)
GROUP BY and aggregation
HAVING clause
✅ Advanced SQL
Subqueries (nested & correlated)
Ranking queries (Nth highest salary)
Date functions and calculations
✅ Expert-Level Concepts
Common Table Expressions (CTEs)
Multi-step query building
Performance-oriented structured queries
🏗️ Database Schema Overview

Across the labs, the following entities are used:

Employees → personal and job details
Departments → organizational structure
Salaries → salary history
Dept_Manager / Dept_Emp → relationships
Customers & Orders → transactional data
Products & Order Details → inventory and sales
🚀 How to Run
Install a SQL environment:
MySQL Workbench / PostgreSQL / SQLite
Execute database setup scripts:
Create tables
Insert sample data
Run queries lab-wise:
Start with Basics
Move to JOINs
Then Advanced & CTEs
Verify outputs using provided screenshots in each lab
📸 Outputs
Each lab includes query outputs (screenshots)
Example outputs:
Employee records
Aggregated reports
Salary comparisons
Date-based analytics

(Outputs are shown across multiple pages in the provided documents.)

⚠️ Note
ChatGPT was used only for syntax correction when required, as stated in the lab documents.
All query logic and problem-solving were implemented independently.
📈 Skills Gained
Writing optimized and readable SQL queries
Solving real-world data problems
Understanding relational database design
Performing advanced data analysis using SQL
🔮 Future Enhancements
Convert queries into reusable views and stored procedures
Add indexing strategies for performance optimization
Integrate with Power BI / Tableau dashboards
Build a web-based SQL query interface
👩‍💻 Author

Swetha Battula

⭐ Conclusion

This portfolio represents a complete SQL learning journey, progressing from:
➡️ Basic queries → Intermediate joins → Advanced subqueries → CTE-based optimization
