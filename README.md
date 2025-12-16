# HR-project-
HR Analytics Report

Employee Attrition Analysis and Predictive Modelling

1. Introduction

This report analyses employee data to understand the key drivers of attrition and to evaluate predictive models that can identify employees at risk of leaving. The dataset contains 1,470 employees with 35 HR-related variables, including demographic information, job characteristics, satisfaction metrics, and compensation data.

The objectives of this analysis are:

To explore workforce characteristics and attrition patterns

To identify key factors associated with employee turnover

To develop and evaluate machine learning models for attrition prediction

2. Dataset Overview

Total employees: 1,470

Employees who left: 237 (16.12%)

Employees who stayed: 1,233 (83.88%)

Key Variables

Demographics: Age, Gender, Marital Status

Job attributes: Job Role, Job Level, Department, Business Travel

Satisfaction indicators: Job Satisfaction, Environment Satisfaction, Work-Life Balance

Compensation: Monthly Income, Daily Rate, Hourly Rate

Experience: Total Working Years, Years at Company, Years with Current Manager

3. Data Quality and Pre-processing
3.1 Missing Data Check

Graph to include:

Missing Data Heatmap

Insight:
The heatmap shows no missing values, confirming the dataset is complete and suitable for statistical and machine learning analysis.

3.2 Distribution of Numerical Variables

Graphs to include:

Histograms of all numerical features (Age, Monthly Income, Job Level, etc.)

Insight:

Age distribution is approximately normal, centred around mid-30s

Monthly income and job level show right-skewed distributions

Attrition is clearly imbalanced, with far fewer leavers than stayers

4. Attrition Analysis
4.1 Overall Attrition Rate

Attrition rate: 16.12%

Majority of employees remain with the organisation

4.2 Age vs Attrition

Graph to include:

Count plot of Age vs Attrition

Insight:
Younger employees show higher attrition rates, particularly in early career stages.

4.3 Job Role, Marital Status, Job Level

Graphs to include:

Count plot: Job Role vs Attrition

Count plot: Marital Status vs Attrition

Count plot: Job Involvement vs Attrition

Count plot: Job Level vs Attrition

Key Findings:

Sales Representatives experience higher attrition than other roles

Single employees leave more frequently than married or divorced employees

Lower job involvement and lower job levels are associated with higher attrition

4.4 Distance from Home

Graph to include:

KDE plot comparing Distance from Home for leavers vs stayers

Insight:
Employees living further from work are more likely to leave, suggesting commute distance contributes to turnover.

4.5 Experience and Management Stability

Graphs to include:

KDE plot: Years with Current Manager

KDE plot: Total Working Years

Insight:

Employees with shorter tenure with their manager show higher attrition

Less experienced employees are more likely to leave

5. Compensation Analysis
5.1 Gender vs Monthly Income

Graph to include:

Boxplot: Monthly Income vs Gender

Insight:
Income distributions for males and females are broadly similar, though high-income outliers appear more frequently among males.

5.2 Job Role vs Monthly Income

Graph to include:

Boxplot: Monthly Income vs Job Role

Insight:
Senior leadership and specialist roles earn significantly higher incomes, while technical and entry-level roles cluster at lower salary ranges.

6. Correlation Analysis
6.1 Correlation Heatmap

Graph to include:

Correlation heatmap of numerical variables

Key Relationships Identified:

Job Level strongly correlates with Monthly Income

Total Working Years correlates with Age and Income

These relationships validate expected HR patterns and support model reliability

7. Predictive Modelling
7.1 Logistic Regression

Graphs to include:

Confusion Matrix Heatmap

Performance:

Accuracy: ~86.7%

Strong at predicting employees who stay

Lower recall for predicting leavers due to class imbalance

7.2 Random Forest Classifier

Graphs to include:

Confusion Matrix Heatmap

Performance:

Accuracy: ~84%

High precision but poor recall for attrition cases

Model tends to favour majority class

7.3 Deep Learning Model

Graphs to include:

Training Accuracy and Loss over Epochs

Performance:

Training accuracy reached 100%

Indicates overfitting, despite excellent training results

Requires regularisation or early stopping for deployment

8. Key Insights and Recommendations
Key Drivers of Attrition

Younger age and lower experience

Low job level and job involvement

Sales-related job roles

Longer commuting distances

Limited time with current manager

Recommendations

Improve engagement for early-career employees

Review workload and incentives in sales roles

Introduce flexible or hybrid working to reduce commute burden

Strengthen manager-employee relationships

Use predictive models as decision-support tools, not standalone solutions

9. Conclusion

This HR analytics project demonstrates how exploratory data analysis combined with machine learning can provide actionable insights into employee attrition. While predictive models achieved good accuracy, addressing class imbalance and overfitting is essential before operational use. Overall, the findings can support strategic HR planning, retention initiatives, and workforce optimisation.
