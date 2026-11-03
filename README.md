# Customer Shopping Behavior Analysis

**Author:** Swayam Dalal

## Project Overview

This project explores customer shopping behavior using transactional data from **3,900 purchases**. It aims to uncover patterns in customer spending, product preferences, subscription status, and purchasing trends, then present the findings through SQL analysis and an interactive Power BI dashboard.

The workflow combines Python for data preparation, PostgreSQL for business-focused querying, and Power BI for visual reporting.

## Tools & Technologies

- **Python** — data cleaning, exploratory data analysis (EDA), and feature engineering
- **Pandas** — data manipulation and preprocessing
- **PostgreSQL** — storing the cleaned dataset and performing SQL analysis
- **SQL** — aggregations, comparisons, and customer segmentation
- **Power BI** — interactive dashboard and data visualization

## Dataset

The dataset contains **3,900 rows and 18 columns**, including:

- Customer details: age, gender, location, and subscription status
- Purchase information: item, category, purchase amount, season, size, and color
- Shopping behavior: discounts, promo codes, previous purchases, and purchase frequency
- Customer feedback and fulfilment: review ratings and shipping type

The `Review Rating` column contained 37 missing values, which were handled during data preparation.

## Project Workflow

### 1. Data Cleaning and Exploratory Analysis

Data preparation was performed in Python using Pandas.

- Inspected the dataset structure and descriptive statistics.
- Checked for missing values and imputed missing review ratings using the median rating of the corresponding product category.
- Standardized column names using `snake_case`.
- Created an `age_group` feature.
- Derived `purchase_frequency_days`.
- Checked for redundancy between discount and promo-code fields and removed the redundant `promo_code_used` column.
- Loaded the cleaned data into PostgreSQL for further analysis.

### 2. SQL Business Analysis

PostgreSQL queries were used to investigate ten business questions:

1. How does revenue compare across male and female customers?
2. Which customers used discounts but still spent above the average purchase amount?
3. Which five products have the highest average review ratings?
4. How do average purchase amounts compare across shipping types?
5. How do subscribers and non-subscribers compare in average spending and total revenue?
6. Which five products have the highest proportion of discounted purchases?
7. How can customers be grouped into New, Returning, and Loyal segments based on purchase history?
8. What are the top three most-purchased products in each category?
9. Are customers with more than five purchases more likely to subscribe?
10. How much revenue does each age group contribute?

### 3. Power BI Dashboard

An interactive dashboard was created in Power BI to present the analysis visually.

The dashboard includes:

- **KPI cards:** number of customers, average purchase amount, and average review rating.
- **Subscription status:** customer split between subscribers and non-subscribers.
- **Category analysis:** revenue and sales by product category.
- **Age-group analysis:** sales and revenue across customer age groups.
- **Interactive filters:** subscription status, gender, category, and shipping type.

## Business Recommendations

The analysis supports several potential business actions:

- Encourage subscription adoption through exclusive subscriber benefits.
- Strengthen customer loyalty initiatives to reward repeat purchases.
- Review discount strategies to balance sales and profitability.
- Promote highly rated and popular products.
- Focus marketing efforts on high-revenue age groups and relevant shipping preferences.

## Repository Contents

Organize the project files in this repository as follows (adjust the names to match the files you upload):

```text
Customer-Shopping-Behavior-Analysis/
├── README.md
├── dashboard.png
├── data/
│   └── shopping_behavior.csv
├── notebooks/
│   └── customer_shopping_behavior.ipynb
└── sql/
    └── customer_behavior_analysis.sql
```

## Key Skills Demonstrated

Data cleaning · Exploratory data analysis · Feature engineering · Python · Pandas · PostgreSQL · SQL · Customer segmentation · Power BI · Data visualization · Business analysis

## Author

**Swayam Dalal**
