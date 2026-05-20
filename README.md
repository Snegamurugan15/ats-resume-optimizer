# ATS Resume Optimizer

A Streamlit app that helps tailor a resume and cover letter to a job description, estimate keyword coverage, and optionally save generated documents to Google Drive.

## Features

- Upload a resume as PDF or DOCX.
- Paste a full job description and role details.
- Estimate an ATS-style keyword match score.
- Generate an optimized resume and matching cover letter as DOCX files.
- Optionally save outputs to a configured Google Drive folder.

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

## Run

```bash
streamlit run app.py
```

Open the local URL shown by Streamlit, usually `http://localhost:8501`.

## Configuration

The app asks for credentials in the sidebar at runtime:

- Claude API key from Anthropic.
- Optional Google Drive service-account JSON.
- Optional Google Drive folder ID.

Do not commit API keys, service-account JSON, generated resumes, or private job-application documents to the repository. For deployed Streamlit apps, prefer Streamlit secrets or environment variables over hard-coded credentials.

## Deployment

See [DEPLOY_GUIDE.md](DEPLOY_GUIDE.md) for Streamlit Cloud deployment notes.

## Disclaimer

This is a productivity tool for resume drafting and keyword review. Generated content should be checked manually for truthfulness, formatting, and fit before use.
