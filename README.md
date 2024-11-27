# Predicting_employee_retention
Predicting employee retention using Logistic Regression, Decision Trees, and Random Forests

## Overview
The goal of this project was to create logistic regression, decision tree, and random forest models to see which could best predict whether an employee would choose to leave the company. This project utilized data from a fictional company. The best model (random forest), with a 98.7% accuracy and a 99.4% precision, determined the features that were most important in separating employees who would leave from those who wouldn't. Based on the random forest model, the most influencial features for determining whether an employee would leave were employee satisfaction, the number of projects they were involved in, their tenure, and the amount of hours they worked.

## Business Understanding
It is expensive to find, interview and hire new employees. In addition, new employees require training that takes additional time and resources. According to b2breviews.com, the average cost of hiring a new employee in 2024 is almost $4700 taking an average of 41 days to complete, and businesses spend an average of $1200 per employee on training. Thus, it is important to understand what factors might encourage employees to leave their job so the HR department can work on those factors and improve employee retention.

## Data Understanding
The data for this fictional company comes from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). The data consists of information from apprixmately 15k employees and 10 features. The features include the following: 

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
