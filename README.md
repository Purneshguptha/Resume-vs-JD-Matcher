
# 📄 Resume vs Job Description Matcher

This project automatically evaluates the **semantic similarity** between a resume and a job description (JD) using **NLP techniques** — specifically **TF-IDF** and **BERT embeddings** with cosine similarity.

## 🚀 Features
- ✅ Read text directly from **PDF** resume and JD files.
- ✅ Compare semantic similarity using:
  - **TF-IDF + Cosine Similarity**
  - **BERT (Sentence Transformers) + Cosine Similarity**
- ✅ Clean, minimal, and beginner-friendly code.

## 🛠️ Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
```

**Or individually:**

```bash
pip install PyMuPDF scikit-learn sentence-transformers
```

## 📁 File Structure

```
resume_vs_jd_matcher.ipynb     # Jupyter notebook for resume-JD similarity
resume.pdf                     # Input resume file
jd.pdf                         # Input job description file
README.md                      # Project documentation
requirements.txt               # Dependencies list
```

## 📌 How It Works

1. **Extract Text from PDFs**  
   Uses `PyMuPDF` to extract raw text from `resume.pdf` and `jd.pdf`.

2. **TF-IDF Similarity**  
   Vectorizes the resume and JD, then computes cosine similarity between them.

3. **BERT Embedding Similarity**  
   Uses `SentenceTransformer` to get deep semantic embeddings, then computes cosine similarity.

## 🧪 Sample Output

```
--- TF-IDF Similarity ---
TF-IDF Similarity Score: 0.5821

--- BERT Embedding Similarity ---
BERT Similarity Score: 0.8643
```

## 🧠 Future Improvements
- Add support for comparing **multiple resumes and JDs**
- Create a **Streamlit web interface**
- Include **skill extraction and keyword matching**

## 📜 License
This project is open source and free to use under the MIT License.
