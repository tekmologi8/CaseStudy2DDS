# Case Study 2 - Employ Attrition. A Case Study #2

Title: Employment Attrition Case Study 2

Author: Ndede, George M.  

DS6306 Fall 2021

Email: gndede@smu.edu

GitHub: https://github.com/tekmologi8/CaseStudy2DDS

YouTube: https://www.youtube.com/watch?v=9t3_HFYbYxg

## Introduction:

The modern workforce in the United States is becoming more fluid than ever before. 
As the cost of living in the country continues to increase, wages are remaining stagnant, as reported 
in the latest economic trends. Aa a result of this, we are seeing more employees shift between companies 
after just a few years and using the larger pay raise associated with switching jobs 
(as compared to staying in a single job) as a way to bolster their income to make a living.

To combat this trend and potentially get a closer feel of the status of each employee and their potential 
for attribution, we are going to conduct a data analysis to identify trends in the employee base job titles, 
overall sentiment as well as salary with hopes to be able to predict which employee is likely to leave the 
company and what salaries are associated with the employee’s current standing. 

## Purpose:

DDSAnalytics purpose in this study is planning to leverage data science for 
talent management. The executive leadership has identified predicting employee 
turnover as its first application of data science for talent management.

## Data files:

## R Markdown Files:

CaseStudy.Rmd      Main report, which includes following files


dataload.Rmd       load data

EDA_Attrition.Rmd  EDA for investigating attrition

EDA_Basic.Rmd      Very simple sanity check EDA

EDA_transform.Rmd  EDA for investigating transform

KNN.Rmd            K-nearest-neighbor implementation

Naive_Bayes.Rmd    Naive Bayes implementation

Salary.Rmd         Linear Regression to predict salary

Selection.Rmd  Using stepwise variable selection

Transform.Rmd      Transform data to improve normality

## Final Products:

Case2PredictionsNdedeAttrition.csv 		  - predicting the Attrition

Case2PredictionsNdedeSalary.csv    		  - predicting the Monthly Income

CaseStudy.html                      	  - Final full report

Ndede_George_DS6306_CaseStudy-2.pptx    - Power Point presentation (Full version)

Ndede_George_DS6306_CaseStudy-2-Presentation.pptx    - Power Point presentation (Summerised version)

## Inference 

Overtime, MonthlyIncome, TotalWorkingYears, HourlyRate, JobRole and Age are the most important factors influencing the attrition rates.
A total of 14 factors influence the attrition rate as is depicted in the decision tree. The complete list includes Age, DailyRate, 
DistanceFromHome, EnvironmentSatisfaction, HourlyRate, JobRole, JobSatisfaction, MaritalStatus, MonthlyIncome, NumCompaniesWorked, 
OverTime, RelationshipSatisfaction, StockOptionLevel and TotalWorkingYears.
CART does not improve upon the baseline accuracy by too much in case the classes are skewed. In this case, we had a skewed dependent 
Variable “Attrition” with 84% as “No”" in the test set.
Other ensemble methods like random forests can be used to improve the accuracy of the prediction.![image](https://user-images.githubusercontent.com/95389971/144554980-2d90b77b-75c1-439f-981f-fb1695d6241f.png)


## Conclusion

The model produced by stepwise selection appears to have the best R squared, and residuals appear normal
This is what is used for predictions on the blind test data.

There is clustering in the residuals that indicates that some other predictor may help, but it is not easy to point out from the dataset or from my analysis.

Some of the reasons for employee attrition.

Sales Representatives have the highest attrition rate, Directors have the lowers
Job level, total working years, years at the company have the most impact on the monthly income
Overtime, no stock options, and employees in lower level jobs are the biggest drivers of attrition.
Employees making less than $5,000 per month have the highest attrition rates
Employees under 30 are more likely to leave a job than older employees.
Employees with less than 5 years at a company or 5 total working years are more likely to leave.
KNN overrides the best prediction model, and correctly identifies employee attrition, but Naïve Bayes does a better job on this dataset.



Employee attrition can't be completely an avoidable problem in organizations. We can address the issue at the right time. By first, computing the attrition rate so we fully understand the issue and the causes behind the attrition. 

We can also then come up with a well-planned, data-driven process to reach out to new job candidates 
engage them with different strategies, and retain them for a longer time period.![image](https://user-images.githubusercontent.com/95389971/144554912-af3e6896-3f8b-4209-8944-6e0f5e4df770.png)


