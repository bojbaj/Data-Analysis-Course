# Day 6 Content: Python for Data Cleaning and Transformation

## Overview
Cleaning and transforming data is a crucial step in data analysis. Python’s pandas library provides powerful tools for these tasks. This guide covers:
1. Handling missing values.
2. Standardizing and formatting data.
3. Creating and transforming columns.

By the end of the day, you’ll be able to clean and prepare datasets for analysis.

---

### 1. Handling Missing Values
Messy datasets often have missing or null values that need to be addressed.

#### Techniques
1. **Fill Missing Values**:
   - Replace missing values with a default or calculated value:
     df['column_name'].fillna(value, inplace=True)
2. **Drop Missing Rows**:
   - Remove rows with missing data:
     df.dropna(subset=['column_name'], inplace=True)

#### Example
Dataset: `retail_store_sales.csv`
- Replace missing values in the `Price Per Unit` column with the median price.
- Drop rows where `Transaction ID` is missing.

---

### 2. Standardizing and Formatting Data
Standardizing data ensures consistency and accuracy.

#### Techniques
1. **Format Strings**:
   - Convert text to lowercase:
     df['column_name'] = df['column_name'].str.lower()
2. **Format Dates**:
   - Convert strings to datetime:
     df['date_column'] = pd.to_datetime(df['date_column'])

#### Example
Dataset: `nike_sales_2024.csv`
- Standardize `Region` names to be lowercase.
- Convert the `Month` column to a standard date format.

---

### 3. Creating and Transforming Columns
Derived columns can help uncover new insights.

#### Techniques
1. **Create New Columns**:
   - Add calculated columns:
     df['Total_Sales'] = df['Units_Sold'] * df['Retail_Price']
2. **Transform Existing Columns**:
   - Apply mathematical or string transformations:
     df['Percentage'] = df['Online_Sales_Percentage'] / 100

#### Example
Dataset: `nike_sales_2024.csv`
- Create a `Profit` column by subtracting `Cost` from `Revenue_USD`.

---

### Bonus Learning
Explore these advanced pandas features:
1. **Pivot Tables in pandas**:
   - Summarize data like in Excel:
     pivot = df.pivot_table(values='Revenue_USD', index='Region', columns='Price_Tier', aggfunc='sum')
2. **Lambda Functions**:
   - Apply custom transformations:
     df['Adjusted_Revenue'] = df['Revenue_USD'].apply(lambda x: x * 0.9)

---

### Practice Example
Dataset: `retail_store_sales.csv`
Task:
1. Replace missing values in `Discount Applied` with "False".
2. Create a new column `Total_Spent` (Quantity × Price Per Unit).
3. Save the cleaned dataset.
