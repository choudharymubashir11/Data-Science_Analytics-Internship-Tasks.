# DevelopersHub Data Science Internship Tasks

## Task 1: Exploring and Visualizing a Simple Dataset
**1. Introduction and Problem Statement**
The objective of this task is to understand how to read, summarize, and visualize the Iris dataset. We will perform Exploratory Data Analysis (EDA) to identify patterns and relationships between sepal and petal measurements across different iris species.

**2. Data Loading and Inspection **
# Download the Iris dataset from UCIML via kagglehub [cite: 13]
dataset_path = kagglehub.dataset_download("uciml/iris")
file_path = os.path.join(dataset_path, "Iris.csv")

# Load the dataset using pandas [cite: 14]
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
