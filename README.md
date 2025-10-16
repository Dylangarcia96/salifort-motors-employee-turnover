# Salifort Motors: Employee Turnover Prediction.

## Project Overview.

Leadership tasked the data team with analysing HR survey data to identify ways to increase employee retention.  
High turnover — both voluntary resignations and terminations — is financially costly.  
Our goal:  
- Build a machine learning model to predict whether an employee will stay or leave.  
- Identify the most influential factors driving turnover.

### Dataset

**Rows:** 15,000 employees (after cleaning: 11,991)

**Columns:** Satisfaction level, performance evaluation, projects, average monthly hours, tenure, work accidents, promotions, department, salary, and turnover flag.

**Target Variable:** `left` (1 = employee left, 0 = stayed)

## Details.

A **Random Forest** model was trained and tested, achieving a **96.3% accuracy** in predicting employee departures.  
Top predictive features:  
- Satisfaction level  
- Number of projects  
- Tenure  
- Last evaluation score  
- Average monthly hours 

<img width="597" height="321" alt="image" src="https://github.com/user-attachments/assets/975573f7-08a5-4c99-87bd-d357afd58484" />

## Modeling

 | Model | Accuracy | Recall | Precision | AUC |
 |---|---|---|---|---|
 | Logistic Regression | 82% | 27% | 44% | 0.60 |
 | Decision Tree | 97.8% | 91.5% | 95.2% | 0.975 |
 | **Random Forest** | **98.3%** | **93.4%** | **96.7%** | **0.963** |
 
**Random Forest** was selected as the champion model.

## Key Insights

- 50% of employees work overtime (>200 hrs/month) → strong driver of turnover.  
- Low promotion rate (1.7%) reduces retention.  
- Low & medium salary employees are more likely to leave.  
- Extreme workloads (too many or too few projects) increase resignation risk.  
- Longer tenure reduces the likelihood of leaving.

## Recommendations

- Reduce overtime by hiring additional staff.  
- Provide promotions and recognition to high performers.  
- Balance project allocation (ideal: ~3 projects per employee).  
- Focus retention strategies on employees in their first 3 years.

## Next steps

- Experiment with **XGBoost** to compare performance.  
- Remove features with low predictive power to simplify the model.  
- Explore **K-means clustering** to segment employee groups for targeted interventions.

## [View the Full Project Notebook on GitHub](https://github.com/Dylangarcia96/salifort-motors-employee-turnover/blob/main/notebooks/Salifort%20Motors%20Project.ipynb)


