# INX Future Inc. Employee Performance Analysis

## 3. Project Summary

This study analyzes 1,200 employee records and addresses the supplied project objectives: department-wise performance, identification of the top three factors affecting performance, prediction of employee performance, and recommendations for improvement.

The main algorithm is a **Random Forest classifier**, with **Logistic Regression** as a baseline. An 80/20 stratified train/test split was used. Categorical variables were one-hot encoded, numerical variables were standardized for the Logistic Regression pipeline, and class weights were balanced. No PCA was used because the business problem requires interpretable original features.

The top three predictive factors, selected by permutation importance on the held-out test set using balanced accuracy, are:
1. Employee Environment Satisfaction
2. Employee Last Salary Hike Percentage
3. Years Since Last Promotion

The Random Forest achieved **92.08% test accuracy**, **87.09% balanced accuracy**, and **91.95% weighted F1**. Other techniques include data-quality validation, descriptive statistics, department aggregation, Spearman correlation, class-weighted learning, confusion-matrix analysis, and permutation feature importance.
