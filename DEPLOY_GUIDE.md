# ATS Resume Optimizer — Streamlit Setup Guide

## Option A — Run Locally on Your Mac (5 minutes)

### 1. Install Python (if not already)
Download from https://python.org/downloads → install

### 2. Open Terminal on your Mac
Press `Cmd + Space` → type `Terminal` → Enter

### 3. Install dependencies
```bash
cd "path/to/Job Application/ATSResumeApp"
pip install -r requirements.txt
```

### 4. Run the app
```bash
streamlit run app.py
```
Your browser opens automatically at `http://localhost:8501`

---

## Option B — Deploy Free Online (access from any device including phone)

### 1. Create GitHub account
Go to https://github.com → Sign Up (free)

### 2. Create a new repository
- Click the **+** button → New repository
- Name: `ats-resume-optimizer`
- Set to **Private**
- Click **Create repository**

### 3. Upload your files
Click **"uploading an existing file"** → drag in `app.py` and `requirements.txt` → Commit

### 4. Deploy on Streamlit Cloud (free)
1. Go to https://share.streamlit.io → Sign in with GitHub
2. Click **"New app"**
3. Repository: `ats-resume-optimizer`
4. Main file: `app.py`
5. Click **Deploy**

Wait ~2 minutes → you get a public URL like `https://ats-resume-snega.streamlit.app`

Open that link on your phone — it works perfectly in mobile browser!

---

## How to Use the App

1. **Sidebar** → paste your Claude API key (from console.anthropic.com)
2. **Sidebar** → paste your Google Drive Service Account JSON (from Step 4 of BUILD_GUIDE)
3. **Sidebar** → paste your Drive Folder ID (from your Drive folder URL)
4. Upload your resume (PDF or DOCX)
5. Enter company name + role title
6. Paste the full job description
7. Click **✨ Optimize My Resume**

### What you get:
- ATS Score (animated, with colour coding)
- Resume DOCX — download button
- Cover Letter DOCX — download button
- Both auto-saved to Google Drive as "CompanyName – RoleName"
- Keyword match analysis (green = matched, red = gaps)
- Improvement summary with certification recommendations

---

## Finding Your Drive Folder ID

1. Go to Google Drive
2. Open your `ATS Resume Outputs` folder (the one you shared with the service account)
3. Look at the URL: `https://drive.google.com/drive/folders/ABC123xyz`
4. The part after `/folders/` is your Folder ID → paste that in the sidebar

---

## No Google Drive? That's Fine!

Leave the Service Account JSON empty — the app still works perfectly.
You'll get download buttons to save files directly to your phone/Mac.
