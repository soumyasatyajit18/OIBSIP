# 📊 OIBSIP: Data Analytics Internship Projects

**Soumya Satyajit | Data Analytics Intern, Oasis Infobyte | #oasisinfobyte**

This repository contains three data analytics projects completed as part of the **Oasis Infobyte (OIBSIP) Data Analytics Internship**. The projects demonstrate practical work with Python, data cleaning, exploratory data analysis, customer segmentation, and data visualization.

---

## 📁 Projects

### 1. Retail Sales Exploratory Data Analysis (EDA)

**Notebook:** `Retail_Sales_EDA_Task1.ipynb`

Explores retail sales data to understand sales patterns, customer demographics, product performance, and relationships between numerical variables.

**What the notebook covers**
- Dataset inspection, data types, missing values, and duplicate checks
- Data preparation and date handling
- Descriptive statistics for numerical columns
- Monthly and quarterly sales trends
- Customer age-group and gender distributions
- Top products by sales value and revenue by category
- Correlation heatmap and average-spend comparisons by demographic group
- Key business metrics and actionable recommendations

### 2. Customer Segmentation using RFM and K-Means

**Notebook:** `Customer_Segmentation_RFM_KMeans.ipynb`

Segments an online retail customer base based on purchasing behaviour, using **Recency, Frequency, and Monetary (RFM)** features and the K-Means clustering algorithm.

**What the notebook covers**
- Loading and inspecting online retail transaction data
- Cleaning transactions and calculating line-level sales
- Creating customer-level RFM features
- Transforming skewed features and standardizing inputs
- Reviewing candidate cluster counts using the elbow method and silhouette score
- Visualizing clusters and profiling customer groups
- Generating interpretable segment names and marketing recommendations
- Exporting customer-level segments and a cluster-profile summary

### 3. Data Cleaning and Quality Assurance

**Notebook:** `Task_3_Data_Cleaning.ipynb`

Builds a reproducible cleaning and validation workflow for a deliberately messy, synthetic Titanic-style passenger dataset.

**What the notebook covers**
- Documenting cleaning rules and decisions
- Auditing missing values, data types, unique values, and invalid ranges
- Standardizing blank values and parsing numeric fields
- Applying column-specific validation and missing-value treatments
- Detecting outliers using the Interquartile Range (IQR) method
- Comparing data quality before and after cleaning
- Validating the cleaned data with assertions
- Exporting an analysis-ready CSV dataset

---

## ✨ Project Highlights

| Project | Main focus | Key techniques |
|---|---|---|
| Retail Sales EDA | Understand sales and customer patterns | Pandas, descriptive statistics, time-based aggregation, visualizations |
| Customer Segmentation | Identify groups of customers by purchasing behaviour | RFM analysis, feature transformation, standardization, K-Means, silhouette score |
| Data Cleaning & QA | Improve data quality and reproducibility | Missing-value handling, range checks, duplicate removal, IQR screening, assertions |

These projects follow a practical analytics workflow: **inspect → clean → analyze → visualize or model → validate → communicate insights**.

> **Note:** Findings and numerical results depend on the input datasets and the outputs generated when the notebooks are run. No specific business result is claimed in this README.

---

## 🖼️ Preview

The notebooks generate their previews when executed:

- **Retail Sales EDA:** Monthly and quarterly sales charts, demographic distributions, product/category comparisons, and a correlation heatmap.
- **Customer Segmentation:** RFM distributions, elbow and silhouette evaluations, customer-cluster scatter plots, and cluster-profile summaries.
- **Data Cleaning & QA:** Before-and-after data quality reports, range audits, outlier summaries, and validation results.

To add screenshots to this README, save your own notebook output images in a folder such as `images/` and link them here. Example:

## Data Cleaning Summary

![Before and After Cleaning](Image/Before-versus-after%20summary.png)

## Correlation Heatmap

![Correlation Matrix](Image/Correlation%20Heatmap_Output.png)

## Customer Segmentation Visualizations

![Customer Segments](Image/Visualise%20clusters.png)



## 🧰 Skills Demonstrated

- **Python for Data Analytics**
- **Pandas and NumPy** for data manipulation and numerical operations
- **Data cleaning and preprocessing**
- **Exploratory Data Analysis (EDA)**
- **Descriptive statistics**
- **Data visualization** with Matplotlib and Seaborn
- **Time-based sales analysis**
- **Customer segmentation and RFM analysis**
- **K-Means clustering and feature standardization**
- **Cluster evaluation** using the elbow method and silhouette score
- **Data quality auditing and validation**
- **Outlier screening using IQR**
- **Jupyter Notebook documentation**
- **Business interpretation and recommendations**

---

## 🗂️ Repository Structure

```text
OIBSIP-Data-Analytics/
├── README.md
├── Retail_Sales_EDA_Task1.ipynb
├── Customer_Segmentation_RFM_KMeans.ipynb
├── Task_3_Data_Cleaning.ipynb
├── Retail Sales Dataset.csv                 # input for Project 1
├── OnlineRetail.csv                         # input for Project 2
└── data/
    ├── titanic_style_messy_dataset.csv       # input for Project 3
    └── titanic_style_cleaned_dataset.csv     # generated output
```

The CSV files shown are expected inputs/outputs based on the notebooks; add the input datasets to your repository only when you have them and are permitted to share them. Generated CSV outputs appear after the relevant notebook is run.

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd OIBSIP-Data-Analytics
```

Replace `<your-github-repository-url>` with your actual GitHub repository URL.

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Add the required datasets

Place each dataset at the path expected by its notebook:

- **Retail Sales EDA:** `Retail Sales Dataset.csv` in the project root, or update `FILE_PATH` in the notebook.
- **Customer Segmentation:** `OnlineRetail.csv` in the project root, or update `DATA_PATH`.
- **Data Cleaning:** `data/titanic_style_messy_dataset.csv`, matching the path in the notebook.

The third notebook describes its data as a deliberately messy, synthetic Titanic-style dataset. Make sure the file you provide matches that expected schema.

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open a notebook and run its cells from top to bottom. Run each notebook separately and verify that its input files are available before execution.

---

## 👤 About Me

### Soumya Satyajit | Data Analytics Intern, Oasis Infobyte

I am building practical data analytics skills through hands-on projects involving Python, data preparation, exploratory analysis, visualization, and customer segmentation. These projects reflect my learning and application of analytical techniques to structure data, investigate patterns, and communicate findings.

**Internship:** Oasis Infobyte — OIBSIP Data Analytics Internship  
**Hashtags:** `#oasisinfobyte` `#OIBSIP` `#DataAnalytics` `#Python` `#EDA` `#CustomerSegmentation`

---

## 🙌 Acknowledgment

Thanks to **Oasis Infobyte** for the opportunity to learn and practice data analytics through project-based work.

---

*Created by Soumya Satyajit as part of the OIBSIP Data Analytics Internship.*
