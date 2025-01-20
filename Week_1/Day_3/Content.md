# Day 3 Content: Python Basics for Data Analysis

## Overview
Python is a versatile programming language that excels at data analysis. This guide will cover:
1. Loading and exploring data with pandas.
2. Cleaning datasets, including handling missing values.
3. Filtering and transforming data.

By the end of the day, you will be able to write Python scripts for basic data analysis tasks.

---

### 1. Loading Data with pandas
Use the pandas library to load datasets:
import pandas as pd
df = pd.read_csv('cleveland1.csv')
print(df.head())

---

### 2. Exploring Data
Inspect the dataset:
- `df.info()`: Overview of columns and data types.
- `df.describe()`: Summary statistics.

---

### 3. Cleaning Data
Handle missing values and ensure consistency:
df['cholesterol'].fillna(df['cholesterol'].median(), inplace=True)

---

### 4. Filtering Data
Filter rows based on conditions:
filtered_df = df[df['age'] > 50]

---

### Bonus Learning
Explore these advanced topics:
1. **Visualizing Data**:
   - Use matplotlib to create basic plots.
   - Example:
     import matplotlib.pyplot as plt
     df['age'].hist()
     plt.show()
2. **Merging DataFrames**:
   - Combine multiple datasets using `merge`.

---

### Practice Example
Dataset: `cleveland2.csv`
Task:
1. Replace missing values in `chol` with the median.
2. Filter rows where `age` > 60.
3. Save the filtered dataset.
