# HR-dashboard
### Project Overview
An interactive HR Analytics Dashboard built in Power BI to help the HR team to gain actionable insights into workforce dynamics, promotion eligibility, job satisfaction, and strategic workforce planning.
### Data Source
The dataset was obtained from a publicly available YouTube tutorial on HR dashboard creation in Power BI. The data was used strictly for learning and demonstration purposes. It was cleaned and enhanced using Power Query, with additional columns created to support HR metrics such as promotion eligibility, retention, and satisfaction analysis.
### Tools
- Power Query Editor for data cleaning and transformation.
- DAX for calculations and metrics.
- Power BI Desktop-Data Visualization.

### Data Preparation
In the initial data preparation phase,we performed the following tasks:
- Data loading and inspection.
- Handling Missing values.
- Adding calculated columns.
### Exploratory Data Analysis
EDA involved exploring the HR data to answer key questions, such as:
- What is the overall profile of the workforce in terms of total number, gender distribution, job roles, job levels, and years of service?
- How is promotion eligibility distributed across job roles, job levels, and years of service?
- What are the patterns in job satisfaction, and how does satisfaction relate to job level, promotion eligibility, or retention?
- How does distance from work affect employees, and are there any links between commuting distance, satisfaction, or retrenchment?
- What does the retention vs. retrenchment data reveal, and are there job roles or conditions more associated with employee exit?
### Data analysis
``` Power Query
Due for promotion = IF(ISBLANK( CALCULATE([Total Employees],'HR Analytics Data'[Promotion Status]="Due for Promotion")),0,CALCULATE([Total Employees],'HR Analytics Data'[Promotion Status]="Due for Promotion"))
```
### Results
The analysis results are summarised as follows:
- The dataset covers 1,470 employees, with a 60% male and 40% female distribution.
-  Most employees hold mid-level roles, have worked for 2–6 years, and show medium to high job satisfaction levels.
-  Only 5% are currently due for promotion, concentrated in a few job roles.
-  A large portion (64%) of employees live very close to work, while a smaller group commutes from farther distances.
-  92% of the workforce is actively retained, while 8% are flagged for retrenchment, which is primarily associated with employees who have had longer tenures in the company.
### Recomendations
- Review promotion criteria to include more eligible mid-level staff.
- Support long-serving employees with leadership roles or flexible options to reduce retrenchment.
- Enhance job satisfaction through growth, recognition, and regular feedback.
- Assist distant commuters with remote work or transport support.
- Use targeted retention plans based on performance and engagement, not just tenure.
 ### Limitations
Assumptions were made when defining promotion and retrenchment logic in the absence of official HR rules.
