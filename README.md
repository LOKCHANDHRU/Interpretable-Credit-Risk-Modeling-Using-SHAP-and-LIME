# Interpretable-Credit-Risk-Modeling-Using-SHAP-and-LIME

This project focuses on building a machine learning model to predict outcomes using a structured dataset. The workflow includes data preprocessing, feature engineering, and model training using an advanced algorithm to achieve high accuracy. The project also includes explainable AI techniques such as SHAP and LIME to understand how the model makes decisions. SHAP provides global insights about which features influence predictions the most, while LIME gives local explanations for individual cases. The final model is evaluated using metrics such as accuracy, AUC, and F1-score, and the trained model is saved for future use.


# Project Objectives

- Dataset loading (or synthetic dataset generation if none provided)  
- Feature engineering (engineered predictors for interpretability and predictive power)  
- Train–test split  
- Feature scaling (StandardScaler)  
- XGBoost model training (tuned parameters)  
- Model evaluation (AUC, Accuracy, F1)  
- SHAP global explanation (summary plot and numeric SHAP values)  
- LIME local explanations for 5 selected test samples  
- Report generation in UTF-8-safe `.txt` files

# Dataset Explanation 

This project uses a structured credit-risk dataset containing borrower financial details and loan outcome labels. The purpose of the dataset is to support the development of an interpretable machine-learning model that predicts whether a borrower will default or remain safe.

<a href = "">  Dataset </a>


# Text-based report section detailing feature engineering choices and final model performance metrics

###  Engineered_features
  - `income_to_loan_ratio`
  - `high_dti`
  - `long_credit_history`
  - `many_open_accounts`
  - `high_revol_util`
  - <a href ="https://github.com/LOKCHANDHRU/Interpretable-Credit-Risk-Modeling-Using-SHAP-and-LIME/blob/main/Feature_Engineering_Report.txt"> Feature_Engineeriong</a>

### Model_Performance
  - AUC
  - F1-score
  - Accuracy
  - Classification report
  - <a href="https://github.com/LOKCHANDHRU/Interpretable-Credit-Risk-Modeling-Using-SHAP-and-LIME/blob/main/Model_Performance_Report.txt"> Model_Performance</a>

# Textual summary of global SHAP findings, including the top 5 feature interpretations

### SHAP_Global_Summary
  - Ranked top-5 features by mean |SHAP|
  - Plain-language interpretation of how each top feature influences default risk
  - <a href ="https://github.com/LOKCHANDHRU/Interpretable-Credit-Risk-Modeling-Using-SHAP-and-LIME/blob/main/SHAP_Global_Summary.txt "> Shap_Global_Summary</a>


# Textual analysis comparing LIME justifications with global SHAP insights

### LIME_Local_Comparison
  - Short explanation of SHAP vs LIME (global vs local)
  - Local LIME explanations for 5 selected cases (feature contributions & predicted labels)
  - A comparison discussing alignment or differences between local justifications and global feature importance
  - <a href="https://github.com/LOKCHANDHRU/Interpretable-Credit-Risk-Modeling-Using-SHAP-and-LIME/blob/main/LIME_Local_Comparison.txt">LIME_Local_Comparison </a>



