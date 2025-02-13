# Employee Churn Prediction

## Overview
This project aims to predict employee churn using machine learning models to help organizations reduce turnover rates and improve retention strategies. By analyzing employee data, we identify key factors contributing to churn and build predictive models to forecast which employees are at risk of leaving.

## Problem Statement
Employee churn is a significant challenge for organizations, leading to increased recruitment costs, loss of institutional knowledge, and reduced productivity. This project focuses on:
- Identifying factors contributing to employee churn.
- Building predictive models to forecast churn likelihood.
- Developing data-driven retention strategies.

## Dataset
The dataset used in this project contains **1,470 records** with **35 features**, including:
- **Demographics**: Age, Gender, Marital Status.
- **Job-related**: Job Role, Job Level, Job Satisfaction.
- **Compensation**: Monthly Income, Percent Salary Hike.
- **Behavioral**: Distance from Home, Overtime, Work-Life Balance.

**Source**: [Kaggle HR Dataset](https://www.kaggle.com/code/shifanaaz125/hr-dataset-eda/input)

## Methodology
### Data Preprocessing
- Handled missing values and encoded categorical variables.
- Dropped irrelevant columns (`EmployeeCount`, `StandardHours`, `Over18`).
- Normalized numerical features for model training.

### Exploratory Data Analysis (EDA)
- Analyzed correlations between features (e.g., Job Level vs. Monthly Income).
- Visualized attrition trends using histograms, boxplots, and count plots.
- Identified key insights:
  - Employees with shorter commutes had higher attrition rates.
  - Single employees showed higher attrition compared to married or divorced employees.

### Models Used
1. **Logistic Regression**:
   - Accuracy: **85.7%**
   - AUC-ROC: **0.72**
2. **Random Forest**:
   - Accuracy: **87.7%**
   - AUC-ROC: **0.76**
3. **Deep Learning (Neural Networks)**:
   - Accuracy: **87.7%**
   - AUC-ROC: **0.76**

### Model Evaluation
- Evaluated models using **Accuracy**, **Precision**, **Recall**, **F1 Score**, and **ROC-AUC**.
- Random Forest emerged as the best model due to its **balanced performance** and **high F1 score**.

## Results
- **Random Forest** achieved the highest accuracy (**87.7%**) and F1 score (**0.18**), making it the optimal choice for churn prediction.
- Key factors influencing churn:
  - **Job Satisfaction**: Lower satisfaction levels correlated with higher attrition.
  - **Distance from Home**: Employees living closer to work had higher attrition rates.
  - **Job Level**: Lower-level employees were more likely to leave.

## Impact
- **Proactive Retention Strategies**: HR teams can use the model to identify at-risk employees and implement targeted interventions.
- **Cost Reduction**: By reducing turnover, organizations can save on recruitment and training costs.
- **Improved Employee Morale**: Addressing churn factors fosters a positive work environment and enhances employee satisfaction.

## Dependencies
- **Python 3.8+**

- **Libraries:** Pandas, NumPy, Scikit-learn, TensorFlow, Matplotlib, Seaborn.

## Contributors
- **Venkata Anantha Reddy Arikatla**
