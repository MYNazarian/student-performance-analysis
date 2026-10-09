Student Performance Analysis

An exploratory data analysis and machine learning project investigating student performance and predicting final grades using Python.

Project Overview

This project explores the "Student Performance dataset" (https://archive.ics.uci.edu/dataset/320/student+performance) from the UCI Machine Learning Repository.

The goal is to understand how selected factors relate to students' final grades and build regression models to predict final performance using earlier-period grades.

Objectives

- Explore and understand the dataset.
- Investigate the relationship between study time, absences, and final grades.
- Analyze correlations between earlier-period grades and final grades.
- Build and evaluate regression models.
- Compare model performance and examine prediction errors.

Dataset

- Source: UCI Machine Learning Repository
- File: "student-mat.csv"
- Samples: 395 students
- Features: 33 columns
- Target: "G3" — final grade

The dataset contains student information, including study time, absences, previous grades, and final grades.

Tools and Libraries

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

Machine Learning

Two regression models were evaluated using "G1" and "G2" as input features:

- Linear Regression
- Random Forest Regressor

The data was split into training and test sets. Five-fold cross-validation was performed on the training data, and final evaluation metrics were calculated on the held-out test set.

Results

Model| Mean CV R²| Test MAE| Test R²
Linear Regression| 0.827| 1.262| 0.795
Random Forest| 0.793| 1.360| 0.772

Linear Regression performed better than Random Forest in these experiments, achieving a lower test MAE and a higher test R².

The results suggest that the simpler model is a useful baseline for this feature set and dataset.

Key Findings

- Earlier-period grades ("G1" and "G2") were strongly correlated with final grades ("G3").
- Study time showed only a weak positive association with final grades in this dataset.
- Absences showed almost no linear correlation with final grades in the initial analysis.
- Linear Regression outperformed Random Forest in the model comparison.

These findings describe associations in this dataset and do not establish causal relationships.

Project Structure

student-performance-analysis/
├── data/
│   └── student-mat.csv
├── notebooks/
│   └── student_analysis.ipynb
├── src/
├── README.md
├── requirements.txt
└── .gitignore

How to Run

1. Clone this repository.
2. Install the dependencies.
3. Open the notebook and run the cells.

Install dependencies:

pip install -r requirements.txt

Launch Jupyter Notebook:

jupyter notebook

Then open "notebooks/student_analysis.ipynb".

Limitations

- The analysis uses a single dataset from two Portuguese schools.
- Model performance may differ on other student populations.
- The model uses earlier-period grades, so its predictions depend on those grades being available.
- The observed relationships should not be interpreted as causal effects.

What I Learned

Through this project, I practiced data exploration, visualization, correlation analysis, regression modeling, cross-validation, model evaluation, and prediction error analysis.

This is part of my ongoing journey to learn machine learning through hands-on projects.

Author

Yasin Nazarian

GitHub: "@MYNazarian" (https://github.com/MYNazarian)