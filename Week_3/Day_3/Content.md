# Day 3 Content: Advanced Data Cleaning with SQL

## Overview
Today, we focus on advanced data cleaning techniques using SQL. You will learn how to write complex queries to clean and transform datasets, handle missing data, and standardize data formats. By the end of the day, you will be able to use SQL to prepare datasets for analysis efficiently.

---

## 1. Why Use SQL for Data Cleaning?
SQL is a powerful tool for data cleaning because it allows you to:
- Filter and transform large datasets quickly.
- Handle missing data and duplicates efficiently.
- Standardize data formats across multiple tables.
- Combine data from different sources using joins.

---

## 2. Handling Missing Data in SQL
Missing data can occur in various forms, such as NULL values or empty strings. Techniques to handle missing data in SQL include:

### 2.1 Removing Rows with Missing Data
- Use the `DELETE` statement to remove rows where specific columns contain NULL values.
- Example: Delete rows where the `Price` column is NULL.

### 2.2 Filling Missing Data
- Use the `UPDATE` statement to replace NULL values with default values, averages, or other calculated values.
- Example: Replace NULL values in the `Price` column with the average price.

---

## 3. Removing Duplicates in SQL
Duplicate rows can skew analysis results. Techniques to remove duplicates in SQL include:

### 3.1 Identifying Duplicates
- Use the `GROUP BY` and `HAVING` clauses to identify duplicate rows based on specific columns.
- Example: Find duplicate rows based on the `Customer ID` column.

### 3.2 Removing Duplicates
- Use the `DELETE` statement with a subquery to remove duplicate rows.
- Example: Remove duplicate rows while keeping the first occurrence.

---

## 4. Standardizing Data Formats in SQL
Inconsistent data formats can lead to errors in analysis. Techniques to standardize data formats in SQL include:

### 4.1 Text Formatting
- Use the `UPDATE` statement with string functions like `LOWER()`, `UPPER()`, or `TRIM()` to standardize text data.
- Example: Convert the `Category` column to lowercase.

### 4.2 Date and Time Formatting
- Use the `UPDATE` statement with date functions like `DATE_FORMAT()` or `CAST()` to standardize date formats.
- Example: Convert the `Transaction Date` column to a consistent format.

---

## 5. Combining Data with Joins
SQL joins allow you to combine data from multiple tables. Techniques include:

### 5.1 Inner Join
- Combine rows from two tables where the join condition is met.
- Example: Combine customer data with transaction data using the `Customer ID` column.

### 5.2 Left Join
- Include all rows from the left table and matching rows from the right table.
- Example: Include all customers, even if they have no transactions.

---

## 6. Practice Exercises
Use the provided datasets to complete the following tasks:
- Practice 1: Remove rows with missing data.
- Practice 2: Fill missing values with default values.
- Practice 3: Remove duplicate rows.
- Practice 4: Standardize text formatting.
- Practice 5: Combine data from multiple tables using joins.
- Practice 6: Validate data integrity.

---

## 7. Advanced Reading
For further learning:
- [SQL Data Cleaning Best Practices](https://towardsdatascience.com/sql-data-cleaning-best-practices)
- [Handling Missing Data in SQL](https://www.sqlshack.com/handling-missing-data-in-sql-server/)