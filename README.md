# 🎯 Job Skill Analyzer: Data Science & Analytics

A professional-grade market intelligence tool designed to quantify technical requirements in the data science and analytics sectors. By combining **Adzuna API** integration with **Deep Web Scraping**, this tool bypasses brief job snippets to analyze full job descriptions, providing a high-fidelity map of the current hiring landscape.

## 📖 Project Overview
This project was developed to provide granular insights into the evolving requirements of Data Science roles. Unlike standard job search engines, this analyzer uses **Advanced Regular Expressions (Regex)** and **automated web scraping** to extract "hidden" requirements—such as specific statistical methodologies, cloud deployment tools, and security clearances—that are often omitted in search result summaries.

## 🚀 Key Features

### 1. Seniority-Level Filtering
* **Automated Classification**: Integrates custom logic to classify roles into `Principal`, `Senior`, or `Junior` tiers based on job title keywords.
* **Targeted Comparison**: Enables users to isolate and compare the technical stack expected at different career stages.

### 2. Deep Web Scraping & Content Extraction
* **Full-Text Retrieval**: Utilizes `cloudscraper` and `trafilatura` to navigate beyond API summaries and retrieve the full text from original job postings.
* **Intelligent Fallback**: Implements a robust mechanism that reverts to API snippets only if deep scraping is blocked, ensuring a continuous data flow.

### 3. Intelligent Experience Binning
* **Dynamic Extraction**: Replaces static keyword matching with a dynamic **Regex engine** that identifies years of experience mentioned anywhere in the job description.
* **Standardized Categorization**: Automatically categorizes raw numerical data into standardized buckets: `0-2 years`, `3-5 years`, `5-8 years`, and `8+ years`.

### 4. Robust Data De-duplication
* **Unique Entry Enforcement**: Implements a `Dictionary-based` storage system that identifies unique Job IDs, ensuring that duplicate postings across different search keywords are only counted once.
* **Data Integrity**: Guarantees that the "Total" job count and the "N" sample size are mathematically consistent with the exported CSV dataset.

### 5. Advanced Market Visualization
* **Analytics Dashboard**: Generates a high-impact, multi-panel dashboard using `Seaborn` and `Matplotlib`.
* **Statistical Insights**: Calculates the relative frequency (%) of specific skills, helping users distinguish between "Core Requirements" and "Nice-to-Have" skills.

## 🛠️ Tech Stack
* **Language**: Python 3.9+
* **Web Framework**: Streamlit
* **Data Engineering**: Pandas, NumPy
* **Scraping Infrastructure**: Cloudscraper, Trafilatura
* **Text Processing**: Regular Expressions (Regex)
* **Visualization**: Matplotlib, Seaborn

## 📈 Impact & Insights
This tool provides a quantitative edge for navigating the data science job market:
* **Trend Detection**: Successfully identifies the rising prevalence of **Generative AI**, **LLMs**, and **RAG** technologies in Senior and Principal roles.
* **Localized Intelligence**: Optimized for the **Baltimore/Washington D.C.** market, highlighting the specific dominance of AWS and Spark in the region's tech stack.

## 🛠️ How to Use
1. Enter your **Adzuna API Credentials** in the sidebar.
2. Select your target **Locations** and **Position Level**.
3. Set the **Max Pages** to define the depth of the search.
4. Execute **"Start Deep Analysis"** to view live visualizations and download the refined CSV dataset.

---