# Customer Shopping Behavior Analysis

## Overview

This project demonstrates an end-to-end data analytics workflow using Python, SQL Server, and Power BI. It covers data loading, cleaning, exploratory data analysis (EDA), SQL querying, and dashboard visualization to extract meaningful insights from customer shopping behavior data.

## Dataset
* **Name:** Customer Shopping Behavior Dataset
* **Format:** CSV
* **Description:** Contains customer demographics, purchase behavior, frequency of purchases, discounts, and review ratings.

## Tools & Technologie
* **Python** (Pandas, NumPy)
* **Jupyter Notebook**
* **MS SQL Server (SQLEXPRESS)**
* **pyodbc & SQLAlchemy**
* **Power BI**

## Project Workflow
### 1. Data Loading
* Imported dataset using Pandas
* Standardized column names (lowercase, underscores)

### 2. Data Cleaning

* Handled missing values using median imputation
* Converted categorical frequency data into numeric format
* Removed redundant columns
* Created new features (e.g., age groups)

### 3. Exploratory Data Analysis (EDA)
* Checked data types and structure
* Analyzed missing values
* Generated summary statistics
* Explored relationships between variables

### 4. SQL Integration (MS SQL Server)
* Connected Python to SQL Server using `pyodbc`
* Created tables directly from Pandas DataFrame
* Stored cleaned dataset in SQL Server
* Ran SQL queries for analysis and validation

### 5. Power BI Dashboard
* Connected Power BI to SQL Server database
* Imported cleaned dataset
* Built interactive dashboards and visualizations

## Results & Insights

* Identified customer purchase patterns
* Analyzed impact of discounts and promo codes
* Segmented customers by age groups
* Evaluated purchase frequency trends

## Dashboard

The Power BI dashboard includes:
* Sales distribution by category
* Customer segmentation (age groups)
* Purchase frequency analysis
* Discount vs purchase behavior

## How to Run the Project

### 1. Clone or Download
* Download the project files and dataset
### 2. Run Jupyter Notebook
```bash
pip install pandas numpy pyodbc sqlalchemy
```
* Open the notebook
* Run all cells step-by-step
### 3. Connect to SQL Server
* Ensure SQL Server (SQLEXPRESS) is running
* Update connection string if needed:
```python
SERVER=localhost\\SQLEXPRESS
```
### 4. Load Data into SQL Server
* Use:
```python
df.to_sql('customer_data', engine, if_exists='replace', index=False)
```

### 5. Open Power BI
* Connect to SQL Server
* Load `customer_data` table
* Build or view dashboard

## Conclusion

This project showcases a complete data analytics pipeline, from raw data to business insights—using industry-standard tools. It highlights skills in data cleaning, SQL integration, and dashboard development.
