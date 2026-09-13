# Job Posting Intern Project

A data analytics project exploring global job postings data — from raw extraction and cleaning to a structured data model and an interactive Power BI dashboard. Built as part of an internship to practice the end-to-end analytics workflow: **data collection → cleaning → modeling → visualization → insights**.

## 📌 Overview

This project analyzes job postings to uncover trends in **salaries, required skills, benefits, and languages** across industries, countries, and experience levels. The raw data is cleaned and transformed into a star-schema-style data model, then visualized in an interactive Business Intelligence dashboard.

## 🎯 Objectives

- Clean and structure raw, unstructured job posting data
- Build a relational data model (fact + bridge tables) suitable for BI tools
- Analyze salary trends by experience level, industry, and country
- Identify the most in-demand skills, benefits, and language requirements
- Present findings through an interactive dashboard

## 🗂️ Repository Structure

```
├── BI dash/                          # Power BI dashboard files
├── other/                            # Supporting/misc files
├── data discovery.ipynb              # Exploratory data analysis & cleaning notebook
├── raw_job_postings.(csv/json/xlsx)  # Raw, unprocessed job posting data
├── job_postings_fact.(csv/xlsx)      # Core fact table: one row per job posting
├── job_postings_salary_cleaned.(csv/xlsx)  # Cleaned salary data
├── job_skills_bridge.(csv/xlsx)      # Bridge table: job postings ↔ required skills
├── job_benefits_bridge.(csv/xlsx)    # Bridge table: job postings ↔ benefits offered
├── job_languages_bridge.(csv/xlsx)   # Bridge table: job postings ↔ required languages
└── README.md
```

The data follows a simple **fact + bridge table** design: `job_postings_fact` holds one record per posting (title, company, salary, country, etc.), while the bridge tables map each posting to its associated skills, benefits, and languages — enabling many-to-many analysis (e.g., "which skills appear most often in high-salary postings").

## 🛠️ Tools & Technologies

- **Python** (Pandas, Jupyter Notebook) — data cleaning and exploratory analysis
- **Excel / CSV** — intermediate data storage
- **Power BI** — dashboard design and data visualization

## 📊 Dashboard Highlights

The Power BI dashboard (see `BI dash/`) includes:
- **Salary by Experience Level** — Entry, Mid, and Senior-level salary comparisons
- **Salary by Industry** — average salary breakdown across company industries
- **Salary by Country** — top-paying countries for the roles analyzed
- Interactive filters/slicers for deeper exploration

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/MohamedAminBrahmi/Job-Posting-Intern-Project.git
   ```
2. Explore the data cleaning process in `data discovery.ipynb`
3. Open the dashboard file inside `BI dash/` using Power BI Desktop to interact with the visuals

## 📈 Key Insights

*(Add 2–4 bullet points here summarizing your top findings — e.g., which industries pay the most, which skills correlate with higher salaries, etc.)*

## 👤 Author

**Mohamed Amin Brahmi**
Data Analytics Intern Project

## 📄 License

*(Add a license if you'd like others to know how they can use/reuse this project — e.g., MIT License)*
