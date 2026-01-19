#  Holocaust History Articles Scraper – Python, BeautifulSoup, Pandas

This project automates the scraping of articles related to "Holocaust history" from Google search results, extracts their textual content, and saves the data into a CSV file for further analysis.

---

## **Problem**
Collecting historical articles manually is time-consuming and prone to missing relevant sources. Additionally, web pages may have complex HTML structures, making it difficult to consistently extract textual content without automation.

---

## **Solution**
A Python-based scraper was developed to automate the process:

- **Search Automation:** Uses `googlesearch` to find URLs relevant to the query "Holocaust history articles".  
- **Web Scraping:** Fetches web pages using `requests` and parses the HTML with `BeautifulSoup`. Extracts all text within `<p>` tags.  
- **Error Handling:** Catches network issues and pages without a proper `<body>` tag to ensure robustness.  
- **Rate Limiting:** Includes a 1-second pause (`time.sleep(1)`) between requests to reduce server load and prevent IP blocking.  
- **Data Structuring:** Stores the URL and extracted text in a Python list of dictionaries, which is then converted to a `pandas` DataFrame.  
- **Export:** Saves the final dataset into a CSV file named `Holocaust_ART.csv`.

---

## **Outcome**
- Efficiently collected a structured dataset of Holocaust history articles.  
- Each record contains the **URL** and **full text content** of the article.  
- Provides a reliable dataset ready for further text analysis, NLP processing, or historical research.  

---

##  **Tools & Technologies**
- **Programming Language:** Python  
- **Libraries:** requests, BeautifulSoup, pandas, googlesearch, time  

---
