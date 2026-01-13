## Resume-Screener-API

### Project Overview

Resume-Screener-API is a backend application that automatically reads and analyzes resumes to determine a candidate’s job category.
It allows users to upload a resume file and get a prediction such as Software Engineer, Data Analyst, or Accountant.
The system is built as a REST API using FastAPI and uses a machine learning model to classify resumes based on their content.

### What This Project Does

1. Resume Upload
A user uploads a resume file (PDF) through an API endpoint.

2. Text Extraction
The system reads the uploaded file and extracts the text using a PDF parser.

3. Text Processing
The extracted text is converted into numerical features using TF-IDF vectorization.

4. ML Prediction
A pre-trained Random Forest Classifier predicts the job category (e.g., "Software Engineer", "Data Analyst") based on the resume content.

6. API Response
The predicted label is returned as a JSON response:
  ```
  {
  "prediction": "Software Engineer"
  }
  ```

### Key Features

- Upload resumes in PDF format through REST API endpoints
- Automatically extracts text from resume files
- Uses TF-IDF and machine learning models to classify job roles
- Built using FastAPI for high-performance backend services
- Uses Scikit-learn for resume analysis and prediction
- Can be run locally or using Docker for deployment
- Suitable for use in HR systems, ATS platforms, and recruitment tools

### Tech Stack

Python, Fast API, Scikit-learn, Uvicorn
