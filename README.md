# MSCS 634 Lab 1: Data Visualization, Data Preprocessing, and Statistical Analysis Using Python

## Purpose

The purpose of this lab was to explore a dataset using Python and apply data visualization, preprocessing, and statistical analysis techniques in Jupyter Notebook. The lab provided hands-on experience working with real-world data using Pandas, Matplotlib, Seaborn, and Scikit-learn.

## Dataset

The Superstore Sales dataset was used for this lab. The dataset contains information about customer orders, sales, profit, product categories, discounts, and geographic locations.

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- GitHub

## Data Collection

The dataset was loaded into a Pandas DataFrame and examined using the `head()` function to verify successful import and understand the structure of the data.

## Data Visualization

Several visualizations were created to better understand the dataset:

### Bar Chart
The bar chart compared total sales across product categories. Technology and Office Supplies generated higher sales than Furniture.

### Histogram
The histogram showed the distribution of sales values. Most sales transactions were smaller amounts, while a smaller number of transactions represented larger sales values.

### Scatter Plot
The scatter plot displayed the relationship between sales and profit. A positive relationship was observed between higher sales and higher profit, although some high-sales transactions produced relatively low profits.

## Data Preprocessing

The following preprocessing techniques were applied:

### Missing Values
The dataset was checked for missing values using `isnull().sum()`. No missing values were identified.

### Outlier Detection and Removal
The Interquartile Range (IQR) method was used to identify outliers in the Sales column. Outliers were detected and removed to improve data quality.

### Data Reduction
Sampling was applied to reduce the dataset size, and less relevant identifier columns were removed to simplify analysis.

### Data Scaling and Discretization
Min-Max Scaling was performed on the Sales column to normalize values between 0 and 1. Sales values were also grouped into Low, Medium, and High categories using discretization.

## Statistical Analysis

### General Overview
The dataset was explored using `info()` and `describe()` to understand data types and summary statistics.

### Central Tendency Measures
The following measures were calculated:
- Minimum
- Maximum
- Mean
- Median
- Mode

### Measures of Dispersion
The following measures were calculated:
- Range
- Quartiles
- Interquartile Range (IQR)
- Variance
- Standard Deviation

### Correlation Analysis
A correlation matrix was generated to evaluate relationships between numerical variables in the dataset.

## Key Insights

- Technology and Office Supplies generated the highest sales.
- Sales values were heavily concentrated in lower ranges, with fewer large transactions.
- Outliers were present in the Sales column and were successfully identified using the IQR method.
- Sales and Profit showed a positive relationship.
- Scaling and discretization improved data consistency and made analysis easier.

## Challenges and Decisions

One challenge was ensuring the dataset loaded correctly because of file encoding issues. This was resolved by using the appropriate file encoding when importing the dataset. Since the dataset contained no missing values, data preprocessing focused primarily on outlier detection, reduction, scaling, and discretization techniques.

## Repository Contents

- Lab1.ipynb
- Sample - Superstore.csv
- screenshots folder
- README.md
