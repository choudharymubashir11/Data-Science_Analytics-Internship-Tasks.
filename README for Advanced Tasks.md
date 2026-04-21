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



# Advanced Task 3: Energy Consumption Time Series Forecasting

## 1. Objective
To forecast daily household energy usage by analyzing historical power consumption data and comparing statistical, machine learning, and temporal models.

## 2. Approach
* **Data Preprocessing**: Combined Date/Time columns, handled missing values via forward filling, and resampled the minute-by-minute data into a Daily frequency for clearer trend analysis.
* **Feature Engineering**: Extracted temporal features such as `day_of_week`, `month`, and `is_weekend` to help models understand seasonal and weekly cyclicality.
* **Modeling**:
    * **ARIMA**: A statistical model used to capture linear relationships in the time series.
    * **XGBoost**: A gradient boosting regressor utilized to model complex non-linear relationships using engineered time features.
* **Evaluation**: Compared models using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## 3. Results and Findings
* **Temporal Patterns**: Energy consumption peaks significantly during specific seasons and shows a clear distinction between weekdays and weekends.
* **Model Performance**: XGBoost generally outperformed ARIMA in capturing sudden spikes in usage, while ARIMA provided a smoother baseline for general trends.
* **Insights**: Household energy usage is highly dependent on time-of-day and seasonal factors, suggesting that targeted energy-saving alerts on peak days could reduce overall consumption.

## 4. Skills Gained
* Time series resampling and parsing
* Statistical vs. ML forecasting comparison
* Error evaluation (MAE, RMSE)
* Temporal data visualization.

# Advanced Task 4: Loan Default Risk with Business Cost Optimization

## 1. Objective
To predict the likelihood of loan default and determine the optimal decision threshold that minimizes the bank's total financial loss (Business Cost Optimization).

## 2. Approach
* **Data Cleaning**: Imputed missing values for employment length and interest rates using medians and removed age/employment outliers.
* **Feature Engineering**: Applied One-Hot Encoding to categorical variables and standardized numerical features for the Logistic Regression model.
* **Cost-Benefit Analysis**:
    * **False Negative (FN)**: Approving a risky loan.
    Cost = Total Loan Principal.
    * **False Positive (FP)**: Rejecting a safe loan.
      Cost = Lost Interest Profit.
  **Optimization**: Iterated through probability thresholds (0.0 to 1.0) to find the specific cut-off that minimizes the sum of FN and FP costs.

## 3. Results and Findings
* **Optimal Threshold**: The model revealed that a lower threshold (e.g., 0.20 - 0.30) is often better than the default 0.50, as it catches more defaults and saves the bank significantly more money.
* **Risk Score**: The loan grade and interest rate were among the most significant predictors of risk.
* **Financial Impact**: By adjusting the threshold based on costs, we reduced the total simulated business loss by [Insert your cost savings]% compared to standard modeling.

## 4. Skills Gained
* Binary classification and risk scoring.
* Cost-based evaluation metrics (moving beyond simple accuracy).
* Decision threshold tuning for business profit.
