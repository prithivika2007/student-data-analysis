# Student Data Analysis

## Overview
This project analyzes a student dataset using Python and Pandas. The dataset contains demographic and family background information of students, including gender, age, parental education, family size, and parental occupations.

## Task 1: Exploratory Data Analysis

### Tasks Performed
- Loaded the dataset using Pandas
- Performed basic data cleaning
- Checked for missing values and duplicate records
- Generated summary statistics
- Created three visualizations
- Derived insights from the dataset

### Visualizations
- Gender Distribution
- Age Distribution of Students
- Mother's Education Level Distribution

### Key Insights
- Female students slightly outnumber male students.
- Most students belong to the 15–18 age group.
- Very few students are older than 19.
- Mother's education level 4 is the most common category.
- The dataset contained no missing values and only a small number of duplicate records.

## Task 2: Machine Learning Model Comparison

### Tasks Performed
- Reused the same dataset from Task 1
- Encoded categorical features using Label Encoding
- Split data into training and testing sets (80/20, stratified)
- Trained and evaluated 6 classification algorithms to predict student gender:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Naive Bayes
- Compared models using Accuracy, Precision, Recall, and F1-Score
- Visualized model performance with a comparison bar chart
- Generated a confusion matrix for the best-performing model

### Best Model
**SVM** achieved the highest accuracy (~53%), followed closely by Logistic Regression, Decision Tree, and Random Forest (~50% each). KNN and Naive Bayes underperformed.

### Key Insights
- All models achieved accuracy in the 40–53% range, only marginally above random guessing — the dataset's gender split is roughly 53% female / 47% male, so even a majority-class guess would score close to this.
- Family background features (parental education, jobs, school, address type, family size) have very weak predictive power for a student's gender.
- This is a meaningful negative result rather than a model failure — it shows gender isn't meaningfully determined by these demographic factors in this dataset.

## Tools Used
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab
