
title: "ATS Resume Score Checker using Gemini 1.5"
date: 2025-04-19 12:00:00 +0530
categories: [AI Tools, NLP]
tags: [gemini, ats, resume, huggingface, streamlit, vision, nlp]
pin: true


🚀 I built and deployed an **AI-powered ATS Resume Score Checker** using [Google Gemini 1.5](https://ai.google.dev/) and deployed it on [Hugging Face Spaces](https://huggingface.co/spaces)!



## 📌 Project Overview

**ATS (Applicant Tracking Systems)** are widely used to screen resumes before human eyes even see them. This tool simulates an ATS system — it evaluates your resume (in PDF form) against a job description and:

- 📊 Gives a **match percentage**
- 🧠 Lists **missing keywords**
- 💡 Provides **feedback & suggestions**

The system uses **Gemini 1.5 Flash** to process and understand the content of uploaded resumes and compare them to job requirements using natural language understanding.



## 🧩 Workflow

1. **User Enters Job Description**  
   - Text area input via Streamlit.

2. **User Uploads Resume (PDF)**  
   - Only `.pdf` files accepted.
   - First page is extracted using `pdf2image` and converted to a JPEG image.

3. **PDF → Image → AI**  
   - The first page of the resume is converted into a base64 JPEG and passed to Google Gemini 1.5.

4. **Gemini Model Evaluation**  
   - Two prompt options:
     - 🧠 *Resume Quality Evaluation*
     - 📊 *ATS Match Percentage*

5. **Output Display**  
   - Streamlit displays Gemini’s response: percentage match, missing keywords, strengths/weaknesses, and improvement tips.



## 🛠 Tech Stack

- **Frontend**: Streamlit
- **Backend AI**: Google Gemini 1.5 Flash (via GenerativeAI API)
- **Deployment**: Hugging Face Spaces
- **PDF Parsing**: `pdf2image` + `PIL`



## 💻 Live Demo

👉 Try the app here: [ATS Resume Checker on Hugging Face](https://your-hugging-face-link.hf.space)

🧠 Source code available here: [GitHub Repo](https://github.com/yourusername/ats-resume-checker)



## 📸 Screenshots

_Add screenshots or a short GIF of your app in action here_



## ✅ What I Learned

- How to use **Gemini 1.5 Vision** for multi-modal AI (text + image input)
- Building full AI apps with **Streamlit**
- Deploying AI apps on Hugging Face Spaces
- Understanding how **ATS systems** parse resumes



## 🚀 Next Features (Coming Soon)

- Support for **multi-page resumes**
- Downloadable **PDF reports**
- Enhanced feedback using **keyword highlighting**
- Resume **section-by-section evaluation**



Thanks for reading! Feel free to [connect with me on LinkedIn](https://www.linkedin.com/in/your-profile) or star the repo on GitHub ⭐
