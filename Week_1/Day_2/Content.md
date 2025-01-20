# Day 2 Content: SQL Basics for Data Analysis

## Overview
SQL (Structured Query Language) is the standard language for interacting with databases. It allows you to retrieve, filter, and manipulate data efficiently. This guide will cover:
1. Writing basic SQL queries.
2. Filtering and sorting data.
3. Aggregating data using functions like `SUM`, `AVG`, and `COUNT`.

By the end of the day, you will know how to interact with a database using SQL commands.

---

### 1. Basic SQL Structure
SQL queries are composed of clauses:
- `SELECT`: Specifies the columns to retrieve.
- `FROM`: Specifies the table to query.
- `WHERE`: Filters rows based on conditions.
- `ORDER BY`: Sorts the result.

#### Example Query
Retrieve rows where `Fiscal Year` is "2021/22":
SELECT * FROM Casino_Gaming_Data
WHERE `Fiscal Year` = '2021/22';

---

### 2. Filtering and Sorting
Filters narrow down results, while sorting organizes them meaningfully.

#### Example
Filter rows where `Online Casino Gaming Win/(Loss)` > 30,000 and sort by `Licensee`:
SELECT * FROM Casino_Gaming_Data
WHERE `Online Casino Gaming Win/(Loss)` > 30000
ORDER BY `Licensee`;

---

### 3. Aggregating Data
Aggregation functions summarize data:
- `SUM`: Adds numeric values.
- `AVG`: Calculates the average.
- `COUNT`: Counts rows.

#### Example
Calculate total `Wagers` for the year 2022:
SELECT SUM(Wagers) AS Total_Wagers
FROM Casino_Gaming_Data
WHERE `Fiscal Year` = '2022/23';

---

### Bonus Learning
Explore these additional SQL concepts:
1. **GROUP BY**:
   - Aggregate data by categories.
   - Example:
     SELECT `Fiscal Year`, AVG(Wagers) AS Avg_Wagers
     FROM Casino_Gaming_Data
     GROUP BY `Fiscal Year`;
2. **JOINs**:
   - Combine data from multiple tables.

---

### Practice Example
Dataset: `Casino_Gaming_Data`
Task:
1. Retrieve all rows where `Cancelled Wagers` > 10.
2. Sort by `Total Gross Gaming Revenue` in descending order.
3. Save the result as a query file.
