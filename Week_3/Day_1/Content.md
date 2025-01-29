# Day 1 Content: Introduction to Data Cleaning

## Overview
Data cleaning is the process of preparing raw data for analysis by identifying and correcting errors, inconsistencies, and missing values. Clean data ensures accurate and reliable analysis. Today, you will learn the fundamentals of data cleaning, including handling missing data, removing duplicates, and standardizing data formats.

---

## 1. What is Data Cleaning?
Data cleaning involves:
- Identifying and correcting errors in datasets.
- Handling missing or incomplete data.
- Removing duplicate entries.
- Standardizing data formats for consistency.

### Why is Data Cleaning Important?
- Ensures data accuracy and reliability.
- Improves the quality of analysis and decision-making.
- Reduces errors in machine learning models and statistical analyses.

---

## 2. Identifying Missing Data
Missing data can occur due to various reasons, such as data entry errors or incomplete records. Common techniques to handle missing data include:

### 2.1 Removing Rows with Missing Values
- Use this technique when missing data is minimal and removing rows won’t significantly impact the dataset.
- Example: In Excel, use the "Remove Duplicates" feature. In Python, use the `dropna()` function.

### 2.2 Filling Missing Values
- Replace missing values with a default value, mean, median, or mode.
- Example: In Excel, use "Fill Down" or "Fill with Mean." In Python, use the `fillna()` function.

---

## 3. Removing Duplicates
Duplicate entries can skew analysis results. Techniques to remove duplicates include:

### 3.1 Identifying Duplicates
- Check for duplicate rows based on unique identifiers (e.g., transaction IDs).
- Example: In Excel, use the "Remove Duplicates" feature. In Python, use the `duplicated()` function.

### 3.2 Removing Duplicates
- Remove duplicate rows to ensure each entry is unique.
- Example: In Excel, use "Remove Duplicates." In Python, use the `drop_duplicates()` function.

---

## 4. Standardizing Data Formats
Inconsistent data formats can lead to errors in analysis. Standardization techniques include:

### 4.1 Text Formatting
- Convert text to a consistent case (e.g., lowercase or uppercase).
- Example: In Excel, use "Text to Columns" or "Find and Replace." In Python, use the `str.lower()` function.

### 4.2 Date and Time Formatting
- Ensure dates and times follow a consistent format.
- Example: In Excel, use "Format Cells." In Python, use the `pd.to_datetime()` function.

---

## 5. Handling Outliers
Outliers are data points that deviate significantly from the rest of the dataset. Techniques to handle outliers include:

### 5.1 Identifying Outliers
- Use statistical methods like the interquartile range (IQR) or z-scores.
- Example: In Excel, use conditional formatting. In Python, use the `describe()` function.

### 5.2 Removing or Adjusting Outliers
- Remove outliers if they are errors or adjust them if they are valid but extreme values.
- Example: In Excel, use filters. In Python, use the `clip()` function.

---

## 6. Data Validation
Data validation ensures the dataset meets specific criteria. Techniques include:

### 6.1 Checking Data Types
- Ensure each column has the correct data type (e.g., numeric, text, date).
- Example: In Excel, use "Data Validation." In Python, use the `dtypes` attribute.

### 6.2 Validating Data Ranges
- Ensure values fall within expected ranges (e.g., age between 0 and 120).
- Example: In Excel, use "Data Validation." In Python, use conditional statements.

---

## 7. Practice Exercises
Use the provided datasets to complete the following tasks:
- Practice 1: Remove rows with missing values.
- Practice 2: Fill missing values with the median.
- Practice 3: Remove duplicate entries.
- Practice 4: Standardize text formatting.
- Practice 5: Identify and handle outliers.
- Practice 6: Validate data types and ranges.

---

## 8. Advanced Reading
For further learning:
- [Data Cleaning Best Practices](https://towardsdatascience.com/data-cleaning-best-practices)
- [Handling Missing Data in Python](https://realpython.com/python-data-cleaning-numpy-pandas/)