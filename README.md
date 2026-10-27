# ResumeRank – AI-Based Resume Screening and Ranking System

ResumeRank is an AI-powered web application that helps recruiters screen and rank resumes according to a job description using Natural Language Processing (NLP) and semantic similarity.

## 🚀 Features

- Upload resumes in PDF and DOCX formats.
- Compare resumes with a job description.
- Calculate semantic similarity scores.
- Rank candidates based on matching scores.
- Categorize candidates as Potential Match or Low Similarity.
- Visualize candidate analysis using charts.
- Export screening results as CSV.

## 🛠️ Tech Stack

- Python
- Streamlit
- Sentence Transformers
- Scikit-learn
- Pandas
- Plotly
- PyMuPDF
- python-docx

## 📂 Project Structure

```text
ResumeRank/
├── app.py
├── requirements.txt
└── README.md
```

## 🌐 Try the Live Demo

**Live Application:** https://resumerank-dl-qdhbqpqyjdtzkmtrhohxgr.streamlit.app/

The live demo will be available after the application is successfully deployed on Streamlit Community Cloud.

## 💻 Run the Project on Your Computer

### 1. Install Python

Install Python from https://www.python.org/downloads/

Python 3.11 is a recommended starting point. During installation on Windows, enable **Add Python to PATH**.

### 2. Download the Project

On this GitHub repository page, click **Code → Download ZIP**.

Extract the ZIP file and open the extracted project folder.

Alternatively, clone the repository:

```bash
git clone https://github.com/GauravYadav0606/ResumeRank.git
cd ResumeRank
```

### 3. Open a Terminal

Open Command Prompt or PowerShell inside the project folder containing `app.py`.

### 4. Create a Virtual Environment (Recommended)

**Windows:**

```bash
py -m venv .venv
.venv\Scripts\activate
```

**macOS/Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 5. Install Dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

The first installation may take some time because the machine-learning libraries and model may be large.

### 6. Run the Application

```bash
streamlit run app.py
```

The terminal will display a local URL, usually:

`http://localhost:8501`

Open that URL in your web browser to use ResumeRank.

## ⚙️ How It Works

1. Enter the job description.
2. Upload candidate resumes.
3. The application extracts text from the uploaded files.
4. Sentence Transformers generates text embeddings.
5. Cosine similarity is used to compare resumes with the job description.
6. Candidates are ranked according to similarity scores.
7. View the analysis and download results as CSV.

## 🧠 NLP Model

The application uses:

`sentence-transformers/bert-base-nli-mean-tokens`

The model may download automatically when first used, so an internet connection may be required.

## 📊 Candidate Categories

- **Potential Match:** Similarity score of 50% or higher.
- **Low Similarity:** Similarity score below 50%.

These categories are based on the application's configured threshold and do not guarantee candidate suitability.

## ⚠️ Limitations

- Scanned PDFs may not produce readable text if OCR is not supported.
- Results depend on the quality and content of the uploaded resumes.
- Similarity scores should not be treated as definitive hiring decisions.
- Test the project in a fresh Python environment before relying on the installation instructions.

## 🔒 Privacy Notice

Use sample or authorized resumes when testing. Avoid uploading confidential candidate information to public repositories or public demos.

## 👨‍💻 Author

**Gaurav Yadav**

## 📄 License

No open-source license has been specified yet. All rights remain with the copyright holder unless a license is added.
