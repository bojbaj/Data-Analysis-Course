# Week 1 Exam: Medium Level

## Objective
Test your ability to clean, query, and analyze data using intermediate-level Excel, SQL, and Python techniques.

---

### Task 1: Advanced Excel
1. Use the `shoes_dim.csv` dataset.
2. Perform the following:
   - Use VLOOKUP to map `best_for_wear` descriptions to predefined categories:
     - City: Urban Wear
     - Running: Sports Wear
     - Sport: General Sports.
   - Highlight rows where `dominant_color` is "Black".
3. Save the updated dataset as "Exam2_Excel_Output.xlsx".

---

### Task 2: Intermediate SQL
1. Use the `Casino_Gaming_Data new.csv` dataset.
2. Write SQL queries to:
   - Calculate total `Wagers` grouped by `Licensee`.
   - Retrieve `Licensee` names with total `Cancelled Wagers` > 10.
3. Save your queries in "Exam2_SQL_Queries.sql" and query results in "Exam2_SQL_Results.txt".

---

### Task 3: Python Cleaning
1. Use the `cleveland2.csv` dataset.
2. Write a Python script to:
   - Replace missing values in `chol` with the median.
   - Create a new column `cholesterol_category`:
     - High if `chol` > 240.
     - Medium if `200 <= chol <= 240`.
     - Low otherwise.
   - Save the updated dataset as "Exam2_Python_Output.csv".
3. Save your Python script as "Exam2_Python_Script.py".
