# Job Skill Analyzer: Data Science & Analytics

A data-driven tool designed to analyze real-time job market trends and skill requirements within the Data Science and Analytics sectors. This application automates the process of fetching, scraping, and visualizing technical demands from active job listings.

## Project Overview
As a **Data Scientist** and **PhD Candidate in Epidemiology at Johns Hopkins University**, I built this analyzer to bridge the gap between academic research and industry requirements. By leveraging the Adzuna API, the tool provides localized insights—specifically targeting areas like **Baltimore, MD** and **Washington DC**—to identify which skills are most valued by employers today.

## Core Features

### 1. Automated Data Pipeline
* **Adzuna API Integration:** Fetches real-time job listings based on specific keywords and regional filters.
* **Deep Scraper:** Uses `cloudscraper` and `trafilatura` to extract full job descriptions, ensuring a more comprehensive skill analysis than basic summaries provide.
* **Title Filtering:** Includes logic to focus strictly on Data Science and Analyst roles while excluding unrelated positions.

### 2. Technical Skill Taxonomy
The analyzer categorizes extracted information into a structured taxonomy, mapping keywords to critical domains:
* **Programming:** Python, SQL, R, SAS, Stata, Java.
* **Stats & Research:** Bayesian Statistics, Causal Inference, Epidemiology, Spatial Analysis.
* **ML & AI:** NLP, LLMs, Deep Learning, Scikit-learn, PyTorch.
* **Cloud & Big Data:** AWS, Azure, Snowflake, Databricks, Spark.
* **Visualization:** Tableau, Power BI, Seaborn, Matplotlib.

### 3. Data Visualization & Export
* **Dynamic Dashboard:** Built with Streamlit to display high-fidelity bar charts of skill frequency.
* **Market Insights:** Calculates the percentage of job postings that mention specific technologies to highlight "must-have" skills.
* **Data Portability:** Allows users to download the full analyzed dataset as a CSV for further exploration.

## Tech Stack
* **Language:** Python
* **Framework:** Streamlit
* **Data Handling:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Web Scraping:** Trafilatura, Cloudscraper
* **API/Networking:** Requests, Pyngrok

## Impact
This project demonstrates the ability to deploy an end-to-end data product—from API handling and NLP-based text parsing to user-facing visualization—providing actionable intelligence for career development in technical fields.