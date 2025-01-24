# Day 4 Content: Advanced Python Visualization with Matplotlib and Seaborn

## Overview
Today, you will take your Python visualization skills to the next level by learning advanced customization and leveraging the **Seaborn** library for beautiful and informative visualizations. Seaborn extends Matplotlib's capabilities, making it easier to create aesthetically pleasing charts.

By the end of this lesson, you will:
1. Understand how to customize plots extensively using Matplotlib.
2. Use Seaborn to create advanced visualizations like heatmaps, pair plots, and box plots.
3. Combine Matplotlib and Seaborn for fine-tuned visualizations.

---

## 1. Advanced Customizations in Matplotlib

### 1.1 Subplots
Subplots allow you to display multiple charts in a single figure.

#### Steps:
1. Import Matplotlib:
   import matplotlib.pyplot as plt
2. Create subplots:
   fig, ax = plt.subplots(1, 2, figsize=(10, 5)) # 1 row, 2 columns
3. Add data to each subplot:
   ax[0].bar(['A', 'B', 'C'], [10, 20, 30])
   ax[1].plot([1, 2, 3], [30, 20, 10])
4. Add titles to each subplot:
   ax[0].set_title('Bar Chart')
   ax[1].set_title('Line Chart')
5. Display the figure:
   plt.show()

---

### 1.2 Advanced Styling
You can customize your chart's style with the following:
- Change fonts:
   plt.rc('font', family='Arial')
- Add annotations:
   plt.annotate('Peak', xy=(2, 30), xytext=(1.5, 35),
                arrowprops=dict(facecolor='black', arrowstyle='->'))
- Use themes:
   plt.style.use('ggplot')

---

## 2. Introduction to Seaborn
Seaborn is a Python data visualization library built on top of Matplotlib. It simplifies creating complex visualizations.

### 2.1 Importing Seaborn
Install and import Seaborn:
   pip install seaborn
   import seaborn as sns

---

### 2.2 Creating Heatmaps
Heatmaps are used to visualize data intensity across a grid.

#### Example:
1. Import your dataset:
   import pandas as pd
   data = pd.read_csv('Adidas_Sales_Data.csv')
2. Reshape the data for a heatmap:
   pivot_table = data.pivot('Month', 'Region', 'Total Sales')
3. Create the heatmap:
   sns.heatmap(pivot_table, annot=True, cmap='coolwarm')
4. Display the chart:
   plt.show()

---

### 2.3 Pair Plots
Pair plots show relationships between numerical variables in a dataset.

#### Example:
1. Import the dataset:
   data = pd.read_csv('Adidas_Sales_Data.csv')
2. Create a pair plot:
   sns.pairplot(data)
3. Display the plot:
   plt.show()

---

### 2.4 Box Plots
Box plots summarize data distributions and detect outliers.

#### Example:
1. Import the dataset:
   data = pd.read_csv('Adidas_Sales_Data.csv')
2. Create a box plot for `Profit Margin` by `Region`:
   sns.boxplot(x='Region', y='Profit Margin', data=data)
3. Display the chart:
   plt.show()

---

## 3. Combining Matplotlib and Seaborn
You can enhance Seaborn visualizations by adding Matplotlib customizations.

#### Example:
1. Create a Seaborn bar chart:
   sns.barplot(x='Region', y='Total Sales', data=data)
2. Add a Matplotlib annotation:
   plt.annotate('Highest Sales', xy=(1, 60000), xytext=(1, 70000),
                arrowprops=dict(facecolor='green', shrink=0.05))
3. Display the chart:
   plt.show()

---

## 4. Common Pitfalls in Advanced Visualization
1. **Overloading Charts**:
   - Avoid visualizing too much data in one chart.
   - Focus on key insights.
2. **Inconsistent Styles**:
   - Use consistent colors and fonts across visualizations.
3. **Ignoring Interactivity**:
   - Consider tools like Plotly or Dash for interactive visualizations.

---

## 5. Practice Exercises
- **Practice 1**: Create subplots with bar and line charts.
- **Practice 2**: Create a heatmap showing `Total Sales` by `Month` and `Region`.
- **Practice 3**: Generate a pair plot for the entire dataset.
- **Practice 4**: Create a box plot for `Profit Margin` by `Region`.
- **Practice 5**: Combine Matplotlib and Seaborn to create a customized bar chart.
- **Practice 6**: Save a Seaborn heatmap as an image file.

---

## 6. Advanced Reading
For further learning:
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Advanced Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/index.html)

---

## Summary
Advanced Python visualization techniques using Matplotlib and Seaborn can elevate your data storytelling. Practice creating and customizing visualizations to build confidence in using these tools.
