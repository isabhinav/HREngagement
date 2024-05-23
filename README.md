# Gender and Workplace Experience
#### _Analytical Approach to Gaining Insights from Employee Engagement Data_

## Introduction
Employee engagement is a critical determinant of organizational success, influencing productivity, retention, and overall workplace satisfaction. However, engagement experiences and perceptions can significantly differ between demographic groups, especially between male and female employees.

In this project, we utilize data analysis techniques in R to uncover gender-based insights into employee engagement. By identifying differences in work experiences and perceptions between male and female employees, this analysis can guide strategic HR decisions to enhance satisfaction, foster inclusivity, and drive organizational success through targeted interventions and resource allocation.

## Problem Statement
The HR Manager is committed to ensuring that all employees feel equally engaged and valued. To achieve this, they need to understand the differences in engagement experiences between male and female employees. Help them uncover these insights, so we can create a more inclusive and satisfying work environment for everyone.

## Data Description
- Mock employee engagement survey dataset developed by Aaron Rodriguez.
- The dataset includes 1,000 rows and 28 columns, representing the responses of all employees within the organization at the individual level.
- Captures employees' perceptions and attitudes -  quantifying scores for metrics such as recommendation, engagement, satisfaction, leadership perception, and others.
- Features a mix of numeric and categorical data types.
- No missing values were reported in the dataset, indicating completeness and reliability for analysis.
- Demographic variables include gender, race, department, and job level

## Key Metrics
- Mean Score: The average score given by employees across all survey questions. Provides general sense of employee sentiment and perception regarding different aspects of their work environment.
- Recommendation Score: Comes directly from the question "On a scale of 0 to 10, how likely is it that you would recommend DataSkillUp as a place to work?" Serves as a key indicator of employee satisfaction and engagement.
- Percentage Agreeable: The percentage of responses that are 4 or higher on a 5-point scale. Helps in identifying the proportion of employees who have a positive perception of specific aspects of their work environment.

## Data Preparation
- Ensured there were no missing values in the dataset. 
- All survey question columns were renamed to concise and meaningful names for ease of analysis.
- Transformed the dataset into a long format for specific analyses and visualizations, such as percentage calculations and heatmaps.
- Split the data into its numerical subsets for applying correlation analysis.

## Data Analysis
Focused on the summary table, visual techniques such as density plots, boxplots, heatmaps, and correlation analysis. Below are a few observations from the analysis.

##### _Summary Table_

| Gender | Count | Mean Recommendation Score | Median Recommendation Score | SD Recommendation Score | Percentage Agreeable |  Mean Score         |
|--------|-------|---------------------------|-----------------------------|-------------------------|----------------------|---------------------|
| Female | 490   | 6.04                      | 6                           | 1.88                    | 90.41                | 3.70                |
| Male   | 510   | 6.45                      | 7                           | 2.10                    | 91.18                | 3.90                |

- Summary table used to provide an overview of key engagement metrics by gender.
- Survey includes responses from 490 female employees and 510 male employees, providing a balanced perspective across genders.
- Male employees have a slightly higher mean `Recommendation Score` (6.45) compared to female employees (6.04), indicating a marginally higher likelihood of recommending the organization as a place to work.
- Both genders exhibit high percentages of agreeable responses, with males at 91.18% and females at 90.41%, reflecting overall satisfaction.
- However, the `Mean Score` for males (3.90) is higher than for females (3.70), suggesting a difference in overall engagement and satisfaction levels.
- This difference in `Mean Score` warrants a deeper dive into the responses of both genders. 

This difference in `Recommendation Score` and `Mean Score` warrants a deeper dive into the responses of both genders. To explore these differences, visual methods such as boxplots, density plots, and heatmaps were employed to compare the engagement scores and perceptions between male and female employees.

##### _Boxplots_
 - Boxplots facilitated the detection of distribution disparities and outliers.
 - Notable outliers in `salary` boxplot suggest that a small number of employees have salaries significantly above the rest.
 - The `bonus` boxplot shows a similar pattern to salary, with most bonuses clustering at the lower end and some outliers indicating exceptionally high bonuses.
 - The `age` boxplot presents a relatively symmetrical distribution, indicating a balanced age range across the workforce. 
 






