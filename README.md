# Data Immersion & Wrangling - Task 1

## Overview

This project focuses on the initial stages of the data analytics workflow: understanding the dataset, assessing data quality, performing data cleaning, and preparing an analysis-ready dataset.

The dataset contains retail sales transaction records, including customer information, product details, and sales data. The objective is to identify data quality issues, apply appropriate cleaning techniques, and create additional features that can support future exploratory analysis and business intelligence tasks.

---

## Dataset Summary

* Total Records: 1000
* Total Features: 12
* Dataset Type: Retail Sales Transactions

### Original Features

* Order_ID
* Order_Date
* Customer_ID
* Customer_Name
* Age
* Gender
* City
* Product
* Category
* Quantity
* Unit_Price
* Total_Sales

---

## Data Dictionary

A detailed data dictionary is provided in the repository, describing:

* Feature names
* Data types
* Business meaning
* Analytical relevance

---

## Data Quality Assessment

### Missing Values Identified

| Column | Missing Values |
| ------ | -------------- |
| Age    | 20             |
| City   | 13             |

### Duplicate Records

* No duplicate records were found.

### Data Consistency Checks

* Gender values were consistent.
* Category values were standardized.
* City names showed no major formatting inconsistencies.

### Outlier Assessment

Numerical columns were analyzed using descriptive statistics:

* Age
* Quantity
* Unit_Price
* Total_Sales

The detected extreme values appeared to represent valid business transactions and were therefore retained.

---

## Data Cleaning Performed

### Missing Value Treatment

* Missing Age values were replaced using the median age.
* Missing City values were replaced using the most frequent city (mode).

### Data Type Conversion

* Order_Date was converted from object format to datetime format.

---

## Feature Engineering

The following new features were created to enhance analytical capabilities:

### Order_Month

Extracted the month from Order_Date to support monthly sales analysis.

### Order_Quarter

Extracted the quarter from Order_Date to support quarterly business reporting.

### Age_Group

Customers were categorized into:

* Young (< 25)
* Adult (25–44)
* Senior (45+)

### Revenue_Category

Orders were categorized based on Total_Sales:

* Low Revenue
* Medium Revenue
* High Revenue

---

## Final Output

The final cleaned dataset is analysis-ready and suitable for:

* Exploratory Data Analysis (EDA)
* Business Intelligence Reporting
* Dashboard Development
* Statistical Analysis
* Machine Learning Applications

---

## Repository Contents

```text
Data-Immersion-Wrangling-Task1/
│
├── Original_Dataset.xlsx
├── Cleaned_Sales_Dataset.xlsx
├── Data_Cleaning.ipynb
├── Data_Dictionary.md
└── README.md
```

---

## Tools & Technologies

* Python
* Pandas
* Jupyter Notebook / Google Colab
* Microsoft Excel
* GitHub

---

## Learning Outcomes

Through this task, the following skills were applied:

* Data Understanding
* Data Profiling
* Data Quality Assessment
* Data Cleaning
* Data Transformation
* Feature Engineering
* Dataset Preparation for Analytics

---
