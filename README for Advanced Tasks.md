**Task 1 Term Deposit Subscription Prediction**
**Objective**
To build a machine learning model that predicts whether a customer will subscribe to a term deposit, and to enhance model transparency using Explainable AI (SHAP).

**Approach**
**Data Preprocessing**
Loaded and parsed semicolon-delimited CSV data
Applied Label Encoding to convert categorical variables into numerical format
**Model Development**
Implemented XGBoost, a powerful gradient boosting algorithm
Tuned model parameters to improve predictive performance
**Evaluation Metrics**
Used F1-Score to balance precision and recall
Used ROC-AUC to evaluate model performance under class imbalance
**Model Interpretability**
Applied SHAP (SHapley Additive exPlanations) for explainability
Identified key influencing features such as:
duration (last contact duration)
poutcome (previous campaign outcome)
**Results and Findings**
Model Performance: Achieved an AUC score of 0.93 (update with your actual score)
**Key Insight:**
The duration of the last contact is the most influential factor in predicting subscription
**Explainability Impact:**
SHAP analysis provided clear explanations for individual predictions
Helped identify high-probability customers and understand model decisions
**Key Skills Gained**
Machine Learning Classification (XGBoost)
Model Interpretability (SHAP / Explainable AI)
Customer Behavior Analysis
Handling Imbalanced Datasets.



