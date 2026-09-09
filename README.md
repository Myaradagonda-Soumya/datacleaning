#  Data Cleaning

## Project Overview

This project demonstrates a professional data cleaning workflow using Python, Pandas, and NumPy.

A deliberately messy employee dataset was analyzed and transformed into a clean, analysis-ready dataset.

## Objective

The main objective of this project is to identify and resolve common data quality problems, including:

- Missing values
- Duplicate records
- Inconsistent formatting
- Incorrect data types
- Date formatting issues
- Numerical outliers
- Data quality anomalies

## Tools and Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Dataset

The project uses a messy employee dataset containing employee information such as:

- Employee ID
- First Name
- Last Name
- Age
- Department/Region
- Status
- Join Date
- Salary
- Email
- Phone
- Performance Score
- Remote Work

## Data Cleaning Process

### 1. Data Quality Assessment

The dataset was inspected for:

- Missing values
- Duplicate rows
- Data types
- Unique values
- Numerical range anomalies

### 2. Missing Value Handling

Missing numerical values were handled using median imputation.

Median was selected because employee salary and age data can contain extreme values, and the median is less affected by outliers than the mean.

### 3. Duplicate Removal

The dataset was checked for duplicate records.

No exact duplicate rows were found.

### 4. Data Standardisation

Inconsistent text formatting was standardized.

Whitespace and categorical formatting were cleaned to improve consistency.

### 5. Date Conversion

The `Join_Date` column was converted from object/string format to:

`datetime64[ns]`

### 6. Data Type Correction

The following data type corrections were performed:

- `Join_Date` → datetime
- `Salary` → float
- `Phone` → string
- `Remote_Work` → Boolean

Phone numbers were stored as strings because they are identifiers rather than numerical values.

### 7. Outlier Detection

The Interquartile Range (IQR) method was used to detect potential outliers in numerical columns.

Outlier analysis was performed on:

- Age
- Salary

No IQR-based outliers were identified, so no observations were removed or capped.

#Conclusion

The messy employee dataset was successfully cleaned and transformed into an analysis-ready dataset.
The project demonstrates practical data cleaning skills including missing value treatment, duplicate verification, standardisation, data type correction, date conversion, and outlier detection using Python and Pandas.

#Author
Soumya



