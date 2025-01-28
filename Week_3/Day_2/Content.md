# Data Cleaning and Transformation (Continued)

## Handling Missing Data
Missing data is common in real-world datasets. It's important to deal with it correctly to ensure the integrity of the analysis. The three common approaches for handling missing data are:

1. **Removal**:
   - Remove rows or columns with missing data. This is only advisable when the data missing is minimal and doesn't impact the overall dataset.
   - Example: `df.dropna()` in Python.

2. **Imputation**:
   - Impute missing data by filling it with a specific value. Common strategies include filling with the mean, median, or mode of the column.
   - In Excel, use `IF` and `ISBLANK` functions to identify and replace missing values.
   - SQL offers `COALESCE()` or `IFNULL()` to handle missing data.

3. **Prediction**:
   - Use machine learning techniques to predict missing values based on the rest of the data.

---

## Identifying and Correcting Data Inconsistencies

Data inconsistencies arise from errors in data entry or inconsistent formats. Two common types of inconsistencies are:

1. **Duplicate Data**:
   - Duplicates can skew results and lead to errors. In SQL, you can use `DISTINCT` to find unique entries, while in Excel, the "Remove Duplicates" feature helps identify and eliminate them.
   - Example: `SELECT DISTINCT column_name FROM table` (SQL).

2. **Inconsistent Data Entries**:
   - This includes inconsistent use of case, naming conventions, or categories. You can standardize data using SQL `UPDATE` queries or Excel's "Text to Columns" feature for reformatting.
   - Example: `UPDATE products SET product_name = 'CorrectName' WHERE product_name = 'IncorrectName';` (SQL).

---

## Data Normalization and Standardization

Both normalization and standardization are techniques used to rescale the data to a specific range or distribution.

- **Normalization**: Rescales the data into a [0, 1] range, often used for machine learning models.
  - Formula: `(X - min(X)) / (max(X) - min(X))`
  
- **Standardization**: Scales the data by subtracting the mean and dividing by the standard deviation, making the data follow a Gaussian distribution.
  - Formula: `(X - mean(X)) / std(X)`

In Python, you can use libraries like Pandas and Scikit-learn to normalize and standardize data. Excel offers similar functionality through the use of formulas.

---

## Data Transformation Using Excel

Excel provides a powerful set of tools for data cleaning and transformation:

1. **Find and Replace**:
   - Use Excel’s "Find and Replace" tool to correct text inconsistencies.
   
2. **Conditional Formatting**:
   - Use conditional formatting to highlight anomalies in data, such as outliers or duplicates.

3. **Data Validation**:
   - Set data validation rules to ensure that only valid data entries are allowed in specific cells.

---

## Data Transformation Using SQL

SQL is a powerful tool for cleaning and transforming data at scale. Common SQL techniques for cleaning data include:

1. **Using `UPDATE` and `DELETE`**:
   - Modify or delete records based on conditions. For example, removing records with null values in a particular column.
   - Example: `UPDATE employees SET salary = 50000 WHERE salary IS NULL;`

2. **Aggregating Data**:
   - Group data by columns and apply aggregate functions like `SUM`, `AVG`, `MAX`, and `MIN`.
   - Example: `SELECT AVG(salary) FROM employees GROUP BY department;`

---

## Python Data Transformation

Python is highly efficient for handling large datasets. The Pandas and Numpy libraries are especially useful for data cleaning and transformation.

- **Pandas**:
  - Use `fillna()` to fill missing values.
  - Use `dropna()` to remove missing values.
  - Example: `df.fillna(df.mean())`

- **Numpy**:
  - Use Numpy for numerical transformations and handling large-scale arrays.

Example: `numpy.where()` for condition-based transformation.

---
