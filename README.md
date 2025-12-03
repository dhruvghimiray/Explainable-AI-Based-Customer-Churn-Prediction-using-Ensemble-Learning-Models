# Customer Churn Prediction Project

## Project Overview

This project focuses on predicting customer churn for a telecommunications company. Customer churn prediction is a critical business problem that helps companies identify customers who are likely to leave, allowing them to take preventive actions to retain those customers.

## Data Science Workflow

The analysis follows a structured data science workflow:

1. **Data Exploration and Review** (`notebooks/01_data_exploration_and_review.ipynb`)
   - Initial exploration of the dataset
   - Understanding data structure, features, and missing values

2. **Exploratory Data Analysis** (`notebooks/02_exploratory_data_analysis.ipynb`)
   - Statistical analysis and visualization of key features
   - Identification of patterns and relationships in the data

3. **Data Engineering and Preprocessing** (`notebooks/03_data_engineering_and_preprocessing.ipynb`)
   - Data cleaning and transformation
   - Feature engineering and selection
   - Handling of missing values and outliers

4. **Processed Data Analysis** (`notebooks/04_processed_data_analysis.ipynb`)
   - Analysis of the preprocessed data
   - Validation of data quality

5. **Model Comparison and Training** (`notebooks/05_model_comparison_and_training.ipynb`)
   - Implementation and comparison of multiple ML algorithms
   - Hyperparameter tuning and cross-validation

6. **Final Model Training and SHAP Analysis** (`notebooks/06_final_model_training_and_shap_analysis.ipynb`)
   - Training of the final selected model
   - SHAP (SHapley Additive exPlanations) analysis for feature importance
   - Model interpretation and insights

## Directory Structure

```
├── data/                 # Data directory
│   ├── external/         # External data sources not used in the model
│   ├── processed/        # Clean, processed data ready for modeling
│   └── raw/              # Raw, immutable data
├── docs/                 # Documentation files
├── models/               # Trained models and model metadata
├── notebooks/            # Jupyter notebooks for each stage
├── results/              # Results, reports, and summary statistics
├── src/                  # Source code
│   ├── data/             # Data loading and preprocessing scripts
│   ├── features/         # Feature engineering functions
│   ├── models/           # Model training and evaluation scripts
│   ├── utils/            # Utility functions
│   └── visualization/    # Visualization and plotting functions
├── requirements.txt      # Project dependencies
└── README.md             # This file
```

## Data Sources

- **Primary Dataset** (`data/raw/customer_churn_data_original.csv`): Original Churn_Modelling dataset used for the main analysis
- **Comparison Dataset** (`data/external/telco_customer_churn_data.csv`): Telco customer churn data used for comparison purposes
- **Processed Dataset** (`data/processed/customer_churn_data_processed.csv`): Cleaned and preprocessed version of the primary dataset
- **Final Dataset** (`data/processed/customer_churn_data_final.csv`): Final feature-engineered dataset used for model training

## Models Explored

The project compares several machine learning algorithms for customer churn prediction, including:
- Logistic Regression
- Random Forest
- Gradient Boosting
- Support Vector Machine
- Neural Networks

## Requirements

Install the required packages by running:

```bash
pip install -r requirements.txt
```

## Key Findings

- Top churn indicators identified through SHAP analysis
- Model performance metrics and interpretation
- Business recommendations based on model insights
"