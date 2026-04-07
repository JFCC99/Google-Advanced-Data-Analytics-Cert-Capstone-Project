# Salifort Motors Employee Turnover Prediction

## Project Overview
Salifort Motors was experiencing high employee turnover that was costly 
in terms of recruiting and training. This project analyzes survey data 
from 14,999 employees to identify the key drivers of turnover and builds 
predictive models to flag at-risk employees before they leave.

## Business Problem
Can we predict whether an employee will leave the company based on their 
satisfaction level, workload, tenure, salary, and other HR data points?

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

## Approach
- Exploratory Data Analysis (EDA) to identify key turnover drivers
- Logistic Regression model (Modeling Approach A)
- Decision Tree and Random Forest models (Modeling Approach B)
- Feature engineering including overworked binary variable

## Key Findings
- Satisfaction level is the strongest predictor of turnover
- Employees working more than 175 hours per month are at higher risk
- Employees assigned 6+ projects leave at significantly higher rates
- Very few overworked employees received promotions
- Tenure years 3 and 5 are critical attrition windows

## Model Results
| Model | AUC | Precision | Recall | F1 | Accuracy |
|-------|-----|-----------|--------|----|----------|
| Logistic Regression | - | 80% | 83% | 80% | 83% |
| Decision Tree | 93.8% | 87.0% | 90.4% | 88.7% | 96.2% |
| Random Forest | 96.5% | 86.7% | 87.9% | 87.2% | 95.7% |

**Champion Model: Random Forest** with AUC of 96.5%

## Recommendations
- Cap projects per employee at 5 to reduce burnout
- Conduct satisfaction and compensation reviews at years 3 and 5
- Review promotion policies for high-performing, overworked employees
- Use the model to score current employees monthly and flag at-risk individuals

## Files
- `Salifort_Motors_JUP.ipynb` — Full Jupyter notebook with EDA and models
- `HR_comma_sep.csv` — Employee survey dataset
- `PACE_Strategy_Document` — Project planning and reflection document
- `Executive_Summary` — One page summary for stakeholders

## Certificate
Google Advanced Data Analytics Professional Certificate — Course 6 Capstone
