# DevelopersHub Data Science Internship Tasks

## Task 1: Exploring and Visualizing a Simple Dataset
**1. Introduction and Problem Statement**
The objective of this task is to understand how to read, summarize, and visualize the Iris dataset. We will perform Exploratory Data Analysis (EDA) to identify patterns and relationships between sepal and petal measurements across different iris species.

**2. Data Loading and Inspection **
# Download the Iris dataset from UCIML via kagglehub
dataset_path = kagglehub.dataset_download("uciml/iris")
file_path = os.path.join(dataset_path, "Iris.csv")

# Load the dataset using pandas 
df = pd.read_csv(file_path)

**3. Exploratory Data Analysis (EDA)**
Using matplotlib and seaborn , we will create the visualizations required by the task.○ Scatter Plot: Relationship Analysis Pythonplt.figure(figsize=(8, 5))
Histogram: Data Distribution Pythonplt.figure(figsize=(8, 5))
Box Plot: Outlier Detection Pythonplt.figure(figsize=(10, 6))

** 4. Conclusion and Insights **
**Structure**: The dataset contains 150 observations with 4 physical features.
**Relationships:** The scatter plot shows that Iris-setosa is clearly separated from the other two species based on sepal dimensions.
**Distributions**: The histogram reveals that petal lengths are not normally distributed, showing a clear gap between species groups.
**Outliers**: The box plots suggest that while most data is tightly grouped, some species show slight variations in petal width that may act as outliers.

**Task 2: Credit Risk Prediction**
**1. Project Objective**
The primary goal of this task is to predict whether a loan applicant is likely to default on a loan. By using historical applicant data, we aim to build a binary classification model that helps financial institutions make data-driven lending decisions.

**2. Dataset Description**
Source: Loan Prediction Dataset via Kaggle.
Features: Includes applicant information such as income, loan amount, education level, and marital status.
Target Variable: A binary indicator representing whether the applicant defaulted (loan_approved/Loan_Status).

**3. My ApproachTo complete this task, I followed a standard Data Science pipeline:**
Data Cleaning: Handled missing values using statistical imputation (median for numerical and mode for categorical data).
Exploratory Data Analysis (EDA): Created histograms and count plots to visualize the distribution of loan amounts and the relationship between applicant income and default risk.
Feature Engineering: Encoded categorical variables into numerical format to make them compatible with machine learning algorithms.
Model Training: Trained a Logistic Regression classifier to establish a baseline for prediction.
Model Evaluation: Tested the model using a 20% data split and evaluated performance using a Confusion Matrix and Accuracy Score.

**4. Key Results and Insights**
Accuracy: The model achieved a baseline accuracy reflecting its ability to distinguish between low-risk and high-risk applicants.
Confusion Matrix: The matrix provided insight into Type I (False Positives) and Type II (False Negatives) errors, which is critical for assessing financial risk.
Insights: Preliminary analysis suggests that variables like income and loan amount are significant indicators of an applicant's ability to repay.

**5. Tools and Libraries UsedPython Pandas: **
For data manipulation and cleaning Matplotlib & Seaborn: 
For data visualization Scikit-learn: 
For model training and evaluation metrics.

**Task 3: Customer Churn Prediction (Bank Customers)**
**1. Introduction and Problem Statement**
The objective of this task is to identify customers who are likely to leave the bank (churn). By identifying these individuals early, the bank can implement retention strategies to reduce customer turnover and maintain a stable customer base.

**2. Dataset Understanding and Description**
**Source:** Churn Modelling Dataset via Kaggle.
**Structure:** The dataset contains customer demographic and account information, including tenure, monthly charges, and total charges.
**Target Variable**: Churn (Converted to binary: 1 for 'Yes', 0 for 'No').

**3. Data Cleaning and Preparation**
**Identification Removal:** Dropped irrelevant columns like customerID to focus on predictive features.
**Handling Categorical Data**: Used One-Hot Encoding (via pd.get_dummies) to convert categorical features such as gender and other object-type columns into numerical format.
**Target Encoding:** Mapped the 'Yes'/'No' churn labels to 1/0 for compatibility with machine learning models.

4. Exploratory Data Analysis (EDA)

**Churn Distribution: **Created a count plot to visualize the ratio of retained customers versus those who exited.
**Tenure Analysis: **Utilized box plots to examine the relationship between a customer's tenure and their likelihood of churning.

**5. Model Training and TestingAlgorithm:** A Random Forest Classifier was utilized to perform supervised classification.Data Split: The dataset was split into training and testing sets (80% training, 20% testing) to ensure unbiased evaluation.

6. Evaluation MetricsThe model was evaluated using the following metrics:
Accuracy: Measures the overall percentage of correct predictions.
Confusion Matrix: Used to analyze True Positives, True Negatives, False Positives, and False Negatives.

**7. Conclusion and Key Insights**

**Feature Importance:** Using the Random Forest model's internal scoring, the top 10 factors influencing churn were identified and visualized.
**Key Findings:** Factors such as tenure and monthly charges play a significant role in a customer's decision to stay or leave.
**Strategic Value:** These insights allow for targeted business interventions to improve customer loyalty.


# Task 4: Predicting Insurance Claim Amounts

## 1. Project Objective
To estimate medical insurance charges for individuals based on their health and demographic data using regression modeling.

## 2. Dataset Description
**Source:** Medical Cost Personal Dataset[cite: 58].
**Features:** Age, Sex, BMI, Children, Smoker, and Region[cite: 56, 61].
**Target:** `charges` (Numerical value of medical costs)[cite: 60].

## 3. My Approach
**Feature Engineering:** Mapped binary categories (Sex, Smoker) and applied One-Hot Encoding to the Region column.
**EDA:** Created scatter plots to analyze the correlation between Age/BMI and insurance costs, specifically highlighting the smoking variable.
**Modeling:** Implemented a Linear Regression model to predict the continuous 'charges' variable[cite: 60, 87].
**Evaluation:** Used Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to quantify prediction errors[cite: 62, 88].

## 4. Results & Insights
**Insights:** Being a smoker is the single largest factor leading to higher insurance charges.
**Observations:** BMI shows a strong positive relationship with charges, but primarily for individuals who smoke.
**Error Metrics:** The MAE provides a direct understanding of the model's average prediction error in dollar terms.

# Task 5: Personal Loan Acceptance Prediction

## 1. Project Objective
To predict customer acceptance of personal loan offers using demographic and campaign data from a bank's marketing efforts.

## 2. Dataset Description
- **Source:** Bank Marketing Dataset (UCI Machine Learning Repository).
- **Features:** Age, Job, Marital Status, Education, Housing/Personal Loan status, and Campaign details.
- **Target:** `y` (Whether the client subscribed to a term deposit).

## 3. My Approach
- **Data Exploration:** Analyzed how job types and marital status correlate with loan acceptance.
- **Data Preprocessing:** Handled the semicolon delimiter and applied One-Hot Encoding to categorical features.
- **Modeling:** Built a Decision Tree Classifier to provide an easily interpretable model for business stakeholders.
- **Evaluation:** Focused on Accuracy and Classification Reports to measure the model's predictive power.

## 4. Results & Insights
- **Key Findings:** Specific job sectors show significantly higher interest in term deposits.
- **Business Extraction:** By focusing on the "high-probability" groups identified by the Decision Tree, the bank can increase its conversion rate while lowering operational costs.
  
