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


# Advanced Task 2: Customer Segmentation

## 1. Objective
To group mall customers into distinct segments based on their annual income and spending patterns using Unsupervised Learning.

## 2. Approach
**EDA**: Visualized age, income, and spending distributions to understand the customer base.
* **Feature Scaling**: Standardized numerical features to ensure the clustering algorithm performs accurately.
* **K-Means Clustering**: Applied the **Elbow Method** to identify 5 optimal customer clusters.
* **Dimensionality Reduction**: Used **PCA (Principal Component Analysis)** to project the 2D clusters onto a readable plot.

## 3. Results and Findings 
We identified 5 distinct customer groups:
1. **Target Customers**: High income, high spending.
2. **Standard Customers**: Average income, average spending.
3. **Careful Customers**: High income, low spending.
4. **Spendthrifts**: Low income, high spending.
5. **Sensible Customers**: Low income, low spending.

## 4. Suggested Marketing Strategies 
* **Target Customers**: Enroll in premium loyalty programs and offer early access to new collections.
* **Careful Customers**: Send personalized promotions on luxury items to encourage spending.
* **Spendthrifts**: Provide frequent discount alerts and "buy-one-get-one" offers to maintain engagement.
* **Sensible Customers**: Focus on value-for-money marketing and essential items.

