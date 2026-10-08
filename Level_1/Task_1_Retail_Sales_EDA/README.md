# Retail Sales Data Analysis & EDA

**Internship:** Oasis Infobyte – AICTE Data Analytics Internship
**Task:** Level 1 – Task 1
**Name:** Prajwal Poojary

---

## Project Overview

This project performs Exploratory Data Analysis (EDA) on a retail sales dataset to understand sales trends, customer demographics, product category performance, and relationships between numerical variables.

The analysis aims to identify meaningful patterns and generate actionable business insights from the available sales data.

## Objectives

* Understand the structure and quality of the dataset.
* Calculate descriptive statistics for numerical variables.
* Analyze monthly and quarterly sales trends.
* Study customer distribution by age group and gender.
* Analyze revenue performance by product category.
* Examine correlations between numerical variables.
* Identify additional customer spending patterns.
* Provide actionable business recommendations.

## Dataset

The dataset contains **1,000 retail transactions** and **9 original columns**:

* Transaction ID
* Date
* Customer ID
* Gender
* Age
* Product Category
* Quantity
* Price per Unit
* Total Amount

The dataset covers transactions from **January 2023 to January 2024**.

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Data Preparation

The following data-quality checks and preparation steps were performed:

* Checked dataset shape and column names.
* Checked data types.
* Checked for missing values.
* Checked for duplicate records.
* Converted the Date column into datetime format.
* Created age groups for customer demographic analysis.

The dataset contained **no missing values and no duplicate records**.

## Analysis Performed

### 1. Descriptive Statistics

Calculated:

* Mean
* Median
* Mode
* Standard deviation

for:

* Age
* Quantity
* Price per Unit
* Total Amount

### 2. Monthly Sales Trend

Monthly sales were analyzed to identify changes in revenue throughout the year.

**Key finding:** May 2023 recorded the highest monthly sales at **53,150**, while September 2023 recorded the lowest at **23,620** among the full months of 2023.

### 3. Quarterly Sales Trend

Quarterly sales were analyzed to identify broader sales patterns.

**Key finding:** Q4 2023 recorded the highest complete-quarter sales at **126,190**, followed by Q2 2023 with **123,735**.

### 4. Customer Demographics

Customer distribution was analyzed using age groups and gender.

The largest age group was **46–55**, with **229 customers**.

Gender distribution was relatively balanced:

* Female: **510**
* Male: **490**

### 5. Revenue by Product Category

Revenue was compared across the available product categories.

| Product Category | Revenue |
| ---------------- | ------: |
| Electronics      | 156,905 |
| Clothing         | 155,580 |
| Beauty           | 143,515 |

**Key finding:** Electronics generated the highest revenue, although Clothing performed very closely.

### 6. Correlation Analysis

A correlation heatmap was created for the main numerical variables.

Important relationships included:

* Price per Unit vs Total Amount: **0.85**
* Quantity vs Total Amount: **0.37**
* Age vs Total Amount: **-0.06**

The strongest relationship was between **Price per Unit and Total Amount**.

### 7. Average Transaction Value by Age Group

An additional analysis was performed to compare average transaction value across age groups.

The results showed:

* 18–25: **500.30**
* 26–35: **480.39**
* 36–45: **454.80**
* 46–55: **439.69**
* 56–64: **412.36**

The analysis suggests that younger customers in this dataset tend to have higher average transaction values.

## Key Business Insights

1. Sales fluctuate considerably across different months and quarters.
2. Q4 2023 was the strongest complete quarter.
3. Electronics generated the highest category revenue.
4. Customer distribution was relatively balanced across gender and age groups.
5. Price per Unit has a strong positive relationship with Total Amount.
6. Younger customer groups showed higher average transaction values in this dataset.

## Business Recommendations

1. **Focus on high-performing categories:** Maintain strong inventory and promotional strategies for Electronics while exploring ways to improve lower-performing categories.

2. **Target younger customers:** Test targeted promotions, product bundles, and digital campaigns for younger customer segments because they showed higher average transaction values.

3. **Use pricing and quantity strategies:** Evaluate higher-value products and consider bundle or multi-unit promotions to encourage larger purchases.

4. **Plan around sales trends:** Prepare inventory and marketing campaigns ahead of historically stronger periods such as Q4 and high-performing months.

5. **Improve product-level data collection:** Record individual product names and product-level sales information to enable more detailed analysis of top-selling products.

## Dataset Limitation

The dataset contains **Product Category** information but does not contain individual **Product Name** information.

Therefore, a genuine **Top 10 Best-Selling Products** analysis could not be performed without introducing unsupported or fabricated data. Instead, this project performs a category-level revenue analysis.

The dataset also contains only a small amount of data for January 2024, so January 2024 should not be directly compared with the complete months of 2023.

## Project Structure

```text
Task_1_Retail_Sales_EDA/
│
├── PrajwalPoojary_Task1.ipynb
├── retail_sales_dataset.csv
└── README.md
```

## How to Run

1. Open the Jupyter Notebook:
   `PrajwalPoojary_Task1.ipynb`
2. Make sure `retail_sales_dataset.csv` is in the same folder as the notebook.
3. Run the notebook cells from top to bottom.
4. The analysis, visualizations, observations, and conclusions will be generated.

## Conclusion

This project demonstrates the use of Python-based exploratory data analysis to understand retail sales performance and customer behavior.

The analysis identified important sales trends, category performance, customer demographic patterns, and relationships between transaction variables. These findings can help businesses improve inventory planning, customer targeting, pricing strategies, and promotional decisions.

---

**Author:** Prajwal Poojary
