# Practice 4: Aggregating Data Using SQL

## Task:
Using **Dataset2.csv** (Product data), write SQL queries to:
1. Find the average price of products in each category.
2. Identify the product with the highest price in each category.

## SQL Queries to Write:
1. Find the average price by category:
   SELECT category, AVG(price)
   FROM products
   GROUP BY category;

2. Identify the highest price by category:
   SELECT category, MAX(price)
   FROM products
   GROUP BY category;
