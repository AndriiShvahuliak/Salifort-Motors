# Salifort-Motors
Building predictive models to improve employee satisfaction level at Salifort Motors company.

## Overview
The goal of this project was to analyze a dataset and build predictive models that can provide insights to the Human Resources (HR) department of a large consulting firm.
The HR department at Salifort Motors wanted to take some initiatives to improve employee satisfaction levels at the company. They collected data from employees, and they did not know what to do with it. They refer to me as a data analytics professional and ask me to provide data-driven suggestions based on my understanding of the data. They have the following question: what’s likely to make the employee leave the company?
<br>
**this story is fictional*
## Dataset
In this [dataset](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv), there are 14,999 rows, 10 columns, and these variables: 

Variable  |Description |
-----|-----| 
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)

## Modeling and Evaluation
After conducting feature engineering, the random forest model achieved AUC of 93.8%, precision of 87.0%, recall of 90.4%, f1-score of 88.7%, and accuracy of 96.2%, on the test set. 
A random forest model comprising 300 decision trees was used to determine feature importance in who would leave the company or not.
The plot below shows that in this random forest model, `last_evaluation`, `number_project`, `tenure`, and `overworked` have the highest importance, in that order. These variables are most helpful in predicting the outcome variable, `left`.
![feature importances](https://github.com/user-attachments/assets/3e5bdb7e-66ab-4e2d-8849-6a2c73143d7c)

## Conclusion
The models and the feature importances extracted from the models confirm that employees at the company are overworked. 
<br>
To retain employees, the following recommendations could be presented to the stakeholders:
<br>
* Cap the number of projects that employees can work on.
* Consider promoting employees who have been with the company for atleast four years, or conduct further investigation about why four-year tenured employees are so dissatisfied. 
* Either reward employees for working longer hours, or don't require them to do so. 
* If employees aren't familiar with the company's overtime pay policies, inform them about this. If the expectations around workload and time off aren't explicit, make them clear. 
* Hold company-wide and within-team discussions to understand and address the company work culture, across the board and in specific contexts. 
* High evaluation scores should not be reserved for employees who work 200+ hours per month. Consider a proportionate scale for rewarding employees who contribute more/put in more effort. 
