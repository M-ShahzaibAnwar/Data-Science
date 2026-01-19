#  Comparative Analysis of Patient Selection Strategies  Python, Genetic Algorithms

This project compares two patient selection strategies—**Roulette Wheel Selection** and **Random Selection**—using a calculated 'Fit_Score' derived from normalized physiological and clinical attributes. The goal is to evaluate how probability-based selection methods bias toward patients with higher suitability scores compared to random sampling.

---

## **Problem**
In patient selection for treatments or clinical studies, it is important to identify individuals most suited based on health indicators. Traditional random selection does not prioritize higher-fit individuals, while probability-based methods like Roulette Wheel can introduce bias towards patients with better health metrics.  

Challenges include:  
- Handling diverse physiological and clinical features (e.g., Age, Blood Pressure, BMI, LDL, HDL)  
- Creating a composite metric to quantify patient suitability  
- Comparing outcomes of different selection strategies  

---

## **Solution**
An end-to-end data analysis and selection pipeline was implemented:

- **Data Preprocessing & Normalization:** Loaded a patient dataset and applied **MinMaxScaler** to normalize critical features ensuring consistent scaling.  
- **Feature Engineering:** Developed a **custom 'Fit_Score'** by assigning weighted importance to normalized attributes, representing patient health or suitability.  
- **Implementation of Selection Algorithms:**  
  - **Roulette Wheel Selection:** Probabilistic selection where patients with higher Fit_Scores have a greater chance of being selected.  
  - **Random Selection:** Baseline random sampling for comparison.  
- **Comparative Analysis & Visualization:** Compared the distribution of Fit-Scores from both methods using **Matplotlib histograms** to illustrate biases and outcomes of each selection strategy.  

---

## **Outcome**
- Demonstrated how probability-based selection (Roulette Wheel) prioritizes higher-fit patients compared to random selection.  
- Visualizations highlighted the difference in score distributions between the two strategies.  
- Showcases skills in **data preprocessing, feature engineering, probability-based algorithms, and data visualization**.  

---

##  **Tools & Technologies**
- **Programming Language:** Python  
- **Libraries:** Pandas, Scikit-learn (MinMaxScaler), Matplotlib  
- **Techniques:** Data Normalization, Feature Engineering, Probability-based Selection Algorithms, Comparative Analysis, Data Visualization  


