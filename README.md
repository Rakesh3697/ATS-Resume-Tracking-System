# ATS-Friendly Resume Tracker System with NLP

## Overview

This project is an Intelligent Applicant Tracking System (ATS) that enhances resume evaluation using Natural Language Processing (NLP) and Generative AI. The system analyzes resumes against job descriptions to provide a percentage match, identify missing keywords, and highlight relevant experience.

## Features

- **Resume Parsing:** Extracts text from PDF and DOCX resume files.
- **NLP Analysis:** Uses spaCy to extract skills and experience from resumes.
- **AI-Based Evaluation:** Utilizes Google Generative AI to evaluate resumes against job descriptions and provide a match percentage.
- **User Interface:** Built with Streamlit to allow users to upload resumes and input job descriptions.

## Requirements

- Python 3.7 or later
- Dependencies:
  - `streamlit`
  - `google-generativeai`
  - `docx2txt`
  - `PyPDF2`
  - `python-dotenv`
  - `spacy`
  - `nltk`

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ats-resume-tracking-system.git
   cd ats-resume-tracking-system
Create a virtual environment and activate it:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Download the spaCy language model:

bash:
python -m spacy download en_core_web_sm
Create a .env file in the root directory of the project and add your Google API key:

env:
replace your Google_api_key
GOOGLE_API_KEY=your_google_api_key

Usage:
Run the Streamlit app:

bash:
streamlit run app.py
Open your web browser and go to http://localhost:8501.

Paste the job description in the provided text area and upload your resume (PDF or DOCX).

Click "Submit" to get the ATS evaluation results.

Code Explanation:
generate_response_from_gemini(input_text): Uses the Generative AI model to evaluate the resume against the job description and generate a response.
extract_text_from_pdf_file(uploaded_file): Extracts text from a PDF resume.
extract_text_from_docx_file(uploaded_file): Extracts text from a DOCX resume.
extract_skills_and_experience(text): Uses spaCy to identify skills and experiences from the resume text.
app.py: The main Streamlit application file that integrates the various functionalities and presents the results to the user.
Contributing
Feel free to open issues or submit pull requests if you have suggestions for improvements or fixes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
Made by Rakesh T
email:rakeshthangaraj89@gmail.com


![ATS_friendly_Resume_screenshot](https://github.com/user-attachments/assets/ca773b4a-e2c2-4e54-bf44-1e4573d540ca)
