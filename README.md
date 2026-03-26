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

