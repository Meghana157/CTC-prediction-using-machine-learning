# CTC Prediction Using Machine Learning

This repository contains the code and analysis for predicting an employee's Cost to Company (CTC) using machine learning models. The project explores various factors that influence CTC, such as work experience, graduation marks, job roles, and more.

---

## Introduction

This project aims to predict an employee's CTC based on historical data using various machine learning models. It provides insights into factors affecting salaries and demonstrates the application of data preprocessing, feature engineering, and model evaluation techniques.

---

## Dataset Description

The dataset includes the following features:

- **Role**: Job role of the employee (Manager = 1, Executive = 0).
- **Previous CTC**: Salary in the previous job.
- **Graduation Marks**: Academic performance in percentage.
- **Experience (Months)**: Total work experience in months.
- **College Tier**: College ranking (Tier 1, Tier 2, Tier 3).
- **City Type**: Whether the city is metro (1) or non-metro (0).
- **CTC**: Target variable representing the employee's current salary.

---

## Project Workflow

1. **Data Preprocessing**  
   - Converted categorical features (e.g., Role, College Tier, City Type) into numerical values using mapping and dummy variables.
   - Removed unnecessary columns like College and City after mapping.

2. **Exploratory Data Analysis (EDA)**  
   - Created visualizations to explore relationships and distributions:
     - Heatmaps for feature correlations.
     - Scatter plots for experience, graduation marks vs. CTC.
     - Histograms for distributions of numerical features etc...

3. **Model Building**  
   - Experimented with various machine learning models:
     - Linear Regression
     - Lasso and Ridge Regression
     - Decision Tree Regressor
     - Random Forest Regressor
     - Gradient Boosting Regressor
     - Bagging Regressor
     - XGBoost Regressor

4. **Model Evaluation**  
   - Used metrics such as:
     - **Mean Squared Error (MSE)** for average prediction error.
     - **R² Score** to measure model accuracy.

---

## Key Insights

- **Graduation Marks and Work Experience** are positively correlated with higher CTC.
- Employees from **Tier 1 Colleges** tend to have better CTC compared to Tier 2 and Tier 3 colleges.
- Metro cities have a slightly higher average CTC compared to non-metro cities.

---

## Results

The **Random Forest Regressor** emerged as the best-performing model based on R² Score and Mean Squared Error.
