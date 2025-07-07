# AI Salary Predictor

Harness the power of machine learning to predict salaries based on various performance metrics, experience, and other key factors. This is a Streamlit web app, designed for easy deployment and use.

## 🚀 Project Overview

This project uses a linear regression model to accurately predict salaries based on several inputs:

* Years of Experience

* Manager's Performance Rating

* Number of Projects Done

* Teamwork Skills

* Leadership Qualities

The app is interactive, fast, and visually appealing, offering a user-friendly experience.

## 📁 Project Structure

```
AI Salary Predictor/
├── app.py             # Main Streamlit application
├── requirements.txt   # Python dependencies
├── salary_data.csv    # Directory for data files (e.g., salary_data.csv)
└── README.md          # Project README file
```

## ✨ Features

* ✅ Real-time salary predictions

* ✅ Interactive input fields for customization

* ✅ Intuitive UI/UX for model input

* ✅ Easy to run and deploy with Streamlit

## 💡 Sample Input

* Years of Experience: 5

* Manager's Performance Rating: 4

* Projects Done: 10

* Teamwork: 8

* Leadership: 7

* **Predicted Salary:** `X` (based on model output)

## 🛠️ Installation & Run

### 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

### 🏃 Run App

```bash
streamlit run app.py
```

The app will open in your default browser at `http://localhost:8501`.

## 📊 Model Details

* **Model Used:** Linear Regression

* **Preprocessing:** StandardScaler

* **Accuracy Score:** ~88%

* **R² Score:** ~0.85

## 🗄️ Dataset Columns

* Years Experience

* Manager Rating

* Projects Done

* Teamwork

* Leadership

* Salary (Target)

## 🖥️ UI PreView

The application features:

* Gradient background

* Performance score cards

* Interactive input

* Live salary prediction display

## 📋 Requirements

* Python 3.x

* Streamlit

* Scikit-learn

* Pandas
