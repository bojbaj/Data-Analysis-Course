# Day 1 Content: Excel Basics for Data Analysis

## Overview
Excel is one of the most widely used tools for data analysis. Its intuitive interface allows for quick data organization, cleaning, and visualization. This guide will cover:
1. Filtering and sorting data.
2. Creating and using pivot tables.
3. Basic data cleaning operations.

By the end of the day, you will have a strong grasp of Excel's core features for handling data effectively.

---

### 1. Filtering and Sorting Data
Filtering and sorting data is essential to focus on relevant subsets and organize information meaningfully.

#### Steps to Filter Data
1. Open the dataset `country_dim.csv` in Excel.
2. Click on any cell in the dataset.
3. Go to the **Data** tab and click **Filter**.
4. Select a column (e.g., `country_code`) and choose a specific value to filter.
5. Use custom filters, such as "contains", "does not contain", or ranges.

#### Steps to Sort Data
1. Select the entire dataset or the column you want to sort.
2. Click on **Sort** in the **Data** tab.
3. Choose the sort criteria:
   - Ascending (A-Z or smallest to largest).
   - Descending (Z-A or largest to smallest).

#### Example
- Filter: Show rows where `country_code` is "US".
- Sort: Order `shoe_metric` column in ascending order.

---

### 2. Creating Pivot Tables
Pivot tables summarize data by aggregating information in a structured format.

#### Steps to Create a Pivot Table
1. Select the dataset (e.g., `country_dim.csv`).
2. Go to the **Insert** tab and click **PivotTable**.
3. Place the pivot table in a new or existing sheet.
4. Drag fields:
   - Rows: `country_code`.
   - Values: `shoe_metric`.

#### Example
- Use the `shoes_dim.csv` dataset.
- Create a pivot table to count the number of `id` by `gender`.

---

### 3. Cleaning Data
Clean data ensures consistency and accuracy in analysis.

#### Cleaning Techniques
1. **Removing Duplicates**:
   - Select the dataset.
   - Go to **Data** > **Remove Duplicates**.
2. **Formatting Cells**:
   - Align text and numbers appropriately.
   - Format dates using **Custom Date Formats**.

#### Example
- Remove duplicate rows from `country_dim.csv`.
- Format the `currency` column to have consistent capitalization.

---

### Bonus Learning
Explore these additional Excel features:
1. **Conditional Formatting**:
   - Highlight cells with specific conditions (e.g., values greater than 50).
2. **Basic Formulas**:
   - `=SUM(A1:A10)`: Sum values.
   - `=AVERAGE(A1:A10)`: Calculate the mean.
3. **Chart Creation**:
   - Create bar charts for visualizing `shoe_metric` by `country_code`.

---

### Practice Example
Dataset: `shoes_dim.csv`
Task:
1. Filter rows where `best_for_wear` is "City".
2. Sort by `dominant_color` in descending order.
3. Save the result as a new Excel file.
