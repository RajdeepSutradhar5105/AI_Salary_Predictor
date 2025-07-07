# 🚀 AI_Salary_Predictor

Harness the power of machine learning to predict employee salaries with precision and style. This app estimates annual salary based on years of experience, manager rating, projects completed, teamwork skills, and leadership potential.

---

## ✨ Features

* **Interactive Input Form:** User-friendly sliders for years of experience, manager rating, projects done, teamwork, and leadership.
* **Real-time Salary Prediction:** Instant estimation of annual salary based on input parameters.
* **Dynamic Performance Score:** Calculates and displays an overall performance score with visual feedback.
* **Input Summary:** Provides a clear breakdown of the values entered for prediction.
* **Training Dataset Preview:** Shows a sample of the data used to train the machine learning model.
* **Model Performance Metric:** Displays the R² score of the trained Linear Regression model.
* **Responsive UI:** Designed with a clean, modern, and responsive user interface using Streamlit and custom CSS.

---

## 📊 Dataset

The project uses a `Salary_Data.csv` dataset, which includes the following columns:

* `YearsExperience`: Number of years of professional experience.
* `ManagerRating`: Performance evaluation from the supervisor (1-10).
* `ProjectsDone`: Total number of successful project deliveries.
* `Teamwork`: Collaboration and team integration abilities (1-10).
* `Leadership`: Ability to guide and inspire others (1-10).
* `Salary`: The annual salary (target variable).

## 🧠 Machine Learning Model

A simple Linear Regression model from `scikit-learn` is used for salary prediction. The model is trained on the provided dataset, and `StandardScaler` is used for feature scaling to ensure optimal model performance.

---

## 🛠️ Technologies Used

* **Python:** The core programming language.
* **Streamlit:** For building the interactive web application.
* **Pandas:** For data manipulation and analysis.
* **NumPy:** For numerical operations.
* **Scikit-learn:** For machine learning model implementation (Linear Regression, StandardScaler, train_test_split).

---

## 🚀 How to Run Locally

Follow these steps to set up and run the application on your local machine:

### Prerequisites

* Python 3.7+
* `pip` (Python package installer)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/RajdeepSutradhar5105/AI-Salary-Predictor.git](https://github.com/your-username/AI-Salary-Predictor.git)
    cd AI-Salary-Predictor
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: `venv\Scripts\activate`
    ```

3.  **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

    > Includes: `streamlit`, `pandas`, `numpy`, `scikit-learn`

---

## How to Run

1.  **Start the Streamlit application:**
    ```bash
    streamlit run app.py
    ```

2.  **Open in your browser:**
    The app will open automatically at `http://localhost:8501`.

---

## Usage

1.  **Adjust Parameters:** Use the sliders for "Years of Experience", "Manager Rating", "Completed Projects", "Teamwork Skills", and "Leadership Potential" to set the employee's attributes.
2.  **View Performance Score:** Observe the "Performance Score" which updates dynamically based on your input.
3.  **Predict Salary:** Click the "🚀 Predict Salary" button to get the estimated annual salary.
4.  **Review Results:** The predicted salary and an input summary will be displayed.
5.  **Explore Data:** Scroll down to see a preview of the training dataset and the model's R² score.

---

## Workflow
```mermaid
flowchart TD
    A[Start: User Opens App] --> B[Page Configuration & Styling]
    B --> C[Load Dataset (Salary_Data.csv)]
    C --> D{Validate Required Columns?}
    D -- No --> E[Display Error & Stop]
    D -- Yes --> F[Display Key Metrics]
    F --> G[Prepare ML Model]
    G --> H[Display Input Section]

    H --> H1[Years of Experience Slider]
    H --> H2[Manager Rating Slider]
    H --> H3[Projects Done Slider]
    H --> H4[Teamwork Skills Slider]
    H --> H5[Leadership Potential Slider]

    H --> I[Calculate & Display Performance Score]
    I --> J[User Clicks 'Predict Salary']

    J --> K[Show Spinner (AI Analyzing)]
    K --> L[Transform User Inputs]
    L --> M[Predict Salary with Model]
    M --> N[Display Prediction Result]
    N --> O[Display Input Summary]
    O --> P[Display Dataset Preview]
    P --> Q[Display Model Performance (R² Score)]
    Q --> R[End]
