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

<a href ="https://github.com/LOKCHANDHRU/Interpretable-Credit-Risk-Modeling-Using-SHAP-and-LIME/blob/main/credit_risk_dataset.csv">  Dataset </a>

# Model Training

The credit risk prediction model is built using **XGBoost**, a high-performance gradient boosting algorithm widely used for tabular financial data.

### Model Training (XGBoost)
The model was trained using the **XGBoost** classifier, a high-performance gradient boosting algorithm widely used for financial risk prediction. The training process included feature scaling, hyperparameter tuning, and iterative boosting rounds to improve accuracy. Key training parameters such as learning rate, number of estimators, max depth, subsampling, and column sampling were optimized to reduce overfitting and enhance model stability. The final model demonstrated strong performance in predicting the likelihood of loan default.

### SHAP Explainability
To ensure transparency and build trust in the model's predictions, **SHAP (SHapley Additive exPlanations)** was used to interpret both global and individual predictions.

#### Global Explanations
- SHAP summary plots highlight the most influential features.
- Feature importance rankings show how financial variables impact default risk.
- Provides a clear understanding of the model’s overall decision logic.

#### Local Explanations
- SHAP force plots explain why a particular applicant is predicted as “default” or “non-default”.
- Shows how each feature pushes the prediction higher or lower.
- Useful for credit officers to justify decisions for individual loan applications.

SHAP ensures the model is highly interpretable and not a black-box system.

# Technologies Used
- **Python 3.x** – Core development language  
- **Pandas & NumPy** – Data manipulation and numerical processing  
- **Scikit-learn** – Preprocessing and evaluation  
- **XGBoost** – Gradient boosting classification model  
- **SHAP** – Explainable AI framework  
- **Matplotlib / Seaborn** – Visualization libraries  
- **Jupyter Notebook / Google Colab** – Development and experimentation environment  


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

# Conclusion
This project successfully demonstrates how machine learning can be used to predict loan default risk with high accuracy while maintaining transparency through explainable AI techniques. The combination of XGBoost for strong predictive performance and SHAP for interpretability ensures the model is reliable, actionable, and suitable for real-world financial decision-making. The insights produced can assist credit officers in making informed, fair, and accountable lending decisions.

