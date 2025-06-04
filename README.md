# 📄 ApplyPro.ai: LLM-Powered Job Application Assistant

## 🔍 Overview

**ApplyPro.ai** is an AI-powered tool that automates the job application process. It parses resumes, matches them to relevant job postings using semantic search, and generates personalized cover letters and recruiter emails — dramatically reducing manual effort for job seekers while improving match quality and communication.
The process to use the application is described in the flowchart below:
![Solution Architecture](Architecture%20and%20Demo%20Images/Solution%20Architecture.png)

---

## 📊 Dataset

This project uses job posting data from Kaggle:

🔗 [LinkedIn Job Postings – Kaggle Dataset](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings?resource=download)

---

## 🎯 Business Problem
Job seekers often struggle with:
- Manually searching for relevant job roles
- Writing tailored cover letters and recruiter outreach emails
- Poor job-to-resume matching from keyword-based systems

**ApplyPro.ai** solves these inefficiencies by using LLMs and embeddings to automate and personalize every stage of the application workflow.

---

## ⚙️ Features
- 📄 Resume parsing and job matching via semantic embeddings
- 🔍 Vector-based search to recommend best-fit job postings
- ✍️ Personalized cover letter generation using GPT
- 📧 Automated cold email drafting in EML format
- 📁 Output-ready Word and email files for immediate use
- ✅ Simple 2-click user experience with real-time document delivery

---

## 🧰 Tech Stack
- **Language Models**: GPT-3.5 Turbo, BART (facebook/bart-large-cnn)
- **Embedding & Matching**: SentenceTransformers (`nomic-embed-text-v1`) + Cosine Similarity
- **Frameworks**: Python, HuggingFace Transformers
- **Interface**: Streamlit
- **Document Generation**: `python-docx`, `eml`
- **Vector Search**: FAISS (optional)
- **Workflow Modularity**: Agent-based design with modular utility functions

---

## 🚀 How It Works
1. **Upload** your resume (PDF).
![User Interface](Architecture%20and%20Demo%20Images/UI.png)
3. **Match**: Your resume is embedded and compared against job post vectors via cosine similarity.
4. **Generate**: The app outputs the top 3 job matches, a custom cover letter, and a cold email to the recruiter.
![Demo](Architecture%20and%20Demo%20Images/Demo.png)

---

## 📈 Business & User Impact
- 🕒 Cuts manual application time by ~70%
- 🎯 Improves accuracy of job matches using context-aware search
- ✉️ Increases outreach quality through personalized emails and cover letters
- 💡 Helps job seekers focus more on interviews and prep, not repetitive tasks

---

## 🔒 Ethical AI Considerations
- **Bias Mitigation**: Regular audits and fairness checks
- **Transparency**: Explainable match logic and editable outputs
- **Data Privacy**: Secure resume handling with anonymization and encryption
- **User Control**: Full ability to review, edit, and delete generated content

---

## 👥 Contributors
- Jialin You  
- Xinghua Peng  
- Hamza Shahab Shafqat  
- Vishanth Hari Raj Balasubramanian
