# Student Performance Analysis

A Python data analysis project exploring student performance, study time, absences, and grades using the Student Performance dataset.

## Project Overview

The goal of this project is to practice Exploratory Data Analysis (EDA) and investigate patterns in student academic performance.

## Dataset

* **Source:** [UCI Student Performance Dataset](https://archive.ics.uci.edu/dataset/320/student+performance)
* **Students analyzed:** 395
* **Features:** 33
* **File:** `data/student-mat.csv`

The dataset contains information about students' backgrounds, study habits, absences, and academic grades.

## Tools & Technologies

* Python
* Pandas
* Matplotlib
* Jupyter Notebook

## Analysis

This project explores:

* The relationship between weekly study time and final grades.
* The relationship between student absences and final grades.
* Correlations between first-period (G1), second-period (G2), and final grades (G3).
* Visual patterns in student performance.

## Key Findings

* Study time showed a very weak positive association with final grades.
* No statistically significant monotonic association was observed between absences and final grades.
* Previous-period grades were strongly correlated with final grades, especially G2.

These findings describe associations in this dataset and do not establish causation.

## Project Structure

```text
student-performance-analysis/
├── data/
│   └── student-mat.csv
├── notebooks/
│   └── student_analysis.ipynb
├── src/
├── README.md
├── requirements.txt
└── .gitignore
```

## How to Run

1. Clone this repository.

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Open `notebooks/student_analysis.ipynb` in Jupyter Notebook.

4. Run the cells to reproduce the analysis.

## Current Status

Exploratory Data Analysis completed. Further analysis and machine learning experiments are planned.

## Author

**Yasin Nazarian**

Learning Machine Learning through hands-on projects and sharing the process along the way.
