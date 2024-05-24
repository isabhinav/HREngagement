# Gender and Workplace Experience
#### _Analytical Approach to Gaining Insights from Employee Engagement Data_

## Introduction
Employee engagement is a critical determinant of organizational success, influencing productivity, retention, and overall workplace satisfaction. However, engagement experiences and perceptions can significantly differ between demographic groups, especially between male and female employees.

In this project, we utilize data analysis techniques in R to uncover gender-based insights into employee engagement. By identifying differences in work experiences and perceptions between male and female employees, this analysis can guide strategic HR decisions to enhance satisfaction, foster inclusivity, and drive organizational success. Furthermore, the analysis provides a framework that can be applied to other similar datasets. 

## Problem Statement
The HR Manager is committed to ensuring that all employees feel equally engaged and valued. To achieve this, they need to understand the differences in engagement experiences between male and female employees. Help uncover these insights, to help create a more inclusive and satisfying work environment for everyone.

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

This difference in `Recommendation Score` and `Mean Score` warrants a deeper dive into the responses of both genders. To explore these differences, visual methods such as density plots, boxplots, and heatmaps were employed to compare the engagement scores and perceptions between male and female employees.

##### _Density Plots_
 - Density plots reveal disparities in the responses between genders, indicating distinct behavioral patterns across various metrics.
 - We observe clear differences in survey responses for both groups, particularly in variables such as `TrustInSeniorLeaders`, `OpportunityForGrowth`, `RecognitionForContributions`, `WorkplaceAuthenticity` and `PersonalLifeFlexibility`.
 - For example, we observe that female employees have a pronounced peak at lower scores for `RecognitionForContributions`, suggesting a need for improved recognition practices for females compared to their male counterparts.
 

![image](https://github.com/isabhinav/HREngagement1/assets/130937665/0c9f8453-2b44-4ed1-9bf7-d4c8b97e2ec2)


##### _Boxplots_
 - Boxplots highlight differences in means and showcase the spread of the two groups, emphasizing disparities in their distributions.
 - We observe that there are differences in means for variables such as `OverallSatisfaction`, `TrustInSeniorLeaders`, `RecognitionForContributions`, `SafeLearningEnvironment` and `BeliefInSurveyAction`.
 - Most variables show overlapping interquartile ranges, indicating that despite differences in means, the middle 50% of responses for each gender often fall within similar ranges.
 - Distibution of variables such as `OpportunityForGrowth` and `PersonalLifeFlexibility`, suggest that some respondents have significantly different experiences compared to the majority.
 

![image](https://github.com/isabhinav/HREngagement1/assets/130937665/577b045d-cd39-4a93-831d-aef72ff75f49)



##### _Heatmaps_
 - Heatmaps illustrate variations in the percentage of agreeable responses, highlighting the differing responses between genders.
 - We observe stark difference in responses for `PersonalLifeFlexibility`, `OverallSatisfaction`, `OpportunityForGrowth`, `ManagerAutonomy` and `InformedByLeadership`.
 - The disparities in the responses emphasize gender-specific variations, indicating different experiences between male and female employees.
 

![image](https://github.com/isabhinav/HREngagement1/assets/130937665/fdd20607-d465-4fb2-aa46-ac923443ccea)


##### _Correlation Analysis_
 - Correlation analysis identifies the most strongly correlated pairs of engagement metrics within each gender group.
 - This analysis also illustrates how different aspects of employee engagement are related within each group.
 - For males, there is strong correlation between pairs such as `SafeLearningEnvironment` and `WorkplaceAuthenticity` (0.48) and `WorkplaceAuthenticity` and `TrustInSeniorLeaders` (0.42).
 - For females, there is slight correlation between `SafeLearningEnvironment` and `WorkplaceAuthenticity` (0.25) and `SafeLearningEnvironment` and `TrustInSeniorLeaders` (0.21).
 - Both male and female employees show a positive correlation between a safe learning environment and workplace authenticity, as well as between workplace authenticity and trust in senior leaders. However, these correlations are stronger for male employees.
 - There is a gender-specific dynamic in how leadership values and learning environments interact. Male employees show a notable correlation between `SafeLearningEnvironment` and the perception that SeniorLeadersValueDifferences. This correlation does not appear in the top correlations for female employees.


![image](https://github.com/isabhinav/HREngagement1/assets/130937665/6cea9203-971a-4f6c-ae88-6b3f97a726cb)


![image](https://github.com/isabhinav/HREngagement1/assets/130937665/23f8387e-c0e7-4f75-9340-77d068b68ef8)



## Observations 
- Gender-specific variations exist in several key engagement metrics.
- Targeted interventions in recognition, work-life balance, and leadership trust are necessary to ensure equity in employee experiences and improve engagement.

 

## Recommendations  
- Improve Recognition for Contributions: Female employees report lower recognition, indicating a need for better recognition practices targeting female employees.
- Enhance Personal Life Flexibility: Both genders show low agreement in `PersonalLifeFlexibility`, with females significantly lower, suggesting the need for policies that support work-life balance.
- Foster a Safe Learning Environment: There is a notable correlation between `SafeLearningEnvironment` and other engagement metrics, especially for males. Enhancing this aspect can have a positive ripple effect.
- Increase Trust in Leadership: `TrustInSeniorLeaders` is strongly correlated with other positive engagement metrics. Initiatives to build and maintain trust can improve overall engagement.

## Conclusion
By leveraging data analysis techniques in R, we identified key areas where male and female employees have differing experiences and perceptions. These insights can guide strategic HR decisions to enhance overall employee satisfaction, address specific gender-based needs, and drive organizational success. 

