# Advanced Task 1: Term Deposit Subscription Prediction

## Objective
To leverage machine learning to predict bank marketing success and provide interpretability using Explainable AI (SHAP).

## Approach
- **Preprocessing**: Parsed semicolon-delimited CSV and performed Label Encoding on categorical variables.
- **Modeling**: Implemented **XGBoost**, an industry-standard gradient boosting algorithm.
- **Evaluation**: Focused on **F1-Score** and **ROC-AUC** to account for the class imbalance in marketing data.
- [**Interpretability**: Used **SHAP** values to explain individual predictions, identifying 'duration' and 'poutcome' as key factors.

## Results and Findings
- **Predictive Power**: The model achieved an AUC of [Insert your score, e.g., 0.93], showing excellent separation between classes.
- **Top Drivers**: SHAP analysis revealed that the duration of the last contact was the single most influential factor in a customer's decision to subscribe.
- **XAI Value**: By explaining 5 individual predictions, we can see exactly why the model flagged specific customers as "high-probability" leads.

## [Key Skills Gained 
- Classification (XGBoost) 
- Model Interpretability (SHAP/XAI)
- Customer Behavior Analysis 


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

