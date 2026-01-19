#  Diabetes Prediction – Python, Scikit-learn, SVM & Logistic Regression

This project builds machine learning models to predict the likelihood of diabetes based on multiple health indicators. It demonstrates a complete data science workflow, including data exploration, preprocessing, modeling, evaluation, and visualization.

---

## **Problem**
Diabetes is a prevalent health concern, and early detection can significantly improve outcomes. The dataset contains several health features, but challenges include:

- Imbalanced target variable (`Outcome`), with more non-diabetic than diabetic cases  
- Features with different scales, requiring standardization  
- Need for interpretable models to predict diabetes risk  

---

## **Solution**
An end-to-end workflow was implemented to predict diabetes:

- **Data Loading & Exploration:** Loaded `diabetes.csv` and examined shape, descriptive statistics, null values, and class imbalance in the `Outcome` variable.  
- **Data Preprocessing:**  
  - Separated features (X) and target (Y)  
  - Standardized features using `StandardScaler` to ensure equal contribution to models  
- **Data Splitting:** Divided the dataset into training (80%) and testing (20%) sets, maintaining class proportions (`stratify=Y`)  
- **Model Training & Evaluation (SVM):**  
  - Trained a Support Vector Machine with a linear kernel  
  - Achieved ~78.5% accuracy on training data and ~76.6% on test data  
  - Demonstrated predictions on new unseen data  
- **Model Training & Evaluation (Logistic Regression):**  
  - Trained and evaluated Logistic Regression as an alternative  
  - Achieved ~78.3% training accuracy and ~75.3% test accuracy  
- **Data Visualization:**  
  - Scatter plots of `Glucose` vs `Insulin` colored by `Outcome`  
  - Box plots and histograms for feature distributions  
  - Correlation heatmap to analyze relationships between attributes  

---

## **Outcome**
- Developed machine learning models capable of predicting diabetes risk from health indicators.  
- Standardization and preprocessing improved model performance and stability.  
- Visualizations helped interpret feature relationships and class separability.  
- Demonstrated ability to apply both **SVM** and **Logistic Regression** to a real-world health dataset.

---

##  **Tools & Technologies**
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Techniques:** Data Preprocessing, Standardization, Train-Test Split, SVM, Logistic Regression, Data Visualization  

---

## **Key Insights**
- Features such as `Glucose` and `Insulin` are strong indicators of diabetes.  
- Standardizing data ensures balanced contributions from all features in machine learning models.  
- Both SVM and Logistic Regression provide interpretable and effective results for binary classification problems.  
