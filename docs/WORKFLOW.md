# Data Science Workflow Documentation

## Project: Customer Churn Prediction

### 1. Data Exploration and Review (`01_data_exploration_and_review.ipynb`)
**Objective**: Initial exploration of the primary dataset (customer_churn_data_original.csv)
- Load and examine the structure of the dataset
- Check for missing values, data types, and basic statistics
- Identify potential issues or anomalies in the data
- Compare with the external Telco dataset characteristics

### 2. Exploratory Data Analysis (`02_exploratory_data_analysis.ipynb`)
**Objective**: Deep analysis of relationships and patterns in the data
- Distribution analysis of features
- Correlation analysis between features and target variable
- Visualization of key patterns and trends
- Identify potential features for modeling
- Compare insights with Telco dataset findings

### 3. Data Engineering and Preprocessing (`03_data_engineering_and_preprocessing.ipynb`)
**Objective**: Prepare the data for machine learning models
- Handle missing values
- Encode categorical variables
- Scale numerical features
- Address class imbalance if present
- Create new features based on domain knowledge
- Create the processed dataset

### 4. Processed Data Analysis (`04_processed_data_analysis.ipynb`)
**Objective**: Validate the quality of the preprocessed data
- Verify the preprocessing steps
- Analyze the processed dataset for any remaining issues
- Confirm feature relationships after preprocessing
- Generate the final dataset for modeling

### 5. Model Comparison and Training (`05_model_comparison_and_training.ipynb`)
**Objective**: Train and compare multiple machine learning models
- Split data into train/validation/test sets
- Train multiple algorithms (Logistic Regression, Random Forest, XGBoost, etc.)
- Perform hyperparameter tuning
- Compare model performance using various metrics
- Select the best performing model based on validation results

### 6. Final Model Training and SHAP Analysis (`06_final_model_training_and_shap_analysis.ipynb`)
**Objective**: Finalize the chosen model and perform interpretability analysis
- Retrain the best model on the complete training dataset
- Evaluate on the test set
- Perform SHAP analysis to understand feature importance
- Generate model interpretation insights
- Document final model performance and recommendations

## Key Results

### Primary Dataset Focus
- The primary analysis focused on the customer_churn_data_original.csv dataset
- The Telco dataset was used for cross-validation of methodologies and insights
- Final model based on the bank customer churn data

### Target Variable
- Target: `exited` (binary: 0 = No churn, 1 = Churn)
- Goal: Predict the likelihood of customer churn

### Success Metrics
- Accuracy: Percentage of correctly predicted instances
- Precision: Proportion of predicted positive instances that are actually positive
- Recall: Proportion of actual positives that are correctly identified
- F1 Score: Harmonic mean of precision and recall
- AUC-ROC: Area under the Receiver Operating Characteristic curve