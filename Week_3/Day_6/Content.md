# Day 6 Content: Data Visualization with Python

## Overview
Today, we focus on data visualization techniques using Python. You will learn how to create various types of charts and graphs to represent data visually. By the end of the day, you will be able to use Python libraries like Matplotlib and Seaborn to create insightful visualizations.

---

## 1. Why Use Python for Data Visualization?
Python is a versatile tool for data visualization because it allows you to:
- Create a wide range of charts and graphs.
- Customize visualizations to suit your needs.
- Automate the creation of visualizations using scripts.
- Integrate with other data analysis tools and libraries.

---

## 2. Creating Basic Charts with Matplotlib
Matplotlib is a foundational library for data visualization in Python. It allows you to create static, interactive, and animated visualizations.

### 2.1 Bar Charts
Bar charts are used to compare categorical data. Steps to create a bar chart:
- Prepare your data: Create lists or arrays for the categories and values.
- Use the `plt.bar()` function to create the bar chart.
- Customize the chart with titles, labels, and colors.

### 2.2 Line Charts
Line charts are ideal for showing trends over time. Steps to create a line chart:
- Prepare your data: Create lists or arrays for the x-axis (time) and y-axis (values).
- Use the `plt.plot()` function to create the line chart.
- Customize the chart with markers, gridlines, and annotations.

### 2.3 Scatter Plots
Scatter plots are used to show relationships between two numerical variables. Steps to create a scatter plot:
- Prepare your data: Create lists or arrays for the x-axis and y-axis.
- Use the `plt.scatter()` function to create the scatter plot.
- Customize the chart with colors, sizes, and labels.

---

## 3. Creating Advanced Charts with Seaborn
Seaborn is a Python library built on top of Matplotlib that provides high-level functions for creating advanced visualizations.

### 3.1 Heatmaps
Heatmaps are used to visualize data intensity across a grid. Steps to create a heatmap:
- Prepare your data: Create a pivot table or correlation matrix.
- Use the `sns.heatmap()` function to create the heatmap.
- Customize the heatmap with annotations and color palettes.

### 3.2 Box Plots
Box plots summarize data distributions and detect outliers. Steps to create a box plot:
- Prepare your data: Use a DataFrame with numerical and categorical columns.
- Use the `sns.boxplot()` function to create the box plot.
- Customize the box plot with titles and labels.

### 3.3 Pair Plots
Pair plots show relationships between numerical variables in a dataset. Steps to create a pair plot:
- Prepare your data: Use a DataFrame with numerical columns.
- Use the `sns.pairplot()` function to create the pair plot.
- Customize the pair plot with colors and markers.

---

## 4. Customizing Visualizations
Customizations make your visualizations more informative and visually appealing. Techniques include:

### 4.1 Adding Titles and Labels
- Use the `plt.title()`, `plt.xlabel()`, and `plt.ylabel()` functions to add titles and labels.

### 4.2 Changing Colors
- Use the `color` parameter in chart functions to change colors.

### 4.3 Saving Visualizations
- Use the `plt.savefig()` function to save your visualizations as image files.

---

## 5. Practice Exercises
Use the provided datasets to complete the following tasks:
- Practice 1: Create a bar chart showing total sales by region.
- Practice 2: Create a line chart showing monthly sales trends.
- Practice 3: Create a scatter plot showing the relationship between price and quantity.
- Practice 4: Create a heatmap showing sales by region and month.
- Practice 5: Create a box plot showing the distribution of prices by category.
- Practice 6: Create a pair plot for numerical columns in the dataset.

---

## 6. Advanced Reading
For further learning:
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- [Seaborn Documentation](https://seaborn.pydata.org/)