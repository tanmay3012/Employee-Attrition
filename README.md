# HR Analytics Dashboard (Employee Attrition) using Power BI
## 📝 Project Overview
This project presents a comprehensive HR Analytics Dashboard built using Microsoft Power BI. 
The primary goal of this dashboard is to provide a clear and interactive way to analyze human resources data, with a special focus on employee attrition. 
By visualizing key HR metrics, the dashboard helps stakeholders to identify trends, understand the drivers of employee turnover,
and make data-driven decisions to improve employee retention. This project is based on the "HR Analytics Dashboard Power BI Tutorial for Beginners" from datawolfs.com.
## ✨ Key Features
Interactive and Dynamic: The dashboard is fully interactive, allowing users to filter and slice data based on various parameters.

Comprehensive KPI Tracking: Key Performance Indicators (KPIs) are prominently displayed to give an at-a-glance view of the company's HR health.

Detailed Visualizations: A variety of charts and graphs are used to represent the data, making it easy to understand and interpret complex information.

User-Friendly Interface: The design is clean and intuitive, making it accessible even for users who are not data experts.

## 📊 Key Areas of Analysis
The dashboard provides insights into the following key areas:

1. Workforce Demographics:

Analysis of the workforce by department, education field, business travel frequency, gender, job role, and age group.

2.Key HR Metrics:

Employee Count: Total number of employees in the organization.

Average Salary: The average salary across the company.

Average Monthly Salary: The average monthly income of employees.

Average Age: The average age of the workforce.

Average Salary Hike: The average percentage of salary increase.

Average Job Satisfaction Score: The average job satisfaction rating given by employees.

Gender Ratio: The ratio of male to female employees.

3.Employee Attrition Analysis:

Identification of the key factors that influence employee turnover, such as salary, age, gender, education, and work-life balance.

Analysis of attrition rates by various parameters like business travel, job satisfaction, and marital status.

## 🛠️ Technologies Used
Microsoft Power BI: The core tool used for data modeling, analysis, and visualization.

DAX (Data Analysis Expressions): A powerful formula language used to create custom calculations and aggregated measures. DAX is fundamental to this project, enabling the creation of KPIs that are not explicitly available in the raw data.

Microsoft PowerPoint: Used to design the custom background for the report, giving it a professional look and feel.

## 🧮 DAX Measures
Data Analysis Expressions (DAX) are the cornerstone of the analysis in this Power BI project. They are used to create new information from the existing data. Below are some of the key DAX measures created for this dashboard.

Total Employee Count: Calculates the total number of employees.

Code snippet

Employee Count = COUNT(HR_Employee_Attrition[EmployeeCount])
Attrition Count: Calculates the number of employees who have left the company.

Code snippet

Attrition Count = CALCULATE([Employee Count], HR_Employee_Attrition[Attrition] = "Yes")
Attrition Rate: Calculates the percentage of employees who have left the company. This measure is crucial for understanding the scale of the attrition problem.

Code snippet

Attrition Rate = DIVIDE([Attrition Count], [Employee Count])
Average Age: Calculates the average age of the employees.

Code snippet

Average Age = AVERAGE(HR_Employee_Attrition[Age])
Average Monthly Income: Calculates the average monthly salary of employees.

Code snippet

Avg Monthly Income = AVERAGE(HR_Employee_Attrition[MonthlyIncome])
Average Job Satisfaction: Calculates the average job satisfaction score, which is a key indicator of employee morale.

Code snippet

Avg Job Satisfaction = AVERAGE(HR_Employee_Attrition[JobSatisfaction])
## 📈 Dataset
The project utilizes an HR dataset provided in a CSV file. The dataset contains 1,470 records, with each record representing an employee. The dataset includes a wide range of attributes, such as:

Demographics: Age, Gender, MaritalStatus

Employment Details: Department, JobRole, JobLevel, MonthlyIncome, BusinessTravel

Educational Background: Education, EducationField

Performance and Satisfaction: PerformanceRating, JobSatisfaction, EnvironmentSatisfaction

Attrition: Attrition (the target variable)

## 🙏 Acknowledgments
This project was created by following the excellent tutorial from datawolfs.com.

A big thank you to the Power BI community for the constant support and inspiration.
