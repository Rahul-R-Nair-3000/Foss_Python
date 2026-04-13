# 📄 AI Resume Analyzer
### FOSSEE Internship Screening — UI/UX Enhancement with Streamlit

---

## 🚀 Quick Start

```bash
# 1. Clone / download the project
cd resume-analyzer

# 2. (Recommended) Create a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
streamlit run app.py
```

The app opens at **http://localhost:8501** in your browser.

---

## 📦 Dependencies

| Library | Purpose |
|---|---|
| `streamlit` | Web UI framework |
| `pdfplumber` | PDF text extraction |
| `python-docx` | DOCX text extraction |
| `plotly` | Interactive charts (gauge, radar, bar) |
| `reportlab` | PDF report generation |

---

## ✨ Features

- **File Upload** — PDF and DOCX support with error handling
- **Section Detection** — Education, Experience, Skills, Projects, Achievements, Summary, Contact
- **Skill Extraction** — ~100 skills across 7 categories (regex word-boundary matching)
- **Resume Scoring** — Transparent 5-dimension, 100-point scoring system
- **Improvement Suggestions** — Colour-coded high / medium / strength tips
- **Charts** — Score gauge, dimension radar, skills bar chart (Plotly)
- **Download Report** — Full PDF report via ReportLab
- **Dark editorial UI** — Syne + DM Sans typography, teal accent palette

---

## 🗂 Project Structure

```
resume-analyzer/
├── app.py            ← Single-file Streamlit application
├── requirements.txt  ← Python dependencies
└── README.md         ← This file
```

---

## 📐 Scoring Weights

| Dimension | Max Points |
|---|---|
| Sections completeness | 30 |
| Skills breadth | 25 |
| Contact information | 15 |
| Action/power verbs | 15 |
| Detail / word count | 15 |
| **Total** | **100** |

---

## 🖥 Screenshots (pages)

1. **Analyzer** — Upload → Score gauge + radar → Skills tab → Sections grid → Suggestions → Raw text
2. **How It Works** — Step-by-step pipeline explanation
3. **About** — Project info and tech stack

---

*Built with Python · Streamlit · Plotly · ReportLab*
