#  Student Performance Clustering – Python, Pandas, Scikit-learn

This project applies **K-Means clustering** to student performance data to identify distinct groups based on their **math** and **reading** scores. The goal is to uncover patterns in student performance and segment students into meaningful clusters for analysis.

---

## **Problem**
Student performance data contains multiple features, making it difficult to identify natural groupings or patterns. Specifically:  

- Students have varied scores in **math** and **reading**  
- No predefined categories exist for grouping students  
- Manual identification of performance clusters is time-consuming and subjective  

---

## **Solution**
An end-to-end clustering workflow was implemented to segment students:

- **Data Loading & Preparation:** Loaded the `StudentsPerformance.csv` dataset using Pandas and selected **math score** and **reading score** as features for clustering.  
- **K-Means Clustering:** Applied the **K-Means algorithm** from Scikit-learn to cluster students into a specified number of groups (e.g., 3 clusters).  
- **Results Visualization:** Visualized the clustering results and centroids using **Matplotlib** and **Seaborn** to clearly interpret student groupings.  
- **Analysis:** Interpreted the clusters to understand which students are high-performing, average, or need additional support.

---

## **Outcome**
- Successfully segmented students into distinct performance groups based on scores.  
- Provided visual insights into student clusters for better understanding and decision-making.  
- Demonstrated practical application of **unsupervised learning** and **data visualization** techniques.

---

##  **Tools & Technologies**
- **Programming Language:** Python  
- **Libraries:** Pandas, Scikit-learn, Matplotlib, Seaborn  
- **Techniques:** K-Means Clustering, Data Preprocessing, Visualization, Unsupervised Learning  

---

## **Key Insights**
- K-Means effectively identifies natural groupings in student performance data.  
- Visualization of clusters and centroids provides actionable insights for educators or analysts.  
- This project demonstrates practical skills in **clustering**, **data analysis**, and **visualization**.
