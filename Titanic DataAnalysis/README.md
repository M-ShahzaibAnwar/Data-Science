#  Titanic Survival Prediction – Machine Learning Project

This project predicts passenger survival on the Titanic using historical passenger data. The dataset contains missing values, categorical variables, and irrelevant features, making it challenging to directly analyze survival patterns or build effective models.

---

## **Problem**
The Titanic dataset is noisy and incomplete. Key challenges include:  

- Missing values in `Age` and `Embarked` columns  
- Categorical data like `Sex` and `Embarked`  
- Irrelevant features such as `PassengerId`, `Ticket`, `Name`, and `Cabin`  

Without proper preprocessing, these issues make it difficult to identify the factors influencing survival and to train reliable machine learning models.

---

## **Solution**
An end-to-end machine learning pipeline was implemented to address these challenges:

- **Data cleaning:** Handle missing values in `Age` and `Embarked`, and remove irrelevant columns.  
- **Feature engineering:** Create a new feature, *FamilySize*, by combining `SibSp` (siblings/spouses aboard) and `Parch` (parents/children aboard) to capture family-related survival patterns.  
- **Categorical encoding:** Convert `Sex` into numerical format and apply one-hot encoding to `Embarked`.  
- **Exploratory Data Analysis (EDA):** Visualize distributions and relationships using box plots and count plots to uncover survival trends.  
- **Model development:** Train a Logistic Regression classifier on the processed dataset.  
- **Model evaluation:** Measure performance using accuracy and classification metrics.

---

## **Outcome**
The model successfully identifies key factors influencing passenger survival, such as **gender** and **family size**.  

This project demonstrates strong skills in **data preprocessing**, **feature engineering**, **exploratory analysis**, and **machine learning model development**, providing a practical example of applying data science to solve real-world problems.

---

##  **Tools & Technologies**
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Visualization:** Matplotlib, Seaborn  

