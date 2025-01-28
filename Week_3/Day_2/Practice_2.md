# Practice 2: Identifying and Correcting Data Inconsistencies in SQL

## Task:
Using **Dataset2.csv** (Product data), you will write SQL queries to:
1. Find all duplicate product entries based on product name.
2. Correct inconsistent product names by updating them to the correct format.

## SQL Queries to Write:
1. Find duplicates:
   SELECT product_name, COUNT(*)
   FROM products
   GROUP BY product_name
   HAVING COUNT(*) > 1;

2. Correct inconsistencies:
   UPDATE products
   SET product_name = 'Correct Product Name'
   WHERE product_name = 'Incorrect Product Name';
