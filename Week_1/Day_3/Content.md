# Day 3 Content: Python Basics for Data Analysis

## Overview
Python is a versatile tool for data analysis. Today, you'll learn:
1. How to load and explore datasets.
2. Basic cleaning techniques.
3. Filtering and transforming data.

---

### 1. Loading Data with pandas
```python
import pandas as pd

# Load a CSV file
df = pd.read_csv('cleveland1.csv')
print(df.head())
