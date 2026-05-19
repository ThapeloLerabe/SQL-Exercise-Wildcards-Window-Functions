☕ Bright Coffee Shop Sales – Advanced SQL Exercise
📌 Overview
This project contains my solutions to the Advanced SQL Exercise focused on:

✅ SQL Wildcards (LIKE, RLIKE, %, _)
✅ Window Functions (Aggregate, Ranking, Value functions)
✅ Analytical problem-solving using real-world sales data

The dataset is based on a fictional coffee shop chain with multiple store locations, and the tasks were completed using Databricks SQL.

🗂️ Dataset Description
The dataset used is:
coffee_sales
It contains transactional sales data from three locations:

Lower Manhattan
Hell’s Kitchen
Astoria

🎯 Objectives
This exercise was designed to strengthen:

SQL filtering using wildcards
Pattern matching using LIKE and RLIKE
Using window functions without grouping
Performing ranking and analytical calculations
Understanding partitioning and ordering

🔹 Section A: SQL Wildcards
Covered:

LIKE patterns (%, _)
Filtering text patterns (e.g. products starting with "Dark")
Combining conditions using OR
Using NOT LIKE
Regex with RLIKE
Identifying patterns in product names

🔹 Section B: Window Functions
📌 Aggregate Functions

SUM() → total revenue per store
AVG() → average revenue
Running totals using ORDER BY

**📊 Ranking Functions

ROW_NUMBER()
RANK()
DENSE_RANK()
NTILE(4) (quartiles)


🔄 Value Functions

LAG() → previous row
LEAD() → next row
FIRST_VALUE() → first value in partition

🧠 Key Learnings

Window functions do not reduce rows like GROUP BY
PARTITION BY creates independent groups
ORDER BY controls calculation flow (important for running totals)
RANK and DENSE_RANK behave differently when ties exist
Data cleaning (e.g., trimming spaces) is important for accurate results

⚠️ Challenges Faced

Handling inconsistent data formats (e.g., comma vs decimal in unit_price)
Understanding why COUNT DISTINCT returned unexpected results
Ensuring correct sorting for window functions
Debugging NULL values in LEAD() and default values in LAG()

