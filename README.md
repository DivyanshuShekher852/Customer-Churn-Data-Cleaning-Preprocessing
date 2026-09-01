Customer Churn Data Cleaning & Preprocessing

Objective

Clean and validate the supplied customer churn sample dataset using Python, Pandas and NumPy.

Step-by-step implementation

1. Dataset

Input: customer_churn_sample.csv

Dataset size: 15 rows × 11 columns

2. Data inspection

The raw data was checked for:

Missing values

Duplicate records

Data type mismatches

Column-header consistency

Categorical-string consistency

Date/time fields

3. Missing values

Missing values found: 0

Because no null values were present, no imputation and no row deletion were required.

4. Standardization

Headers were converted to lowercase snake_case.

CamelCase headers such as CustomerID and TenureMonths were handled correctly.

Categorical strings were stripped of leading/trailing whitespace.

Integer and decimal columns were explicitly converted to the expected numeric types.

No date/time columns exist in this dataset, so date-format conversion was not applicable.

5. Validation

The cleaned data passed these checks:

Customer IDs are unique.

Age values are within the expected range.

Tenure is non-negative.

Monthly charges are non-negative.

Total charges are non-negative.

Support tickets are non-negative.

Total charges equal monthly charges × tenure for every record.

6. Final result

Rows after cleaning: 15

Columns after cleaning: 11

Missing values after cleaning: 0

Duplicate rows after cleaning: 0

Deliverables

customer_churn_clean.csv — final cleaned dataset

customer_churn_cleaning.py — reusable cleaning script

data_quality_report.csv — quality-control results

Tools

Python, Pandas, NumPy, CSV
