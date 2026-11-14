# Employee Attrition Prediction Using Statistical and Machine Learning Techniques

## Project Overview

This project focuses on analyzing employee attrition and identifying the factors associated with employees leaving an organization. Statistical analysis and machine learning techniques are applied to understand employee behavior and predict attrition.

The project includes Exploratory Data Analysis (EDA), hypothesis testing, multicollinearity analysis, classification models, ROC-AUC evaluation, and feature importance analysis.

## Objectives

- Analyze employee attrition patterns.
- Identify key factors associated with employee turnover.
- Examine relationships between employee characteristics and attrition.
- Perform statistical hypothesis testing.
- Build machine learning classification models.
- Compare model performance using evaluation metrics.
- Identify important features influencing employee attrition.

## Dataset Description

The dataset contains employee information with the following characteristics:

- **Total Records:** 1,470 employees
- **Total Features:** 21
- **Numerical Variables:** 14
- **Categorical Variables:** 7
- **Missing Values:** None
- **Target Variable:** Attrition

The dataset includes employee age, department, job role, monthly income, overtime, job satisfaction, work-life balance, years at company, and other employment-related variables.

## Tools & Technologies

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn, Statsmodels
- **Environment:** Jupyter Notebook

## Project Workflow

### 1. Data Cleaning and Preprocessing
- Dataset loading and inspection.
- Missing value and duplicate checking.
- Data type inspection.
- Label encoding of categorical variables.
- Log transformation of selected numerical variables.
- Feature scaling using StandardScaler.

### 2. Exploratory Data Analysis (EDA)
- Summary statistics and data distribution.
- Attrition distribution analysis.
- Overtime vs Attrition.
- Marital Status vs Attrition.
- Department vs Attrition.
- Job Role vs Attrition.
- Age and Monthly Income analysis.
- Years at Company analysis.
- Job Satisfaction and Work-Life Balance analysis.
- Correlation heatmap.
- Outlier detection using boxplots.

### 3. Statistical Analysis

**Normality Testing**
- Shapiro-Wilk test.

**Hypothesis Testing**
- Chi-Square Test of Independence.
- Independent Two-Sample t-Test.

**Multicollinearity Analysis**
- Variance Inflation Factor (VIF).

### 4. Machine Learning Models

The dataset was divided into training and testing sets using an 80:20 split.

The following classification algorithms were implemented:

- Logistic Regression
- Random Forest Classifier
- Gaussian Naive Bayes
- Gradient Boosting Classifier
- AdaBoost Classifier

### 5. Model Evaluation

Models were compared using accuracy scores.

| Model | Accuracy |
|---|---:|
| Logistic Regression | 88.10% |
| Gradient Boosting | 87.41% |
| AdaBoost | 87.07% |
| Naive Bayes | 86.05% |
| Random Forest | 85.71% |

Logistic Regression achieved the highest accuracy of 88.10% among the implemented models.

### 6. ROC Curve and AUC Analysis

ROC curves were plotted to compare Logistic Regression and Random Forest.

| Model | AUC Score |
|---|---:|
| Logistic Regression | 0.763 |
| Random Forest | 0.778 |

Random Forest achieved a slightly higher AUC score, indicating better discrimination between the two classes in this evaluation.

### 7. Feature Importance Analysis

Feature importance was extracted using the Random Forest model.

The top influential features included:

- Monthly Income
- Log Monthly Income
- OverTime
- Age
- Distance From Home
- Total Working Years
- Years At Company
- Marital Status
- Job Satisfaction

## Key Findings

- Out of 1,470 employees, 237 (16.12%) left the organization.
- Employees working overtime had an attrition rate of approximately 30.53%, compared to 10.44% among employees not working overtime.
- Single employees showed a higher attrition rate than married and divorced employees.
- Sales Representatives had a relatively high attrition rate of 39.76%.
- Employees who left the organization generally had lower monthly incomes and fewer years at the company.
- Chi-Square tests indicated significant associations between attrition and OverTime, MaritalStatus, Department, and JobRole.
- Logistic Regression achieved the highest classification accuracy, while Random Forest achieved a slightly higher AUC score.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Keep the dataset and notebook in the same project directory.
4. Open the notebook:

`0.1-EmployeeAttrition.ipynb`

5. Run all cells to reproduce the analysis and model results.

## Repository Structure

```text
employee-attrition-prediction/
│
├── 0.1-EmployeeAttrition.ipynb
├── Employee_Attrition.csv
├── README.md
└── requirements.txt
```

## Conclusion

The analysis highlights several employee-related factors associated with attrition, including overtime, job role, department, monthly income, age, and years at company.

Multiple statistical tests and machine learning models were implemented to understand and predict employee attrition. Logistic Regression achieved the highest accuracy among the evaluated models, while Random Forest showed a slightly higher AUC score.

These findings can help organizations better understand employee turnover patterns and support data-driven employee retention strategies.

## Author

**Anuj Maurya**

M.Sc. Statistics and Computing

Banaras Hindu University (BHU)
