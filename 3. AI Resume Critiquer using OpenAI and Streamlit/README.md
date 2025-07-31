# AI-Powered Resume Critiquer using OpenAI and Streamlit

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

![Libraries](https://img.shields.io/badge/Libraries-OpenAI%2C%20Streamlit-orange.svg)

## 📝 Overview

This project provides an interactive web app for AI-powered resume feedback using [Streamlit](https://streamlit.io/) and the [OpenAI API](https://platform.openai.com/). Users can upload their resume in PDF or text format, optionally specify a target job role, and receive detailed, tailored suggestions to optimize their resume. The system analyzes the content and returns actionable insights on various aspects such as clarity, skills, experience, and job alignment.

## ✨ Features

- **AI-Powered Analysis:** Uses the `gpt-4o-mini` model to provide expert-level feedback on resumes.
- **Multi-Format Resume Upload:** Supports both PDF and TXT resume uploads for maximum flexibility.
- **Job Role Customization:** Lets users specify the target job role to get feedback tailored to their career goals.
- **Comprehensive AI Feedback:** Uses the OpenAI GPT-4o-mini model to deliver structured and practical resume improvement recommendations.
- **Streamlit User Interface:** Offers a simple, accessible browser-based experience with live feedback.
- **Error Handling:** Checks for empty or invalid uploads and guides the user accordingly.
- **Secure Key Management:** Leverages environment variables to keep API keys secure.


## 🛠️ Installation

Install the required dependencies in your Python environment:

```bash
pip install streamlit openai PyPDF2 python-dotenv
```

> The app is designed to run on your local machine. Please ensure you have set your OpenAI API key in a `.env` file or as an environment variable (`OPENAI_API_KEY`) before starting.

## 🚀 Usage

1. **Clone or download** this repository and open the notebook or script: `ChatGPT_based_resume_critiquer.ipynb`
2. **Set your OpenAI API key** as an environment variable or in a `.env` file.
3. **Run the Streamlit app:**

```bash
streamlit run ChatGPT_based_resume_critiquer.ipynb
```

4. **Upload your resume** (PDF or TXT) via the browser UI.
5. **(Optional) Specify your target job role.**
6. **Click "Analyze Resume"** to receive AI-generated feedback.

### Example

```
Upload your resume (pdf or txt): champ_resume.pdf
Enter the job role you are targeting (optional): Data Analyst
[Analyze Resume]

### Analysis Results

Resume Analysis for Bruce Wayne

1. Content Clarity and Impact

   Strengths:
   - The summary section communicates enthusiasm and a foundational understanding of data analysis concepts.
   - Projects provide valuable practical insights.
   ...

   Final Recommendations
   - Revise the formatting to achieve a clean, professional appearance.
   - Strengthen the summary and skills sections to target the data analyst role.
   ...
```


## 🧩 Models Used

- **Language Model:** [`gpt-4o-mini`](https://platform.openai.com/docs/models/gpt-4o) (via OpenAI API)


## 📦 Dependencies

- `Python 3.x`
- `streamlit`
- `openai`
- `PyPDF2`
- `python-dotenv`

