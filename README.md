**Project Overiew**:

**Dashboard:**
![dashboard](https://github.com/swarna987456/Garment_Employees_DataAnalysis_Excel/assets/111689182/d58c95fe-f98d-4a4b-857f-6d6359ff2c9e)

**1. Data Collection:**

Dataset link: [Dataset](https://archive.ics.uci.edu/dataset/597/productivity+prediction+of+garment+employees)

**About the dataset:** This dataset includes important attributes of the garment manufacturing process and the productivity of the employees which had been collected manually and also been validated by the industry experts.

**2. Data Cleaning:** 

**Observations:** 
date	department	day	month	team_no	targeted_productivity	actual_productivity
01-01-2015	finishing 	Thursday	January	1	75.00%	88.65%
01-01-2015	sweing	Thursday	January	1	75.00%	75.04%

1.	Each row represent A unique team productivity score in one day for particular department(team_id)
2.	Team members count in each group is not clear and constant, there is some variabilty. As the scores are focusing more on the teams not individual we will also do analysis based on teams scores
   
**Data Cleaning Steps:**
1.	Corrected the Date column datatype.
2.	Ensured four quarters per month as specified.
3.	Added Month column and Productivity boolean value.
4.	Converted no_of_workers to integer.
5.	Filled null WIP values with 0 (indicating no work).
6.	Changed targeted and actual productivity to percentages.

**3. Data Analysis:**
**Objective:**
1.	Performance Comparison Targeted Vs Actual
2.	Productivity Time series Analysis

**Exploratory Data Analysis (EDA)** 

**1.	Performance Comparison:**
  1.	Utilized basic statistics, histograms, box plots, and a paired T-test.
  2.	73% of the time, teams met their targets; 23% failed.
  3.	Conducted a paired T Test on actual and target mean performance scores, concluded that there is no significant difference between two at 95% confidence level
  4.	Average targeted productivity: 72.96% (low variability, SD = 9.7%)
  5.	Average actual productivity: 73.5% (high variability, SD = 17.4%)
**2. Productivity by Quarter and Day:**
  1.	Highest productivity in Q1, lowest in Q3 (limited data for Q3).
  2.	Significant difference in productivity scores across months (ANOVA test).
  3.	Higher productivity on Saturdays, Mondays, and Tuesdays.

  **3. Examine the relationship between idle time, idle men, and overtime.**
        
**4. Data Visualization:**

**Dashboard Development:**
Stakeholders requested a dashboard to monitor team performance:
1.	Compare actual vs. targeted average productivity for each team.
2.	Analyze overtime by each team to identify issues and optimize processes.
3.	Examine the relationship between idle time, idle men, and overtime.
4.	Include slicers for Month, Quarter, and Day to filter performance data accordingly.

**5. Conclusion & Recommendations:**
This comprehensive analysis and visualization aim to enhance productivity tracking and decision-making in garment manufacturing.
1.	As there is no significant difference between actual and targeted mean performance scores, management and the workforce should continue to follow the current processes.
2.	Since there is lower productivity on Wednesday and Thursday, management should discuss with the workforce to understand the challenges they are facing and take necessary steps.
3.	As we identify the idle time and manpower in each team, management should investigate the reasons for overtime and take the necessary steps.
