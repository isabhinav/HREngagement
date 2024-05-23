# Gender and Workplace Experience
#### _Analytical Approach to Gaining Insights from Employee Engagement Data_

## Introduction
Employee engagement is a critical determinant of organizational success, influencing productivity, retention, and overall workplace satisfaction. However, engagement experiences and perceptions can significantly differ between demographic groups, especially between male and female employees.

In this project, we utilize exploratory data analysis techniques in R to uncover gender-based insights into employee engagement. By identifying differences in work experiences and perceptions between male and female employees, this analysis can guide strategic HR decisions to enhance satisfaction, foster inclusivity, and drive organizational success through targeted interventions and resource allocation.

## Problem Statement
The HR Manager is committed to ensuring that all employees feel equally engaged and valued. To achieve this, they need to understand the differences in engagement experiences between male and female employees. Help them uncover these insights, so we can create a more inclusive and satisfying work environment for everyone.

## Data Description
- Mock employee engagement survey dataset developed by Aaron Rodriguez.
- The dataset includes 1,000 rows and 28 columns, representing the responses of all employees within the organization at the individual level.
- Captures employees' perceptions and attitudes -  quantifying scores for metrics such as recommendation, engagement, satisfaction, leadership perception, and others.
- Features a mix of numeric and categorical data types.
- No missing values were reported in the dataset, indicating completeness and reliability for analysis.
- Demographic variables include gender, race, department, and job level

## Exploratory Data Analysis
Focused on the summary table, visual techniques such as density plots, boxplots, heatmaps, and correlation analysis. Below are a few observations from the analysis.

##### _Summary Table_

| Gender | Count | Mean Recommendation Score | Median Recommendation Score | SD Recommendation Score | Percentage Agreeable | Overall Mean Score |
|--------|-------|---------------------------|-----------------------------|-------------------------|----------------------|---------------------|
| Female | 490   | 6.04                      | 6                           | 1.88                    | 90.41                | 3.70                |
| Male   | 510   | 6.45                      | 7                           | 2.10                    | 91.18                | 3.90                |


- Males have a slightly higher mean `recommendation score` (6.45) compared to females (6.04).

- Summary table used to provide an overview of key engagement metrics by gender, enabling easy comparison and identification of disparities between male and female employees.
- Survey includes responses from 490 female employees and 510 male employees, providing a balanced perspective across genders.
- Male employees have a slightly higher mean recommendation score (6.45) compared to female employees (6.04), indicating a marginally higher likelihood of recommending the organization as a place to work.
- Both genders exhibit high percentages of agreeable responses, with males at 91.18% and females at 90.41%, reflecting overall satisfaction. However, the overall mean score for males (3.90) is higher than for females (3.70), suggesting a difference in overall engagement and satisfaction levels.





