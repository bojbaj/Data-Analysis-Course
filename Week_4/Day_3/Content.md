# Day 3 Content: Correlation and Regression Analysis

## Overview
Correlation and regression analysis are essential tools for understanding relationships between variables. Today, you will learn how to calculate **correlation coefficients**, perform **linear regression**, and interpret the results. These techniques are widely used in fields like finance, healthcare, and marketing to make data-driven decisions.

---

## 1. What is Correlation?
Correlation measures the strength and direction of the relationship between two variables. It ranges from **-1 to 1**:
- **1**: Perfect positive correlation.
- **-1**: Perfect negative correlation.
- **0**: No correlation.

### 1.1 Pearson Correlation Coefficient
- The Pearson correlation coefficient is the most common measure of correlation.
- Formula:  
  \[
  r = \frac{\sum{(x_i - \bar{x})(y_i - \bar{y})}}{\sqrt{\sum{(x_i - \bar{x})^2} \sum{(y_i - \bar{y})^2}}}
  \]
- Example: If `Sales` and `Profit` have a correlation of 0.85, it means they are strongly positively correlated.

---

## 2. What is Regression Analysis?
Regression analysis is used to model the relationship between a dependent variable (target) and one or more independent variables (predictors). The most common type is **linear regression**.

### 2.1 Simple Linear Regression
- Models the relationship between two variables using a straight line.
- Formula:  
  \[
  y = mx + b
  \]
  - \( y \): Dependent variable.
  - \( x \): Independent variable.
  - \( m \): Slope of the line.
  - \( b \): Y-intercept.

### 2.2 Interpreting Regression Results
- **Slope (m)**: Indicates the change in the dependent variable for a one-unit change in the independent variable.
- **R-squared**: Measures how well the regression line fits the data (ranges from 0 to 1).

---

## 3. Applications of Correlation and Regression
- **Finance**: Predicting stock prices based on historical data.
- **Healthcare**: Analyzing the relationship between patient age and treatment outcomes.
- **Marketing**: Understanding the impact of advertising spend on sales.

---

## 4. Practice Exercises
Today, you will work with three datasets to apply what you've learned. Each dataset is designed for specific practices:

### Dataset 1: Sales and Profit Data (`Dataset1.csv`)
- **Description**: Contains sales and profit data for different regions.
- **Practices**: Practice 1, Practice 2.

### Dataset 2: Advertising and Sales Data (`Dataset2.csv`)
- **Description**: Contains advertising spend and sales data for different products.
- **Practices**: Practice 3, Practice 4.

### Dataset 3: Housing Price Data (`Dataset3.csv`)
- **Description**: Contains housing prices and features like square footage and number of bedrooms.
- **Practices**: Practice 5, Practice 6.

---

## 5. Practice Tasks
### Practice 1: Calculating Correlation
- **Dataset**: `Dataset1.csv`
- **Task**: Calculate the correlation between `Sales` and `Profit`.

### Practice 2: Performing Simple Linear Regression
- **Dataset**: `Dataset1.csv`
- **Task**: Perform a simple linear regression to predict `Profit` based on `Sales`.

### Practice 3: Creating a Correlation Matrix
- **Dataset**: `Dataset2.csv`
- **Task**: Create a correlation matrix for all numerical columns.

### Practice 4: Performing Multiple Linear Regression
- **Dataset**: `Dataset2.csv`
- **Task**: Perform multiple linear regression to predict `Sales` based on `Advertising Spend` and `Product Category`.

### Practice 5: Predicting Housing Prices
- **Dataset**: `Dataset3.csv`
- **Task**: Perform linear regression to predict `Price` based on `Square Footage` and `Bedrooms`.

### Practice 6: Creating a Summary Report
- **Dataset**: `Dataset3.csv`
- **Task**: Create a summary report of your regression analysis, including R-squared and predictions.

---

## 6. Advanced Reading
For further learning:
- [Correlation and Regression in Python](https://realpython.com/linear-regression-in-python/)
- [Understanding R-squared](https://towardsdatascience.com/understanding-r-squared)