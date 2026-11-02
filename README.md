# Machine Learning CIE Activity 1
## Student Performance Dataset Preparation and Exploratory Data Analysis (EDA)

---

## 👨‍🎓 Student Information

- **Name:** Sanat Ramteke
- **Roll Number:** AD3307
- **Division:** AIDS (C)
- **Activity:** Dataset Preparation and Exploratory Data Analysis
- **Subject:** Machine Learning

---

## 📌 Project Overview

This project focuses on preparing a student performance dataset for Machine Learning applications. The activity uses the Student Performance dataset from the UCI Machine Learning Repository.

The main objective is to understand the dataset, perform basic data cleaning, explore the data using statistical methods and visualizations, encode categorical variables, and standardize numerical features.

This activity focuses on data preparation and exploratory data analysis (EDA). No machine learning prediction model is trained.

## 🎯 Objectives

- Load and inspect the student performance dataset.
- Understand the structure and features of the dataset.
- Identify missing values and duplicate records.
- Perform basic data cleaning.
- Calculate summary statistics for numerical features.
- Explore categorical features using frequency counts.
- Visualize the distribution of final grades.
- Analyze the relationship between study time and final grades.
- Compare the number of students from different schools.
- Perform correlation analysis on numerical variables.
- Convert categorical features into numerical representations using one-hot encoding.
- Standardize numerical features.
- Save the prepared dataset as a CSV file.

---

## 📊 Dataset Information

**Dataset Name:** Student Performance  
**Source:** UCI Machine Learning Repository  
**Dataset Creator:** Paulo Cortez  
**Subject Area:** Social Science  
**Associated Tasks:** Classification and Regression

The dataset contains information about students' academic performance, demographic details, family background, school-related features, and study habits.

The original dataset contains two subject-specific files:

1. `student-mat.csv` — Mathematics performance.
2. `student-por.csv` — Portuguese language performance.

For this activity, the mathematics dataset is used.

### Dataset Summary

| Property | Details |
|---|---|
| Original observations | 395 |
| Original features | 33 |
| Prepared observations | 395 |
| Prepared features | 42 |
| Missing values after preparation | 0 |
| Duplicate rows remaining | 0 |

*These values are based on the notebook execution results.*

---

## 🛠️ Technologies Used

- **Python** — Programming language
- **Google Colab** — Notebook execution environment
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Feature standardization

---

## ⚙️ Activity Workflow

### Step 1: Load the Dataset

The student performance dataset is loaded into a Pandas DataFrame.

The dataset is read using a semicolon (`;`) separator.

### Step 2: Inspect the Dataset

The dataset is inspected to understand its structure.

The following operations are performed:

- Display the first five rows.
- Display the last five rows.
- Check the number of rows and columns.
- Display column names.
- Identify the data types of columns.

### Step 3: Exploratory Data Analysis (EDA)

Exploratory Data Analysis is performed to understand the dataset and identify useful patterns.

The analysis includes:

- Summary statistics of numerical features.
- Frequency counts of students from each school.
- Distribution of final grades.
- Relationship between study time and final grades.
- Comparison of student counts across schools.

### Step 4: Data Cleaning

Basic data cleaning operations are performed.

- Check for duplicate rows.
- Remove exact duplicate rows if present.
- Remove leading and trailing spaces from text columns.
- Check missing values.

The notebook reports zero duplicate rows after cleaning.

### Step 5: Statistical Analysis

Descriptive statistics are calculated for numerical columns.

The statistics include:

- Count
- Mean
- Standard deviation
- Minimum value
- Maximum value
- 25th percentile
- 50th percentile (median)
- 75th percentile

These statistics help in understanding the distribution of student data.

### Step 6: Data Visualization

The following visualizations are created using Matplotlib.

#### 1. Distribution of Final Grades (G3)

A histogram is used to show the distribution of students' final grades.

It helps identify the grade ranges in which most students fall.

#### 2. Study Time vs Final Grade

A scatter plot is used to examine the relationship between study time categories and final grades.

It helps visualize how students with different study times perform.

#### 3. Number of Students by School

A bar chart compares the number of students from the two schools represented in the dataset.

The observed dataset contains:

- GP: 349 students
- MS: 46 students

### Step 7: Correlation Analysis

Correlation analysis is performed on numerical variables.

A correlation matrix is calculated to examine relationships between numerical features.

A heatmap is used to visualize the correlation matrix.

The heatmap helps identify positive and negative correlations between variables.

### Step 8: One-Hot Encoding

Categorical variables are converted into numerical representations using one-hot encoding.

The `pandas.get_dummies()` function is used with `drop_first=True`.

This creates indicator columns containing 0 and 1 values to represent categorical information.

**Result:**
- Original cleaned dataset shape: `(395, 33)`
- Dataset shape after one-hot encoding: `(395, 42)`

### Step 9: Feature Scaling

Numerical input features are standardized using `StandardScaler` from Scikit-learn.

Standardization transforms numerical features to have approximately:

- Mean = 0
- Standard deviation = 1

The target column `G3`, representing the final grade, is excluded from scaling.

The scaled dataset is stored in `df_prepared`.

### Step 10: Save the Prepared Dataset

The prepared dataset is exported as a CSV file.

**Output filename:** `student_performance_prepared.csv`

The notebook verifies:

- Final dataset shape.
- Total number of missing values.
- Number of duplicate rows.

The prepared CSV file is then downloaded from Google Colab.

---

## 📁 Project Files

The repository contains the following project files:

| File Name | Description |
|---|---|
| `ML_Activity_1_Dataset_Preparation.ipynb` | Jupyter Notebook containing the complete activity and Python code |
| `student_performance_prepared.csv` | Prepared dataset generated after data preprocessing |
| `README.md` | Project description, objectives, methodology, and results |

*Upload the listed files to the repository to make the project complete. Include the original dataset file if needed to reproduce the notebook.*

---

## 📈 Results and Observations

After executing the activity, the following results were obtained:

1. The original mathematics dataset contained 395 rows and 33 columns.
2. No duplicate rows remained after the cleaning step.
3. The dataset contained zero missing values after preparation.
4. The final-grade histogram showed the distribution of student grades.
5. The scatter plot displayed the relationship between study time and final grades.
6. The school-count bar chart showed that GP had more students than MS in the dataset.
7. One-hot encoding increased the number of features from 33 to 42.
8. Numerical input features were standardized using `StandardScaler`.
9. The final prepared dataset contained 395 rows and 42 columns.
10. The prepared dataset was saved as `student_performance_prepared.csv`.

---

## 💡 Conclusion

In this activity, the Student Performance dataset was prepared for further Machine Learning analysis.

Basic data inspection, cleaning, statistical analysis, visualization, correlation analysis, one-hot encoding, and feature scaling were performed using Python libraries.

The final dataset was saved in CSV format and can be used for further data analysis and Machine Learning experiments.

This activity helped in understanding the importance of data preparation before developing a Machine Learning model.

---

## 🔗 Dataset Reference

**UCI Machine Learning Repository — Student Performance Dataset**

Dataset DOI: `10.24432/C5TG7T`

Official dataset page: https://archive.ics.uci.edu/dataset/320/student+performance

---

## 👨‍💻 Author

**Sanat Ramteke**  
B.Tech — Artificial Intelligence and Data Science  
Division: AIDS (C)  
Roll Number: AD3307

---

*Machine Learning CIE Activity 1 — Dataset Preparation and Exploratory Data Analysis*
