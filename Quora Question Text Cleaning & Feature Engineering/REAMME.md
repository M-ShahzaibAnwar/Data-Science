#  Quora Question Text Cleaning & Feature Engineering – Python, Pandas, Regex, NLTK

This project focuses on **text preprocessing and feature engineering** for a Quora question pairs dataset. The goal is to clean the textual data, apply NLP techniques like stemming and lemmatization, and create additional features to facilitate downstream analysis or machine learning tasks.

---

## **Problem**
Raw text data often contains noise such as missing values, special characters, inconsistent casing, and duplicate words. In the context of Quora question pairs, these issues make it challenging to:  

- Compare question similarity accurately  
- Extract meaningful features for modeling  
- Maintain consistent and clean textual datasets  

---

## **Solution**
A systematic text preprocessing and feature engineering pipeline was implemented:

- **Data Loading:** Loaded `q_quora.csv` into a Pandas DataFrame.  
- **Column Cleaning:** Removed irrelevant 'Unnamed' columns.  
- **Missing Value Handling:** Dropped rows with missing values in `question1` or `question2`.  
- **Text Lowercasing:** Converted all text in `question1` and `question2` to lowercase.  
- **Text Cleaning (Regex):** Removed special characters, reduced multiple spaces to a single space, and trimmed leading/trailing spaces.  
- **Stemming:** Created `question1_stemmed` and `question2_stemmed` using **Porter Stemmer** to reduce words to their root form.  
- **Lemmatization:** Created `question1_lemmatized` and `question2_lemmatized` using **WordNet Lemmatizer** to reduce words to their base form.  
- **Duplicate Word Removal:** Created `question1_no_duplicates` and `question2_no_duplicates` by removing repeated words within each question.  
- **Feature Engineering:**  
  - `q1_length` & `q2_length`: Lengths of cleaned questions  
  - `common_words`: Number of shared words between question1_no_duplicates and question2_no_duplicates  
  - `same_start`: Boolean flag indicating if both questions start with the same word  

- **Data Export:** Saved the enhanced dataset with all new features as `q_quora_regix.csv`.

---

## **Outcome**
- Cleaned and normalized Quora question text suitable for NLP tasks.  
- Added meaningful features for similarity detection or machine learning models.  
- Demonstrated practical skills in **text preprocessing, NLP, feature engineering, and Pandas data manipulation**.

---

##  **Tools & Technologies**
- **Programming Language:** Python  
- **Libraries:** Pandas, Regex, NLTK (Porter Stemmer, WordNet Lemmatizer)  
- **Techniques:** Text Cleaning, Stemming, Lemmatization, Duplicate Removal, Feature Engineering  

---

## **Key Insights**
- Preprocessing raw text is crucial for accurate NLP analysis.  
- Stemming and lemmatization reduce word variations and improve consistency.  
- Engineered features like `common_words` and `same_start` can provide additional signals for similarity modeling.
