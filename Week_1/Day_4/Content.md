# Day 4 Content: Advanced Excel for Data Analysis

## Overview
Excel’s advanced functionalities enable more efficient and insightful data analysis. This guide will cover:
1. Using advanced formulas like `VLOOKUP` and `INDEX-MATCH`.
2. Applying conditional formatting.
3. Summarizing data using advanced pivot tables.

---

### 1. Advanced Formulas
#### VLOOKUP
Use `VLOOKUP` to fetch data from another table based on a common key.
Example:
=VLOOKUP(1001, A2:E10, 3, FALSE)
- Looks for `1001` in the first column of the range `A2:E10`.
- Returns the value in the 3rd column.

#### INDEX-MATCH
`INDEX-MATCH` is a more flexible alternative to `VLOOKUP`.
Example:
=INDEX(C2:C10, MATCH(1001, A2:A10, 0))
- `MATCH` finds the row number for `1001` in column `A`.
- `INDEX` retrieves the corresponding value from column `C`.

---

### 2. Conditional Formatting
Highlight data trends and outliers visually.
1. Select the dataset.
2. Go to **Home** > **Conditional Formatting**.
3. Choose:
   - Highlight Cells Rules: Values greater than 100.
   - Data Bars: Create gradient bars for numeric values.

---

### 3. Advanced Pivot Tables
Add calculated fields to pivot tables:
1. Insert a pivot table from the dataset `Employee.csv`.
2. Drag `Department` to Rows and `Salary` to Values.
3. Add a calculated field to show the percentage of total salary by department.

---

### Bonus Learning
Explore these advanced features:
1. **Array Formulas**:
   - Example: {=SUM(A1:A10 * B1:B10)} calculates the weighted sum.
2. **Power Query**:
   - Automate data cleaning and transformations.
3. **Excel Macros**:
   - Record macros to automate repetitive tasks.

---

### Practice Example
Dataset: `PerformanceRating.csv`
Task:
1. Use `VLOOKUP` to merge performance data with employee IDs from `Employee.csv`.
2. Apply conditional formatting to highlight employees with a `ManagerRating` above 4.
3. Save the results as "Performance_Analysis.xlsx".
