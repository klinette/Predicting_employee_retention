# Predicting_employee_retention
Predicting employee retention using Logistic Regression, Decision Trees, and Random Forests

## Overview
The goal of this project was to create logistic regression, decision tree, and random forest models to see which could best predict whether an employee would choose to leave the company. This project utilized data from a fictional company. The best model (random forest), with a 98.7% accuracy and a 99.4% precision, determined the features that were most important in separating employees who would leave from those who wouldn't. Based on the random forest model, the most influencial features for determining whether an employee would leave were employee satisfaction, the number of projects they were involved in, their tenure, and the amount of hours they worked.

## Business Understanding
It is expensive to find, interview and hire new employees. In addition, new employees require training that takes additional time and resources. According to b2breviews.com, the average cost of hiring a new employee in 2024 is almost $4700 taking an average of 41 days to complete, and businesses spend an average of $1200 per employee on training. Thus, it is important to understand what factors might encourage employees to leave their job so the HR department can work on those factors and improve employee retention.

## Data Understanding
The data for this fictional company comes from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). The data consists of information from approximately 15k employees and 10 features. The features include the following: 

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

In addition, the bar chart below shows the breakdown of the percent of the employees that left versus those that stayed that exist in the data set.
![image](https://github.com/user-attachments/assets/82b4c9b7-582d-4d6e-a636-82933d494fbe)

Features were renamed and irrelevant columns were dropped after exploratory data analysis. The final features included in the models were satisfaction, last_eval, num_proj, average_monthly_hours, tenure, and salary, with the outcome variable as left.

## Modeling and Evaluation
Three models were created to predict whether employees would leave the company. The results of the three models on a validation set used to compare model performance are listed below:

model	|precision	|recall	|F1	|accuracy |
-----|-----|-----|-----|-----| 
Logistic Regression	|0.4114	|0.1841	|0.2544	|0.8181 |
Decision Tree	|0.9828	|0.9196	|0.9501	|0.9840 |
Random Forest	|0.9942	|0.9196	|0.9554	|0.9858 |


