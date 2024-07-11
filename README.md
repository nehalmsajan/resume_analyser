# CareerCraft: ATS-Optimized Resume Analyzer Using Gemini Model - README

## Introduction
Welcome to the Resume ATS Tracker! This application leverages advanced ATS (Applicant Tracking System) technology to help users optimize their resumes for better job application outcomes. The tool provides detailed analysis, skill enhancement tips, and career progression guidance. It is built using Streamlit and integrates Google Generative AI for text analysis.

## Libraries and Dependencies
The project uses several Python libraries to function. Below is a brief description of each library and its purpose:

1. **streamlit**: Used for creating the web application interface.
2. **streamlit_extras**: Provides additional functionality for the Streamlit app, such as adding vertical space.
3. **google.generativeai**: Google Generative AI library used to generate responses based on user input.
4. **os**: Used for accessing environment variables.
5. **PyPDF2**: A library for reading and extracting text from PDF files.
6. **dotenv**: Loads environment variables from a `.env` file.
7. **json**: Standard library for working with JSON data.
8. **PIL (Python Imaging Library)**: Used for handling images within the app.

## Environment Setup
Before running the application, ensure you have a `.env` file in your project directory with the following content:
  GOOGLE_API_KEY=your_google_api_key_here


This file is necessary for configuring the Google Generative AI API.

## Main Functions

### `get_gemini_response(input)`
This function interacts with Google Generative AI to generate a response based on the provided input. It uses the 'gemini-pro' model to generate content.

### `input_pdf_text(uploaded_file)`
This function extracts text from an uploaded PDF file using the PyPDF2 library. It reads each page of the PDF and concatenates the text into a single string.

## Streamlit Interface
The Streamlit app has a user-friendly interface that guides the user through uploading their resume and entering a job description for analysis. Key UI elements include:

- **Page Configuration**: Sets the page title and layout.
- **Custom CSS Styling**: Enhances the visual appearance of the app using custom styles.
- **Main Content Sections**: Divided into several columns and sections for a clean layout.
  - **Title and Description**: Provides an introduction to CareerCraft and its features.
  - **Offerings List**: Highlights the various services provided by CareerCraft.
  - **Resume Upload and Job Description Input**: Allows users to upload their resume and paste a job description for analysis.
  - **Response Display**: Shows the analysis results, including matching percentage, missing keywords, and a profile summary.
  - **FAQ Section**: Provides answers to common questions about the service.

## Usage
To run the application, use the following command in your terminal:
  streamlit run app.py

## Conclusion
CareerCraft is a powerful tool designed to help job seekers enhance their resumes and improve their chances of landing a job. By leveraging advanced AI technology, it provides valuable insights and personalized recommendations to users. Enjoy your journey with CareerCraft and unlock new opportunities for professional success!

