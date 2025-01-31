# Day 2 Content: Inferential Statistics and Hypothesis Testing

## Overview
Inferential statistics allow us to make predictions or inferences about a population based on sample data. Today, you will learn about **hypothesis testing**, a key component of inferential statistics. You will also perform **t-tests** and **chi-square tests** to validate your findings.

---

## 1. What is Inferential Statistics?
Inferential statistics are used to:
- Draw conclusions about a population from a sample.
- Make predictions or generalizations based on data.
- Test hypotheses and validate assumptions.

### Why is Inferential Statistics Important?
- It helps us make data-driven decisions with confidence.
- It allows us to test theories and validate insights.
- It is widely used in research, business, and healthcare.

---

## 2. Hypothesis Testing
Hypothesis testing is a statistical method used to determine whether a hypothesis about a population parameter is supported by the data.

### 2.1 Null and Alternative Hypotheses
- **Null Hypothesis (H₀)**: The default assumption (e.g., no difference between groups).
- **Alternative Hypothesis (H₁)**: The hypothesis we want to test (e.g., there is a difference between groups).

### 2.2 Types of Hypothesis Tests
- **t-Test**: Used to compare the means of two groups.
- **Chi-Square Test**: Used to test relationships between categorical variables.

---

## 3. Performing a t-Test
A t-test is used to compare the means of two groups. There are three types:
1. **Independent t-Test**: Compares the means of two independent groups.
2. **Paired t-Test**: Compares the means of the same group at two different times.
3. **One-Sample t-Test**: Compares the mean of a single group to a known value.

### Steps to Perform a t-Test:
1. Formulate the null and alternative hypotheses.
2. Choose a significance level (e.g., α = 0.05).
3. Calculate the t-statistic and p-value.
4. Interpret the results:
   - If p-value < α, reject the null hypothesis.
   - If p-value ≥ α, fail to reject the null hypothesis.

---

## 4. Performing a Chi-Square Test
A chi-square test is used to test relationships between categorical variables. There are two types:
1. **Chi-Square Test of Independence**: Tests if two categorical variables are independent.
2. **Chi-Square Goodness-of-Fit Test**: Tests if observed frequencies match expected frequencies.

### Steps to Perform a Chi-Square Test:
1. Formulate the null and alternative hypotheses.
2. Choose a significance level (e.g., α = 0.05).
3. Calculate the chi-square statistic and p-value.
4. Interpret the results:
   - If p-value < α, reject the null hypothesis.
   - If p-value ≥ α, fail to reject the null hypothesis.

---

## 5. Applications of Hypothesis Testing
Hypothesis testing is used in various fields:
- **Business**: Testing the effectiveness of marketing campaigns.
- **Healthcare**: Comparing the effectiveness of treatments.
- **Education**: Evaluating the impact of teaching methods.

---

## 6. Practice Exercises
Today, you will work with three datasets to apply what you've learned. Each dataset is designed for specific practices:

### Dataset 1: Sales Performance (`Dataset1.csv`)
- **Description**: Contains sales data for two regions (Region A and Region B).
- **Practices**: Practice 1, Practice 3.

### Dataset 2: Customer Satisfaction (`Dataset2.csv`)
- **Description**: Contains customer satisfaction scores for two products (Product X and Product Y).
- **Practices**: Practice 2, Practice 4.

### Dataset 3: Employee Performance (`Dataset3.csv`)
- **Description**: Contains employee performance ratings and training program participation.
- **Practices**: Practice 5, Practice 6.

---

## 7. Practice Tasks
### Practice 1: Independent t-Test for Sales Performance
- **Dataset**: `Dataset1.csv`
- **Task**: Perform an independent t-test to compare the mean sales of Region A and Region B.

### Practice 2: Chi-Square Test for Customer Satisfaction
- **Dataset**: `Dataset2.csv`
- **Task**: Perform a chi-square test to determine if there is a relationship between product type and customer satisfaction.

### Practice 3: Paired t-Test for Sales Performance
- **Dataset**: `Dataset1.csv`
- **Task**: Perform a paired t-test to compare the mean sales of Region A before and after a marketing campaign.

### Practice 4: Chi-Square Test for Product Preference
- **Dataset**: `Dataset2.csv`
- **Task**: Perform a chi-square test to determine if there is a relationship between product type and customer preference.

### Practice 5: One-Sample t-Test for Employee Performance
- **Dataset**: `Dataset3.csv`
- **Task**: Perform a one-sample t-test to compare the mean performance rating of employees to a benchmark value of 4.0.

### Practice 6: Hypothesis Testing Report
- **Dataset**: `Dataset3.csv`
- **Task**: Write a report summarizing the results of all hypothesis tests performed today.

---

## 8. Advanced Reading
For further learning:
- [Hypothesis Testing in Python](https://realpython.com/python-statistics/)
- [Understanding Hypothesis Testing](https://towardsdatascience.com/understanding-hypothesis-testing)