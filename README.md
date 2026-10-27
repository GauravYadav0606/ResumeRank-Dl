# ResumeRank – AI-Based Resume Screening and Ranking System

ResumeRank is a Python-based web application that helps HR professionals screen and rank resumes according to a given job description using Natural Language Processing (NLP) and semantic similarity.

## Features

- Upload resumes in PDF and DOCX formats.
- Compare resumes with a job description.
- Generate semantic similarity scores.
- Rank candidates based on matching scores.
- Categorize candidates as Potential Match or Low Similarity.
- View HR analysis charts.
- Export screening results as CSV.

## Tech Stack

- Python
- Streamlit
- Sentence Transformers
- Scikit-learn
- Pandas
- Plotly
- PyMuPDF
- python-docx

## Run Locally

Install the required libraries:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run app.py
```

## How It Works

1. Enter the job description.
2. Upload candidate resumes.
3. The application extracts resume text.
4. Semantic similarity scores are calculated.
5. Candidates are ranked and results can be exported.

## Disclaimer

ResumeRank is a screening assistance tool. Similarity scores should not be used as the sole basis for hiring decisions.

## Author

Gaurav Yadav
