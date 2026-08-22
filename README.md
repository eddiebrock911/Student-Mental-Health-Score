# 🧠 Student Mental Health Score

<p align="center">
  <strong>Machine Learning • FastAPI • HTML • CSS • JavaScript</strong>
</p>

<p align="center">
  An end-to-end Machine Learning web application that estimates a student's mental health score from social-media usage and demographic factors.
</p>

<p align="center">
  <a href="https://mentalkit.onrender.com">🚀 Live Demo</a> •
  <a href="https://github.com/eddiebrock911/Student-Mental-Health-Score">💻 Source Code</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi&logoColor=white">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white">
  <img src="https://img.shields.io/badge/HTML5-Frontend-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-Styling-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-Frontend-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/Render-Deployed-46E3B7?style=for-the-badge&logo=render&logoColor=black">
</p>

---

## 📌 Overview

**Student Mental Health Score** is a full-stack Machine Learning application designed to demonstrate how a trained ML model can be integrated into a real-world web application.

The project takes selected student demographic and digital-behaviour information as input, sends the data to a **FastAPI backend**, processes it through a pre-trained **Machine Learning pipeline**, and returns a predicted mental health score to the frontend.

The project covers the complete ML application workflow:

```text
Dataset
   ↓
Data Analysis
   ↓
Feature Engineering
   ↓
Model Training
   ↓
ML Pipeline
   ↓
Model Serialization
   ↓
FastAPI API
   ↓
HTML / CSS / JavaScript
   ↓
Prediction
```

> **Important:** This project is an educational Machine Learning application. Its output should not be considered a medical diagnosis, psychological assessment, or professional mental-health advice.

---

## 🚀 Live Application

### 🌐 Try the Project

**Live Demo:**
https://mentalkit.onrender.com

The application provides a clean web interface where users can enter the required information and receive a model-generated prediction.

---

## ✨ Features

* 🧠 Machine Learning-based prediction
* ⚡ FastAPI REST API backend
* 🎨 Responsive HTML/CSS frontend
* 🖥️ Interactive JavaScript interface
* 🔄 Real-time API communication
* 🤖 Pre-trained Scikit-learn pipeline
* 📊 Data analysis using Jupyter Notebook
* 🌍 Country-based input handling
* 📱 Responsive UI
* ☁️ Render deployment
* 🔐 Input validation through FastAPI/Pydantic
* 🧩 Modular project structure

---

## 🧠 Machine Learning

The project uses a trained Machine Learning pipeline to generate the prediction.

### Model Pipeline

```text
Raw User Input
      ↓
Feature Selection
      ↓
Preprocessing
      ↓
Categorical Encoding
      ↓
Feature Transformation
      ↓
Random Forest Model
      ↓
Predicted Mental Health Score
```

The trained pipeline is stored as:

```text
mental_health_rf_pipeline.pkl
```

Using a serialized pipeline allows preprocessing and prediction logic to remain consistent between training and production.

---

## 📥 Input Features

The application collects information such as:

| Feature            | Description                                |
| ------------------ | ------------------------------------------ |
| Age                | Student's age                              |
| Gender             | Gender category                            |
| Country            | Student's country                          |
| Academic Level     | Current academic level                     |
| Most Used Platform | Social-media platform used most frequently |
| Purpose of Use     | Primary reason for using social media      |

These features are passed from the frontend to the FastAPI backend for prediction.

---

## 🏗️ Project Architecture

```text
┌─────────────────────────────┐
│        User / Browser       │
└──────────────┬──────────────┘
               │
               │ HTTP Request
               ▼
┌─────────────────────────────┐
│     HTML / CSS / JavaScript │
│          Frontend            │
└──────────────┬──────────────┘
               │
               │ JSON
               ▼
┌─────────────────────────────┐
│          FastAPI            │
│          Backend             │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│   Pydantic Input Validation │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│  mental_health_rf_pipeline  │
│        .pkl Model            │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│     Prediction / Score      │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│      Frontend Result        │
└─────────────────────────────┘
```

---

## 📂 Repository Structure

```text
Student-Mental-Health-Score/
│
├── Mental_Health_Impact.ipynb
│
├── Student Social Media And Mental Health Impact.csv
│
├── mental_health_rf_pipeline.pkl
│
├── main.py
│
├── index.html
│
├── style.css
│
├── script.js
│
├── requirements.txt
│
├── render.yaml
│
└── README.md
```

### 📄 File Description

| File                                                | Purpose                                        |
| --------------------------------------------------- | ---------------------------------------------- |
| `Mental_Health_Impact.ipynb`                        | Data analysis, experimentation and ML workflow |
| `Student Social Media And Mental Health Impact.csv` | Dataset                                        |
| `mental_health_rf_pipeline.pkl`                     | Trained ML pipeline                            |
| `main.py`                                           | FastAPI backend                                |
| `index.html`                                        | Application UI                                 |
| `style.css`                                         | Frontend styling                               |
| `script.js`                                         | Frontend logic and API communication           |
| `requirements.txt`                                  | Python dependencies                            |
| `render.yaml`                                       | Render deployment configuration                |
| `README.md`                                         | Project documentation                          |

---

## ⚙️ Tech Stack

### Machine Learning

* Python
* Pandas
* NumPy
* Scikit-learn
* Random Forest
* Joblib

### Backend

* FastAPI
* Pydantic
* Uvicorn

### Frontend

* HTML5
* CSS3
* JavaScript

### Deployment

* Render

### Development

* Jupyter Notebook
* Git
* GitHub

---

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/eddiebrock911/Student-Mental-Health-Score.git
```

### 2. Enter the project directory

```bash
cd Student-Mental-Health-Score
```

### 3. Create a virtual environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
```

```bash
source venv/bin/activate
```

---

## 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run Locally

Start the FastAPI development server:

```bash
uvicorn main:app --reload
```

The application will normally be available at:

```text
http://127.0.0.1:8000
```

FastAPI automatically provides interactive API documentation at:

```text
http://127.0.0.1:8000/docs
```

---

## 🔌 API Workflow

The frontend communicates with the FastAPI backend using HTTP requests.

### Request Flow

```text
Frontend Form
     ↓
JavaScript
     ↓
POST Request
     ↓
FastAPI
     ↓
Pydantic Validation
     ↓
ML Pipeline
     ↓
Prediction
     ↓
JSON Response
     ↓
Frontend UI
```

This architecture keeps the Machine Learning model separated from the presentation layer.

---

## 📊 Machine Learning Workflow

The notebook follows a typical ML development lifecycle:

```text
1. Load Dataset
       ↓
2. Explore Data
       ↓
3. Clean Data
       ↓
4. Select Features
       ↓
5. Preprocess Data
       ↓
6. Train Model
       ↓
7. Evaluate Model
       ↓
8. Build Pipeline
       ↓
9. Serialize Model
       ↓
10. Integrate with FastAPI
```

---

## ☁️ Deployment

The project is configured for deployment using **Render**.

The repository includes:

```text
render.yaml
```

The deployment architecture is:

```text
GitHub Repository
       ↓
Render Build
       ↓
Python Environment
       ↓
FastAPI Server
       ↓
Public Web Application
```

### Live Deployment

🚀 https://mentalkit.onrender.com

---

## 🔒 Input Validation

FastAPI/Pydantic is used to validate incoming user data before it reaches the Machine Learning pipeline.

This helps prevent invalid input from being directly passed into the model.

Example validation concepts include:

```text
Age Range
Gender Categories
Academic Level
Supported Platforms
Purpose Categories
Country Input
```

---

## 🧪 API Documentation

When running locally, FastAPI provides automatic interactive documentation.

### Swagger UI

```text
http://127.0.0.1:8000/docs
```

### ReDoc

```text
http://127.0.0.1:8000/redoc
```

These interfaces make it easy to inspect and test the API endpoints.

---

## 🎯 Project Goals

This project was built to demonstrate practical skills in:

* Machine Learning
* Data preprocessing
* Feature engineering
* Model deployment
* REST API development
* Frontend/backend integration
* Model serialization
* Cloud deployment
* Full-stack ML application development

Rather than keeping the ML model inside a notebook, this project turns it into an accessible web application.

---

## 🔮 Future Improvements

Potential improvements include:

* [ ] Add model performance metrics to the application
* [ ] Add prediction history
* [ ] Add user dashboards
* [ ] Add data visualization
* [ ] Add model explainability
* [ ] Add feature importance visualization
* [ ] Add automated ML retraining pipeline
* [ ] Add database integration
* [ ] Add authentication
* [ ] Add automated testing
* [ ] Add CI/CD with GitHub Actions
* [ ] Improve API documentation
* [ ] Add monitoring and logging
* [ ] Add accessibility improvements

---

## ⚠️ Disclaimer

This application is created for **educational and research purposes**.

The generated score is a Machine Learning prediction based on the provided dataset and model. It is **not a medical diagnosis**, psychological evaluation, or substitute for professional healthcare.

For real mental-health concerns, users should seek support from a qualified mental-health professional or trusted adult.

---

## 👨‍💻 Author

### Ankit

**AI / Machine Learning Developer**

* GitHub: https://github.com/eddiebrock911
* Project Repository: https://github.com/eddiebrock911/Student-Mental-Health-Score
* Live Project: https://mentalkit.onrender.com

---

## ⭐ Support

If you find this project useful:

⭐ Star the repository
🍴 Fork the project
🐛 Report issues
💡 Suggest improvements

---

## 📜 License

This project is intended for educational purposes.

If you plan to reuse, modify, or redistribute the project, please review the repository contents and dataset licensing requirements before doing so.

---

<p align="center">
  <strong>Built with Python, Machine Learning & FastAPI.</strong>
</p>

<p align="center">
  Made by <strong>Ankit</strong> 🚀
</p>

