 Titanic Survival Prediction – Machine Learning Project
 Project Overview

This project focuses on predicting passenger survival on the Titanic using historical passenger data. The dataset contains missing values, categorical features, and multiple attributes that require preprocessing and feature engineering before applying machine learning models.

The goal is to identify key factors that influenced survival and build a reliable classification model using Python and machine learning techniques.

 Problem Statement

The Titanic passenger dataset is complex and noisy, containing:

Missing values

Categorical variables

Irrelevant features

These challenges make it difficult to directly analyze survival patterns and train effective machine learning models without proper data preprocessing.

Solution Approach

An end-to-end data science pipeline was developed to:

Clean and preprocess the dataset

Engineer meaningful features

Perform exploratory data analysis (EDA)

Train and evaluate a machine learning model for survival prediction

🛠️ Tools & Technologies

Programming Language: Python

Libraries: Pandas, NumPy, Scikit-learn

Visualization: Matplotlib, Seaborn

 Project Workflow
1. Data Loading

Loaded the titanic_train.csv dataset into a Pandas DataFrame.

2. Initial Data Exploration

Inspected dataset structure using:

df.head()

df.info()

df.describe()

df.shape

Identified missing values using df.isnull().sum().

3. Data Cleaning

Dropped irrelevant or high-missing-value columns:

PassengerId, Cabin, Ticket, Name

Handled missing values:

Imputed Age using median

Imputed Embarked using mode

4. Feature Engineering

Created a new feature FamilySize using:

FamilySize = SibSp + Parch + 1


Captured family-related survival patterns.

5. Categorical Encoding

Converted Sex into numerical format:

Male → 0

Female → 1

Applied one-hot encoding to the Embarked feature.

6. Exploratory Data Analysis (EDA)

Visualized data distributions and relationships using:

Box plots

Count plots

Analyzed survival trends based on age and gender.

7. Model Development

Implemented a Logistic Regression classifier.

Split dataset into training and testing sets (80/20).

8. Model Evaluation

Evaluated model performance using:

Accuracy score

Classification report (precision, recall, F1-score)

9. Data Export

Saved the cleaned and processed dataset as:

cleaned_titanic_data.csv

 Key Insights

Gender and family size significantly influenced survival probability.

Data preprocessing and feature engineering improved model performance.

Logistic Regression provided interpretable and effective results for binary classification.

Conclusion

This project demonstrates a complete data science workflow, from raw data preprocessing to model evaluation. It highlights strong skills in data cleaning, feature engineering, exploratory data analysis, and machine learning model development.
