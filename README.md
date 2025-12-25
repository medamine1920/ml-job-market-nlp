ML Job Market Intelligence using NLP

OVERVIEW
This project analyzes 1,000 machine learning–related job postings across the United States
(late 2024 – early 2025) and applies Natural Language Processing (NLP) techniques to extract
in-demand technical skills from unstructured job descriptions.

The objective is to understand what skills are required today and how expectations change
by seniority level and location.

This project is framed as a job market intelligence case study similar to how data teams
support hiring strategy, workforce planning, and career guidance.

------------------------------------------------------------

DATASET
Source: Kaggle (ML job postings scraped from company career pages and job boards)
Rows: ~1,000 job postings
Geography: United States

Key columns:
- job_posted_date
- company_address_region (state)
- company_name
- job_title
- seniority_level
- job_description_text

Note: The dataset does not include salary or hiring outcomes. The analysis focuses on
skill demand and role structure.

------------------------------------------------------------

BUSINESS QUESTIONS ANSWERED
- What are the most in-demand machine learning skills?
- How do skill requirements differ by seniority level?
- Which U.S. states show the highest demand for ML roles?
- What skills should junior candidates prioritize?

------------------------------------------------------------

METHODOLOGY

1) Data Cleaning & Preparation
- Removed duplicate job postings
- Parsed and standardized posting dates
- Normalized seniority levels into consistent categories
- Cleaned and normalized job description text for NLP processing

2) NLP Skill Extraction
- Designed a custom machine learning skill taxonomy
- Applied regex-based keyword extraction on job descriptions
- Converted unstructured text into structured skill-level data

3) Analysis & Visualization
- Skill frequency analysis
- Skill demand comparison by seniority
- Geographic analysis by U.S. state
- Time-based job posting trends
- Visualization using Matplotlib

------------------------------------------------------------

KEY INSIGHTS (EXAMPLE)
- Python and SQL dominate ML job requirements across all seniority levels
- Senior roles emphasize Cloud and MLOps skills more than entry-level roles
- ML hiring is geographically concentrated in a small number of states

------------------------------------------------------------

PROJECT STRUCTURE

ml-job-market-nlp/
├── notebook/
│   └── ml_job_market_nlp.ipynb
├── outputs/
│   └── charts/
├── README.txt
├── requirements.txt
└── .gitignore

------------------------------------------------------------

HOW TO RUN
1) Install dependencies:
pip install -r requirements.txt

2) Open the notebook:
jupyter notebook

3) Run all cells from top to bottom.

------------------------------------------------------------

LIMITATIONS & NEXT STEPS
- No salary data available for compensation analysis
- Skill extraction is keyword-based and can be extended with TF-IDF or transformer models
- Potential extensions:
  - Skill trend detection over time
  - Seniority prediction from job descriptions
  - Interactive dashboard (Power BI or Streamlit)

------------------------------------------------------------

AUTHOR
Med Amine Gnichi
Portfolio Project
