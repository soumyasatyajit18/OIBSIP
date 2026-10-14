# Retail Sales Data — Exploratory Data Analysis (EDA)

## Project Overview

This project explores a retail sales dataset using Python to understand sales trends, customer demographics, product/category performance, and relationships between numerical variables. The analysis follows a typical data analyst workflow: load, inspect, clean, summarize, visualize, and translate findings into business recommendations.

## Objectives

- Inspect dataset dimensions, data types, missing values, and duplicate records.
- Calculate descriptive statistics for numerical variables.
- Analyze monthly and quarterly sales trends.
- Explore customer age-group and gender distributions.
- Identify the top 10 products or product categories by sales value.
- Compare revenue across product categories.
- Examine correlations between numerical variables.
- Compare average transaction value across age groups and gender.
- Summarize key business metrics and propose actionable recommendations.

## Tools and Libraries

- **Python**
- **Pandas** — data loading, cleaning, grouping, and aggregation
- **NumPy** — numerical operations
- **Matplotlib** — charts and trend visualizations
- **Seaborn** — statistical visualizations and heatmaps
- **Jupyter Notebook** — interactive analysis

## Dataset

The notebook is configured to read a CSV file named `Retail Sales Dataset.csv`. Place the dataset in the same directory as the notebook, or update `FILE_PATH` in the first code cell to point to its location.

The notebook is designed for transaction-level retail data with fields such as:

- Date or transaction date
- Customer ID
- Gender
- Age
- Product category or product name
- Quantity
- Price per unit
- Total amount / sales

The exact columns depend on the CSV provided. The notebook checks for several alternative column names, but the dataset must include a usable date field and a sales field for the monthly and quarterly trend analyses.

## Analysis Workflow

1. **Initial inspection:** Review dataset shape, column data types, missing values, and duplicate rows.
2. **Data preparation:** Standardize column names and convert the detected date column to datetime format.
3. **Descriptive statistics:** Calculate mean, median, mode, and standard deviation for numerical columns.
4. **Sales trends:** Aggregate sales by month and quarter.
5. **Customer segmentation:** Visualize age-group and gender distributions.
6. **Product and category performance:** Rank the top 10 available product-level groups and compare revenue by category.
7. **Correlation analysis:** Use a heatmap to explore linear relationships between numerical variables.
8. **Average spend analysis:** Compare average transaction value by age group and gender when the required columns are available.
9. **KPI summary:** Calculate total sales, number of transactions, average transaction value, and total units sold when quantity is available.
10. **Business recommendations:** Use the observed charts and metrics to guide inventory planning, promotions, and customer targeting.

## Getting Started

### 1. Clone or download the project

Download this repository or place the notebook and dataset in a project folder.

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Add the dataset

Place `Retail Sales Dataset.csv` beside `Retail_Sales_EDA_Task1.ipynb`, or change the `FILE_PATH` variable in the notebook.

### 4. Run the notebook

```bash
jupyter notebook Retail_Sales_EDA_Task1.ipynb
```

Run the cells from top to bottom.

## Key Metrics

The notebook calculates these metrics where the necessary fields are available:

- **Total Sales:** Sum of the selected sales column.
- **Transactions:** Number of rows in the dataset.
- **Average Transaction Value:** Mean value of the selected sales column.
- **Total Units Sold:** Sum of the quantity column, if present.

## Business Questions

- How do sales change month to month and quarter to quarter?
- Which customer age groups account for the most transactions?
- How is the transaction base distributed by gender?
- Which products or product groups contribute the most sales value?
- Which product categories generate the most revenue?
- Which numerical variables have strong linear relationships?
- Do average transaction values vary across age and gender segments?


## Repository Structure

```text
.
├── Retail_Sales_EDA_Task1.ipynb
├── Retail Sales Dataset.csv
└── README.md
```
📄 License
Created for educational and portfolio purposes as part of the Oasis Infobyte Summer Internship Program.

## Author

Soumya Satyajit | Data Analytics Intern, Oasis Infobyte | #oasisinfobyte

