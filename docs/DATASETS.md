# Dataset Documentation

## Primary Dataset: Customer Churn Data

**File**: `data/raw/customer_churn_data_original.csv` (originally Churn_Modelling.csv)

This dataset contains information about bank customers and whether they exited the bank (churned). It was selected as the primary dataset for the churn prediction analysis.

### Features:
- `row_number`: Row number
- `customer_id`: Unique customer identifier
- `surname`: Customer surname
- `credit_score`: Credit score of the customer
- `geography`: Country of residence (Germany, Spain, France)
- `gender`: Gender of the customer (Male, Female)
- `age`: Age of the customer
- `tenure`: Number of years the customer has been with the bank
- `balance`: Account balance
- `num_of_products`: Number of bank products the customer uses
- `has_cr_card`: Whether the customer has a credit card (0: No, 1: Yes)
- `is_active_member`: Whether the customer is active (0: No, 1: Yes)
- `estimated_salary`: Estimated salary
- `exited`: Target variable (0: No, 1: Yes)

### Dataset Size:
- Rows: [To be updated based on actual data]
- Columns: 14

## Comparison Dataset: Telco Customer Churn

**File**: `data/external/telco_customer_churn_data.csv` (originally Telco_customer_churn(Telco_Churn).csv)

This dataset contains customer churn information from a telecommunications company and was used for comparison purposes in our analysis to validate findings and methodologies across different domains.

### Features:
- [To be updated based on actual data - varies significantly from primary dataset]

## Processed Datasets

### Processed Data
**File**: `data/processed/customer_churn_data_processed.csv`
- Contains cleaned and preprocessed version of the primary dataset
- Missing values handled, categorical variables encoded
- Outliers treated, feature engineering applied

### Final Data
**File**: `data/processed/customer_churn_data_final.csv`
- Contains the final features used for model training
- Feature selection performed
- Ready for machine learning algorithms