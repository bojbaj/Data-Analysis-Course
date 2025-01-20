# Week 1 Exam: Hard Level

## Objective
Challenge your skills by solving real-world data analysis tasks using advanced Excel, SQL, and Python techniques.

---

### Task 1: Advanced Excel
1. Use the `nike_sales_2024.csv` dataset.
2. Perform the following:
   - Create a pivot table summarizing `Revenue_USD` by `Region` and `Main_Category`.
   - Add conditional formatting to highlight regions with total revenue > $15,000.
   - Use INDEX-MATCH to look up `Sub_Category` names for any given `Main_Category`.
3. Save your results as "Exam3_Excel_Output.xlsx".

---

### Task 2: Advanced SQL
1. Use the `Casino_Gaming_Data new.csv` and `Quality_of_Life.csv` datasets.
2. Write SQL queries to:
   - Perform an INNER JOIN between the datasets on `country_code`.
   - Retrieve `Licensee` names where `Total Gross Gaming Revenue` exceeds 30,000 and `Quality of Life Value` > 75.
   - Use GROUP BY and HAVING to show average `Patron Winnings` for each `Fiscal Year` where the average exceeds 100,000.
3. Save your queries in "Exam3_SQL_Queries.sql" and query results in "Exam3_SQL_Results.txt".

---

### Task 3: Python Transformation
1. Use the `retail_store_sales.csv` dataset.
2. Write a Python script to:
   - Fill missing values in `Price Per Unit` with the median price.
   - Create a new column `Total Revenue` (Price Per Unit × Quantity).
   - Filter rows where `Total Revenue` > 200 and save the results.
   - Create a bar chart showing `Category` vs. total `Revenue`.
3. Save your script as "Exam3_Python_Script.py".
4. Save the filtered dataset as "Exam3_Python_Output.csv".
5. Save the chart as "Exam3_Bar_Chart.png".
