
## 📄 Automated Resume Analyzer using Streamlit, NLP, and ML

This project is a **Streamlit web app** that helps recruiters and data science teams analyze single or multiple resumes (PDF/DOCX).
It extracts key information like name, email, and phone, then calculates a **similarity score** between each resume and a provided Job Description (JD).
Results are sorted automatically by score so the best-matching resumes appear first.

---

## ✨ **Features**

✅ Upload one or multiple resumes (batch or single)
✅ Extracts: name, email, phone number (using NLP)
✅ Compares resumes against pasted JD using **TF-IDF + cosine similarity**
✅ Shows final score (%) in a clean table, sorted top-down
✅ Choose job title to load relevant skills and certifications (from dataset)
✅ Simple, interactive web interface built with Streamlit
✅ Modular Python code, easy to extend (e.g., add export, charts)

---

## 📦 **Installation**

1️⃣ Clone this repository or download the code.

2️⃣ Install dependencies:

```bash
pip install -r requirements.txt
```

3️⃣ *(Optional, only first time)* Download NLTK resources:

```python
import nltk
nltk.download('punkt')
nltk.download('maxent_ne_chunker')
nltk.download('averaged_perceptron_tagger')
nltk.download('words')
```

---

## 🚀 **Run the app**

```bash
streamlit run your_script_name.py
```

Replace `your_script_name.py` with your actual Python file.

---

## 🛠 **Project structure**

```bash
.
├── resume_analyzer.py                # Streamlit app
├── IT_Job_Roles_Skills.csv      # Dataset with job roles, skills & certifications
├── requirements.txt
└── README.md
```

---

## 🧠 **How it works**

* User selects a **Job Title** (e.g., "AI Architect")
* Uploads one or many resumes (PDF/DOCX)
* Pastes the Job Description text
* App extracts name/email/phone and computes similarity score
* Displays a sorted table of results (highest scores first)

---

## 📊 **Tech stack**

* Python
* Streamlit
* Pandas
* NLTK (for name/entity extraction)
* scikit-learn (TF-IDF & cosine similarity)
* pdfminer.six & python-docx (for reading PDF/DOCX)

---

## ✅ **To do / ideas**

* Export results to CSV
* Add charts (e.g., score distribution)
* Deploy online (Streamlit Cloud / HuggingFace Spaces / Render)
* Highlight matched skills directly

---

## ❤️ **Credits**

* Built with Python & Streamlit
* Inspired by common recruiter workflows and real-life data challenges

---

## 📬 **Feedback & contributions**

Pull requests, issues, or suggestions are welcome!
Let’s make resume screening smarter and faster together.


