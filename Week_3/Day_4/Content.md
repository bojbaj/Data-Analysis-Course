# Day 4 Content: Data Transformation with Python

## Overview
Today, we focus on data transformation techniques using Python. You will learn how to manipulate and reshape datasets, handle missing data, and create new columns for analysis. By the end of the day, you will be able to transform raw data into a format suitable for analysis using Python.

---

## 1. Why Use Python for Data Transformation?
Python is a versatile tool for data transformation because it allows you to:
- Handle large datasets efficiently.
- Perform complex transformations with ease.
- Automate repetitive tasks using scripts.
- Integrate with other data analysis tools and libraries.

---

## 2. Handling Missing Data in Python
Missing data can occur in various forms, such as NULL values or empty strings. Techniques to handle missing data in Python include:

### 2.1 Removing Rows with Missing Data
- Use the `dropna()` function to remove rows where specific columns contain missing values.
- Example: Remove rows where the `Price` column is missing.

### 2.2 Filling Missing Data
- Use the `fillna()` function to replace missing values with default values, averages, or other calculated values.
- Example: Replace missing values in the `Price` column with the median price.

---

## 3. Removing Duplicates in Python
Duplicate rows can skew analysis results. Techniques to remove duplicates in Python include:

### 3.1 Identifying Duplicates
- Use the `duplicated()` function to identify duplicate rows based on specific columns.
- Example: Find duplicate rows based on the `Customer ID` column.

### 3.2 Removing Duplicates
- Use the `drop_duplicates()` function to remove duplicate rows while keeping the first occurrence.
- Example: Remove duplicate rows based on the `Customer ID` column.

---

## 4. Standardizing Data Formats in Python
Inconsistent data formats can lead to errors in analysis. Techniques to standardize data formats in Python include:

### 4.1 Text Formatting
- Use string functions like `str.lower()`, `str.upper()`, or `str.strip()` to standardize text data.
- Example: Convert the `Category` column to lowercase.

### 4.2 Date and Time Formatting
- Use the `pd.to_datetime()` function to standardize date formats.
- Example: Convert the `Transaction Date` column to a consistent format.

---

## 5. Creating New Columns
Derived columns can help uncover new insights. Techniques to create new columns in Python include:

### 5.1 Calculated Columns
- Use arithmetic operations to create new columns based on existing ones.
- Example: Create a `Total Revenue` column by multiplying `Price` and `Quantity`.

### 5.2 Conditional Columns
- Use the `apply()` function to create columns based on conditions.
- Example: Create a `Discount Applied` column based on the `Price` column.

---

## 6. Practice Exercises
Use the provided datasets to complete the following tasks:
- Practice 1: Remove rows with missing data.
- Practice 2: Fill missing values with default values.
- Practice 3: Remove duplicate rows.
- Practice 4: Standardize text formatting.
- Practice 5: Create new columns for analysis.
- Practice 6: Validate data integrity.

---

## 7. Advanced Reading
For further learning:
- [Python Data Transformation Best Practices](https://towardsdatascience.com/python-data-transformation-best-practices)
- [Handling Missing Data in Python](https://realpython.com/python-data-cleaning-numpy-pandas/)