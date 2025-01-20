# Day 5 Content: Intermediate SQL Queries

## Overview
Intermediate SQL builds on the basics by introducing powerful techniques for combining and summarizing data. This guide will cover:
1. Joining tables.
2. Aggregating data with GROUP BY.
3. Using HAVING for filtered aggregations.

By the end of the day, you’ll be able to write complex SQL queries to analyze data from multiple tables.

---

### 1. Joining Tables
JOINs combine data from two or more tables based on a related column.

#### Types of JOINs
- **INNER JOIN**: Returns only matching rows.
- **LEFT JOIN**: Returns all rows from the left table and matching rows from the right table.
- **RIGHT JOIN**: Returns all rows from the right table and matching rows from the left table.
- **FULL OUTER JOIN**: Returns all rows from both tables.

#### Example
Combine `Casino_Gaming_Data` and `Quality_of_Life` to include country-related metrics:
SELECT g.`Licensee`, g.`Total Gross Gaming Revenue`, q.`Quality of Life Value`
FROM `Casino_Gaming_Data` g
INNER JOIN `Quality_of_Life` q
ON g.`country_code` = q.`country`;

---

### 2. Aggregating Data with GROUP BY
GROUP BY groups rows into categories and applies aggregate functions.

#### Aggregate Functions
- `SUM`: Adds numeric values.
- `AVG`: Calculates the average.
- `COUNT`: Counts rows.
- `MAX`/`MIN`: Finds the highest/lowest value.

#### Example
Calculate total `Wagers` per `Fiscal Year`:
SELECT `Fiscal Year`, SUM(`Wagers`) AS Total_Wagers
FROM `Casino_Gaming_Data`
GROUP BY `Fiscal Year`;

---

### 3. Filtering Aggregations with HAVING
HAVING applies filters to grouped data.

#### Example
Filter results to show years with total `Wagers` greater than 300,000:
SELECT `Fiscal Year`, SUM(`Wagers`) AS Total_Wagers
FROM `Casino_Gaming_Data`
GROUP BY `Fiscal Year`
HAVING Total_Wagers > 300000;

---

### Bonus Learning
Explore these additional SQL concepts:
1. **Subqueries**:
   - Use queries inside another query.
   - Example:
     SELECT `Licensee`, `Total Gross Gaming Revenue`
     FROM `Casino_Gaming_Data`
     WHERE `Total Gross Gaming Revenue` > 
         (SELECT AVG(`Total Gross Gaming Revenue`) 
          FROM `Casino_Gaming_Data`);
2. **Window Functions**:
   - Perform calculations across a specific range of rows.

---

### Practice Example
Dataset: `Casino_Gaming_Data new.csv`
Task:
1. Join the dataset with `Quality_of_Life.csv` to include country-level metrics.
2. Calculate average `Wagers` for each `Fiscal Year` and filter for years with an average above 100,000.
3. Save the results as a query file.
