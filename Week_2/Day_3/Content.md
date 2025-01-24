# Day 3 Content: Introduction to Python Visualization with Matplotlib and Pandas

## Overview
Python is one of the most versatile tools for data visualization, offering libraries like **Matplotlib** and **Pandas**. Today, you'll learn how to create various charts and customize them using Python. These skills are essential for building dynamic and scalable visualizations.

By the end of this lesson, you will:
1. Understand the basics of Matplotlib and Pandas plotting capabilities.
2. Create bar, line, and scatter plots in Python.
3. Customize visualizations with titles, labels, and styles.
4. Save visualizations as images for reports.

---

## 1. Why Use Python for Visualization?
While tools like Excel are great for quick visualizations, Python offers:
- **Scalability**: Handle large datasets efficiently.
- **Flexibility**: Customize every aspect of your charts.
- **Automation**: Create reproducible visualizations in scripts.
- **Integration**: Combine visualizations with data processing.

---

## 2. Getting Started with Matplotlib
Matplotlib is the foundational library for data visualization in Python. It allows you to create static, interactive, and animated visualizations.

### 2.1 Importing Matplotlib
To use Matplotlib, import it as follows:
import matplotlib.pyplot as plt

---

### 2.2 Creating a Simple Bar Chart
Bar charts are used to compare categorical data.

Steps:
1. Prepare your data:
   regions = ['North America', 'Europe', 'Asia']
   sales = [50000, 45000, 40000]
2. Plot the bar chart:
   plt.bar(regions, sales)
3. Add labels and a title:
   plt.title('Total Sales by Region')
   plt.xlabel('Region')
   plt.ylabel('Total Sales')
4. Display the chart:
   plt.show()

---

### 2.3 Creating a Line Chart
Line charts are ideal for showing trends over time.

Steps:
1. Prepare your data:
   months = ['January', 'February', 'March']
   sales = [50000, 55000, 60000]
2. Plot the line chart:
   plt.plot(months, sales, marker='o')
3. Customize the chart:
   - Add gridlines:
     plt.grid(True)
   - Add labels and a title:
     plt.title('Monthly Sales Trend')
     plt.xlabel('Month')
     plt.ylabel('Total Sales')
4. Display the chart:
   plt.show()

---

### 2.4 Creating a Scatter Plot
Scatter plots are used to show relationships between two numerical variables.

Steps:
1. Prepare your data:
   ages = [25, 30, 35, 40, 45]
   transaction_values = [200, 250, 300, 350, 400]
2. Plot the scatter chart:
   plt.scatter(ages, transaction_values, color='green')
3. Add labels and a title:
   plt.title('Age vs Transaction Value')
   plt.xlabel('Age')
   plt.ylabel('Transaction Value')
4. Display the chart:
   plt.show()

---

## 3. Plotting with Pandas
Pandas provides a simpler way to create plots directly from dataframes.

### Example: Bar Chart
Steps:
1. Import the data:
   import pandas as pd
   data = pd.read_csv('Adidas_Sales_Data.csv')
2. Plot the bar chart:
   data.groupby('Region')['Total Sales'].sum().plot(kind='bar', title='Total Sales by Region')
3. Customize the chart:
   plt.xlabel('Region')
   plt.ylabel('Total Sales')
4. Display the chart:
   plt.show()

---

## 4. Customizing Charts
Customizations make your charts more informative and visually appealing.

### Adding Titles and Labels
Use the following functions:
- plt.title('Chart Title')
- plt.xlabel('X-axis Label')
- plt.ylabel('Y-axis Label')

### Changing Colors
Specify colors for your plots:
- Bar chart: plt.bar(x, y, color='skyblue')
- Line chart: plt.plot(x, y, color='red')

### Saving Charts
Save your chart as an image:
- plt.savefig('chart.png')

---

## 5. Common Mistakes in Python Visualization
1. **Overcrowding the Chart**:
   - Avoid plotting too many data points at once.
   - Use subplots if necessary.
2. **Ignoring Labels**:
   - Always label axes and add a title.
3. **Default Styles**:
   - Customize styles to make charts stand out.

---

## 6. Practice Exercises
- **Practice 1**: Create a bar chart showing `Total Sales` by `Region` using Matplotlib.
- **Practice 2**: Create a line chart showing `Monthly Sales Trend` using Matplotlib.
- **Practice 3**: Create a scatter plot showing `Age` vs `Transaction Value` using Matplotlib.
- **Practice 4**: Use Pandas to create a bar chart for `Total Sales` by `Region`.
- **Practice 5**: Customize a chart with titles, labels, and gridlines.
- **Practice 6**: Save a chart as an image file.

---

## 7. Advanced Reading
For further learning:
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- [Pandas Visualization](https://pandas.pydata.org/docs/user_guide/visualization.html)

---

## Summary
Python is a powerful tool for creating dynamic and scalable visualizations. By combining Matplotlib and Pandas, you can build charts tailored to your data analysis needs. Practice creating and customizing charts to reinforce your skills.
