# INX Future Inc. Employee Performance Analysis

## Project Overview

This project is an Employee Performance Analysis project for **INX Future Inc.** The objective is to analyze employee performance data, identify the major factors associated with employee performance, build a machine-learning model to predict employee performance, and provide actionable business recommendations.

The project focuses on:

- Department-wise employee performance analysis
- Identification of the top three factors associated with employee performance
- Exploratory data analysis
- Feature analysis and engineering
- Machine-learning model development
- Employee performance prediction
- Business insights and recommendations

---

## Business Problem

INX Future Inc. has observed concerns regarding employee performance and service delivery. The organization wants to use data science to understand the underlying factors associated with employee performance.

The project addresses the following business requirements:

1. Analyze employee performance department-wise.
2. Identify the top three important factors affecting employee performance.
3. Develop a machine-learning model to predict employee performance based on employee attributes.
4. Provide recommendations to improve employee performance.

---

## Dataset

The project uses the **INX Future Inc. Employee Performance dataset**.

### Dataset Information

- **Number of records:** 1,200 employees
- **Number of columns:** 28
- **Target variable:** `PerformanceRating`
- **Employee identifier:** `EmpNumber`

### Target Variable

`PerformanceRating` represents the employee performance rating.

The dataset contains the following performance ratings:

- `2`
- `3`
- `4`

The target variable is not evenly distributed, so class imbalance was considered during model training.

---

## Project Structure

```text
INX_Future_Employee_Performance_Project/
│
├── README.md
│
├── Project Summary/
│   ├── Project Summary.md
│   │
│   ├── Requirement/
│   │   └── requirements.md
│   │
│   ├── Analysis/
│   │   ├── analysis.md
│   │   ├── department_performance.csv
│   │   ├── feature_importance.csv
│   │   ├── model_results.txt
│   │   ├── spearman_correlation.csv
│   │   ├── environment_salary_interaction.csv
│   │   └── environment_promotion_interaction.csv
│   │
│   └── Summary/
│       └── summary_and_recommendations.md
│
├── data/
│   ├── raw/
│   │   ├── INX_Future_Inc_Employee_Performance_CDS_Project2_Data_V1.8.xls
│   │   └── INX_Future_Inc_Employee_Performance_CDS_Project2_Data_V1.8.xlsx
│   │
│   ├── processed/
│   │   └── employee_performance_clean.csv
│   │
│   └── external/
│       └── data_definitions.csv
│
├── src/
│   │
│   ├── Data Processing/
│   │   ├── data_processing.ipynb
│   │   └── data_exploratory_analysis.ipynb
│   │
│   ├── models/
│   │   ├── train_model.ipynb
│   │   └── predict_model.ipynb
│   │
│   └── visualization/
│       └── visualize.ipynb
│
└── references/
    ├── CDS_Project_2_INX_Future_Emp_Data_V1.6.pdf
    └── README.md
