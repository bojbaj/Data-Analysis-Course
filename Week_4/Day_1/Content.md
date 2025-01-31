# Day 1 Content: Introduction to Descriptive Statistics

## Overview
Descriptive statistics are the foundation of data analysis. They help us summarize and understand the main features of a dataset. Today, you will learn about **measures of central tendency** (mean, median, mode) and **measures of dispersion** (variance, standard deviation). By the end of the day, you will be able to calculate these metrics and interpret their meaning in real-world datasets.

---

## 1. What are Descriptive Statistics?
Descriptive statistics are used to:
- Summarize large datasets into key metrics.
- Provide insights into the distribution of data.
- Identify patterns, trends, and outliers.

### Why are Descriptive Statistics Important?
- They help us understand the data before applying more complex analyses.
- They provide a clear picture of the dataset's characteristics.
- They are essential for making data-driven decisions.

---

## 2. Measures of Central Tendency
Measures of central tendency describe the **center** of a dataset. They help us understand where most of the data points lie.

### 2.1 Mean
- The **mean** is the average of all data points.
- Formula:  
  \[
  \text{Mean} = \frac{\sum_{i=1}^{n} x_i}{n}
  \]
- Example: If the sales values are [100, 200, 300], the mean is (100 + 200 + 300) / 3 = 200.

### 2.2 Median
- The **median** is the middle value when the data is sorted in ascending or descending order.
- If the dataset has an even number of observations, the median is the average of the two middle values.
- Example: For the dataset [100, 200, 300], the median is 200. For [100, 200, 300, 400], the median is (200 + 300) / 2 = 250.

### 2.3 Mode
- The **mode** is the value that appears most frequently in the dataset.
- Example: For the dataset [100, 200, 200, 300], the mode is 200.

---

## 3. Measures of Dispersion
Measures of dispersion describe how **spread out** the data is. They help us understand the variability in the dataset.

### 3.1 Variance
- **Variance** measures how far each number in the dataset is from the mean.
- Formula:  
  \[
  \text{Variance} = \frac{\sum_{i=1}^{n} (x_i - \text{Mean})^2}{n}
  \]
- Example: For the dataset [100, 200, 300], the variance is calculated as follows:
  - Mean = 200
  - Variance = [(100-200)² + (200-200)² + (300-200)²] / 3 = (10000 + 0 + 10000) / 3 = 6666.67

### 3.2 Standard Deviation
- **Standard deviation** is the square root of the variance.
- It provides a measure of the average distance from the mean.
- Formula:  
  \[
  \text{Standard Deviation} = \sqrt{\text{Variance}}
  \]
- Example: For the dataset [100, 200, 300], the standard deviation is √6666.67 ≈ 81.65.

---

## 4. Applications of Descriptive Statistics
Descriptive statistics are used in various fields:
- **Business**: Summarizing sales data, analyzing customer behavior.
- **Healthcare**: Understanding patient data, analyzing treatment outcomes.
- **Education**: Summarizing student performance, analyzing test scores.

---

## 5. Practice Exercises
Today, you will work with three datasets to apply what you've learned. Each dataset is designed for specific practices:

### Dataset 1: Sales Data (`Dataset1.csv`)
- **Description**: Contains sales data with columns like `Region`, `Sales`, `Profit`, and `Quantity`.
- **Practices**: Practice 1, Practice 2, Practice 3.

### Dataset 2: Customer Feedback Data (`Dataset2.csv`)
- **Description**: Contains customer feedback scores and demographic information.
- **Practices**: Practice 4, Practice 5.

### Dataset 3: Product Performance Data (`Dataset3.csv`)
- **Description**: Contains product performance metrics like `Price`, `Sales`, and `Customer Rating`.
- **Practices**: Practice 6.

---

## 6. Practice Tasks
### Practice 1: Calculating Mean, Median, and Mode
- **Dataset**: `Dataset1.csv`
- **Task**: Calculate the mean, median, and mode for the `Sales` column.

### Practice 2: Calculating Variance and Standard Deviation
- **Dataset**: `Dataset1.csv`
- **Task**: Calculate the variance and standard deviation for the `Profit` column.

### Practice 3: Summarizing the Quantity Column
- **Dataset**: `Dataset1.csv`
- **Task**: Summarize the `Quantity` column using descriptive statistics (mean, median, mode, variance, standard deviation).

### Practice 4: Comparing Feedback Scores Across Demographics
- **Dataset**: `Dataset2.csv`
- **Task**: Compare the central tendency and dispersion of `Feedback Score` across different demographic groups.

### Practice 5: Identifying Outliers in Feedback Scores
- **Dataset**: `Dataset2.csv`
- **Task**: Identify outliers in the `Feedback Score` column using standard deviation.

### Practice 6: Creating a Summary Report for Product Performance
- **Dataset**: `Dataset3.csv`
- **Task**: Create a summary report for the entire dataset, including mean, median, mode, variance, and standard deviation for all numerical columns.

---

## 7. Advanced Reading
For further learning:
- [Descriptive Statistics in Python](https://realpython.com/python-statistics/)
- [Understanding Descriptive Statistics](https://towardsdatascience.com/understanding-descriptive-statistics)