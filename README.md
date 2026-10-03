# ApexPlanet Data Analytics – Task 1

## Task 1: Data Immersion & Wrangling

### Objective
The objective of this task is to understand, assess, clean, and transform the provided sales dataset into an analysis-ready dataset.

## Dataset
The dataset contains sales, customer, product, order, and transaction information.

### Main Columns
- Order_ID
- Order_Date
- Customer_ID
- Customer_Name
- Age
- Gender
- City
- Product
- Category
- Quantity
- Unit_Price
- Total_Sales

## Work Performed

### 1. Data Access & Familiarization
- Reviewed the provided sales dataset.
- Studied the variables and their data types.
- Created a data dictionary describing each column.

### 2. Data Quality Assessment
The dataset was checked for:
- Missing values
- Duplicate records
- Inconsistent formatting
- Potential outliers
- Sales calculation consistency

### 3. Data Cleaning
- Handled missing Age values using the dataset median.
- Replaced missing City values with `Unknown`.
- Standardized text fields by removing unnecessary spaces.
- Converted Order_Date into a proper date format.
- Reviewed repeated Order_ID values without deleting valid transactions.

### 4. Data Transformation
- Created `Order_Month` from Order_Date.
- Created `Order_Year` from Order_Date.
- Created `Calculated_Total_Sales` using Quantity × Unit_Price.
- Added `Sales_Outlier_Flag` using the IQR method.

## Key Data Quality Findings
- Missing Age values: 20
- Missing City values: 13
- Exact duplicate rows: 0
- Repeated Order_ID occurrences were reviewed and handled.
- Potential sales outliers were flagged for review rather than automatically deleted.

## Tools Used
- Microsoft Excel
- Python
- Pandas

## Project Files

```text
ApexPlanet-DataAnalytics-Task1/
│
├── Dataset/
│   ├── ApexPlanet_DataAnalytics_Dataset.xlsx
│   └── ApexPlanet_Task1_Cleaned_Data.csv
│
├── Data Dictionary/
│   └── ApexPlanet_Data_Dictionary.xlsx
│
├── Python Script/
│   └── cleaning_script.py
│
├── Data Quality Report/
│   └── ApexPlanet_Data_Quality_Report.xlsx
│
└── README.md
```

## Final Outcome
The data was cleaned and transformed into an analysis-ready dataset that can be used for further data analysis and visualization.

## Author
ApexPlanet Data Analytics Internship – Task 1
