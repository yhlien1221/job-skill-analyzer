# Job Skill Analyzer

A Streamlit-based application that analyzes recent job postings in a given U.S. city
and extracts the most in-demand skills for Data Scientist and Data Analyst roles.

This project is designed to help job seekers identify skill gaps, prioritize learning,
and better align their technical skills with current job market demand.

---

## Features

- Search job postings by **city**, **job title**, and **posting date**
- Fetch recent job data using a **legal job posting API (Adzuna)**
- Automatically extract technical skills from job descriptions
- Visualize skill demand using interactive charts
- View and download raw job data and aggregated skill results

---

## Tech Stack

- **Programming Language:** Python  
- **Web App Framework:** Streamlit  
- **Data Processing:** Pandas  
- **Job Data Source:** Adzuna Job Search API  
- **Visualization:** Streamlit built-in charts  
- **Configuration Management:** dotenv  

---

## Project Structure

job-skill-analyzer/
├── app.py              # Streamlit main application
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation
├── .gitignore
├── .env.example        # Environment variable template
├── data/
│   ├── jobs_raw.csv    # Raw job postings
│   └── skill_frequency.csv # Aggregated skill frequency
├── src/
│   ├── __init__.py
│   ├── fetch_jobs.py   # Fetch jobs from Adzuna API
│   ├── skill_extractor.py # Extract skills
│   └── utils.py        # Shared helper functions
└── notebooks/
    └── exploration.ipynb # Optional exploratory analysis



---

## How It Works

1. The user selects a city, job title(s), and a minimum posting date in the Streamlit UI.
2. The application queries the Adzuna API to retrieve relevant job postings.
3. Job descriptions are processed to identify predefined technical skills.
4. Skill frequencies are aggregated and visualized.
5. Results can be exported as CSV files for further analysis.

---

## How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/your-username/job-skill-analyzer.git
cd job-skill-analyzer

## 2. Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # macOS / Linux
# venv\Scripts\activate    # Windows

## 3. Install dependencies
pip install -r requirements.txt

## 4. Configure environment variables
cp .env.example .env

### Add your Adzuna API credentials:
ADZUNA_APP_ID=your_app_id
ADZUNA_APP_KEY=your_app_key

## 5. Run the Streamlit app
streamlit run app.py


## A job seeker targeting Data Scientist roles in Baltimore can:

* Analyze postings from the last 30–60 days

* Identify the most frequently required skills (e.g., Python, SQL, AWS)

* Compare those requirements against their current skill set

* Prioritize which skills to develop next

## Output
* jobs_raw.csv (Raw job postings that match the search criterias)
* skill_frequency.csv (Aggregated skill demand across job postings)

## Author
* Created by Yu-Hui Lien