# 💜 EmoShield – Student Stress Analysis and Prediction

### Student Wellbeing Dashboard Using Data Science and Machine Learning

EmoShield is a student wellbeing project that analyzes survey responses to understand factors associated with student stress. It combines data analysis, interactive visualizations, and a Machine Learning classification model to demonstrate how student-reported information can be used to predict stress levels.

## 📌 Project Overview

College students may experience stress due to academic pressure, sleep patterns, screen time, deadlines, and other lifestyle factors. EmoShield explores these factors using survey data collected through a Google Form.

The project includes an interactive wellbeing dashboard and a Random Forest classification model that predicts a student's self-reported stress level on a scale of 1 to 5.

**Note:** This is an educational prototype, not a medical diagnostic tool. Its predictions should not be treated as a clinical assessment of a student's mental health.

## 🎯 Objectives

- Analyze student wellbeing and stress survey responses.
- Explore academic, lifestyle, and wellbeing-related factors.
- Visualize stress-level distributions and related patterns.
- Prepare survey data for Machine Learning.
- Train a Random Forest classification model.
- Evaluate the model using accuracy, a classification report, and a confusion matrix.
- Demonstrate stress-level prediction using sample student responses.

## ✨ Project Features

### 1. Interactive Wellbeing Dashboard

The dashboard presents survey information through visualizations and summary statistics. It explores stress levels, sleep, screen time, study hours, academic deadlines, and other relevant factors.

### 2. Data Preprocessing

The notebook prepares the dataset by cleaning column names, converting the target stress level to numeric values, handling missing target values, and processing the age column.

### 3. Machine Learning Model

The project uses a **Random Forest Classifier** to predict self-reported stress levels from selected survey features.

Model configuration:

- Algorithm: Random Forest Classifier
- Number of trees: 200
- Random state: 42
- Class weighting: Balanced
- Categorical feature encoding: One-Hot Encoding
- Train-test split: 80% training and 20% testing

### 4. Model Evaluation

The notebook evaluates the model using:

- Accuracy score
- Precision, recall, and F1-score
- Confusion matrix
- Comparison of actual and predicted stress levels

### 5. New Student Prediction

A sample student's survey responses are passed to the trained model to demonstrate a predicted stress level and the model's estimated class probabilities.

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Plotly
- ipywidgets
- Scikit-learn
- Google Forms for survey data collection

## 📂 Project Structure

```text
EmoShield/
├── README.md
├── emoshield.ipynb
├── requirements.txt
├── .gitignore
└── data/
    └── [your permitted survey dataset CSV files]
```

The data folder is a suggested organization. Survey datasets are not included automatically and should only be shared when appropriate permission and privacy safeguards are in place.

## ⚙️ Installation and Setup

### Prerequisites

Install Python 3 and Git. A Python environment manager such as `venv` is recommended.

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_REPOSITORY_NAME
```

Replace the placeholders with your actual GitHub repository URL and repository name.

Alternatively, download the repository as a ZIP file and extract it.

### Step 2: Create a virtual environment

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Step 3: Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Step 4: Prepare the dataset

Place the required, permitted CSV survey files in the `data/` folder.

Update the dataset paths in the notebook to point to these files using relative paths. The notebook currently contains absolute paths from the original developer's computer, which must be changed before the project can run on another machine.

Ensure the CSV column names match the fields expected by the dashboard and prediction model.

### Step 5: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `emoshield.ipynb` in the browser.

### Step 6: Run the notebook

Run the cells in order, from top to bottom. Ensure the required CSV files are available before running the data-loading cells.

The notebook will process the survey data, display dashboard content, train the classifier, evaluate its predictions, and demonstrate a prediction for a sample student.

## 📊 Machine Learning Workflow

1. Load the survey dataset.
2. Explore the dataset and inspect its columns.
3. Clean column names and prepare the target variable.
4. Select academic, lifestyle, and wellbeing features.
5. Process numerical and categorical data.
6. Split the data into training and testing sets.
7. Apply One-Hot Encoding to categorical features.
8. Train the Random Forest Classifier.
9. Generate predictions on the test dataset.
10. Evaluate the model and demonstrate a new prediction.

## 📈 Results

The notebook calculates the model's accuracy and other evaluation metrics when executed against the available dataset.

Actual performance values should be reported only after running the notebook successfully. Model performance depends on the dataset size, data quality, class distribution, and the representativeness of the survey responses.

## 🚀 Future Enhancements

- Develop a dedicated web or mobile application.
- Integrate real-time wellbeing inputs where appropriate and consented to.
- Add personalized wellbeing resources and relaxation activities.
- Improve model validation using a larger and more representative dataset.
- Deploy the model through a suitable application interface.
- Add stronger privacy and data-protection controls.

## 👩‍💻 Project Information

**Project:** EmoShield – Student Stress Analysis and Prediction Using Data Science and Machine Learning

**Academic Year:** 2026–2027

**Project Contributors:** Vaishnavi Kuchekar 


*EmoShield demonstrates the application of Data Science and Machine Learning to student wellbeing research. Its purpose is educational and exploratory.*
