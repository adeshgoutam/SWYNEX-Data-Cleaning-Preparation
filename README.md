# SWYNEX Task 1 - Data Cleaning & Preparation

## Project Overview

This project was completed as part of the SWYNEX Technologies internship.

The objective was to clean and prepare a raw retail dataset for further data analysis by identifying and handling missing values, duplicate records, data type issues, and inconsistent values.

## Dataset

**Dataset:** Online Retail Dataset

**Source:** UCI Machine Learning Repository

The dataset contains online retail transaction records with the following columns:

* InvoiceNo
* StockCode
* Description
* Quantity
* InvoiceDate
* UnitPrice
* CustomerID
* Country

## Tools Used

* Python
* Pandas
* Jupyter Notebook
* GitHub
* Google Drive

## Data Cleaning Process

### 1. Missing Values

Missing values were identified using Pandas.

* Rows with missing `Description` values were removed.
* Missing `CustomerID` values were retained because customer information is not required for every transaction-level analysis.

### 2. Duplicate Records

Duplicate records were identified and removed.

**Remaining duplicate rows:** 0

### 3. Data Types

The `InvoiceDate` column was converted to a proper datetime format for analysis.

### 4. Inconsistent Values

The dataset was checked for inconsistent or suspicious values, including:

* Extra spaces in text fields
* Negative quantities
* Zero or negative unit prices
* Cancelled invoices

Negative quantities and cancelled invoices were not automatically removed because they can represent legitimate business transactions such as returns or cancellations.

### 5. Final Validation

The cleaned dataset was validated after the cleaning process.

| Metric                   |  Result |
| ------------------------ | ------: |
| Original Rows            | 541,909 |
| Original Columns         |       8 |
| Cleaned Rows             | 536,641 |
| Cleaned Columns          |       8 |
| Rows Removed             |   5,268 |
| Remaining Duplicate Rows |       0 |

## Output

The final cleaned dataset is available here:

**Cleaned Dataset:**
[Google Drive - cleaned_online_retail.csv](https://drive.google.com/file/d/1_kR6xOn0ZyJOQ1Gy8L3JeWDphgQ9uR3E/view?usp=sharing)

## Notebook

The complete Python data-cleaning process is available in:

`Data_Cleaning_Preparation.ipynb`

## Key Learning Outcomes

Through this task, I practiced:

* Data quality assessment
* Missing value handling
* Duplicate detection and removal
* Data type conversion
* Text cleaning
* Identifying inconsistent values
* Dataset validation
* Working with Pandas
* Preparing data for further analysis

## Project Structure

```text
SWYNEX-Data-Cleaning-Preparation
│
├── Data_Cleaning_Preparation.ipynb
└── README.md
```

## Internship

Completed as part of **SWYNEX Technologies Internship - Task 1: Data Cleaning & Preparation**.
