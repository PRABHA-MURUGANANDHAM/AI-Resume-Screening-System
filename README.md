AI Resume Screening System

A web-based application built with Streamlit that allows recruiters to upload a job description and multiple resumes (PDFs) and automatically ranks candidates based on their skills and relevance. The system highlights key skills in the resumes and identifies the best candidate.

Features

Upload Job Description (text input)

Upload multiple resumes in PDF format

Automatic candidate ranking based on resume-job description matching

Extracts and highlights top 5–6 relevant skills from resumes

Displays the best candidate with a badge

Simple, clean, and interactive UI

Tech Stack

Python 3.x

Streamlit (UI)

PyPDF2 (PDF text extraction)

scikit-learn (cosine similarity for matching)

Requests (API calls to embeddings API)

Gemini AI API for embedding generation

Installation

Clone the repository:

git clone https://github.com/username/ai-resume-screening.git
cd ai-resume-screening


Install dependencies:

pip install -r requirements.txt


Run the Streamlit app:

streamlit run app.py

Usage

Open the app in your browser.

Paste or type the Job Description.

Upload one or more resumes (PDF).

Click Analyze Candidates.

View the candidate ranking, matched skills, and the best candidate badge.

Configuration

Set your Gemini API key in the script:

GEMINI_API_KEY = "YOUR_API_KEY_HERE"
GEMINI_EMBEDDING_URL = "https://api.gemini.ai/v1/embeddings"


Ensure your API key is kept secret (do not push it to GitHub).

Folder Structure
ai-resume-screening/
│
├── app.py                  # Main Streamlit application
├── requirements.txt        # Python dependencies
├── sample_resumes/         # Optional folder for demo PDF resumes
└── README.md               # Project documentation

Future Improvements

Multi-language support for resumes

More advanced skill extraction and matching

Integration with LinkedIn profiles

Real-time API-based scoring for large-scale recruitment
