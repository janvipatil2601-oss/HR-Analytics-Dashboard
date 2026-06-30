# HR Analytics (Interactive dashboard creation using Power Bi)

## Project Objective
The main objective of this project is to analyze employee data and identify factors affecting employee attrition. The dashboard helps HR professionals understand workforce trends, improve employee retention, and make data-driven decisions.
Specific objectives include:
-  Analyze employee data such as salary, department, experience, and demographics. 
-  Identify patterns and trends in employee attrition. 
-  Compare attrition across departments, job roles, age groups, and gender. 
-  Evaluate the impact of overtime, salary, and job satisfaction on attrition. 
-  Calculate important HR KPIs such as Attrition Rate and Retention Rate. 
-  Develop an interactive dashboard for effective decision-making.

## Dataset
-<a href="https://github.com/janvipatil2601-oss/HR-Analytics-Dashboard/blob/main/HR_Analytics.xlsx">Dataset</a>

## Project Process
### Step 1: Data Collection
Collected employee HR dataset containing demographic and employment details.
### Step 2: Data Cleaning
-  Removed duplicate records.
-  Handled missing values.
-  verified data types.
-  Corrected inconsistencies in categorical values. 
### Step 3: DAX Measures Created
-  Total Employees = COUNT(Employee[EmployeeNumber])
-  Attrition Employees =CALCULATE([Total Employees],Employee[Attrition] = "Yes")
-  Active Employees =[Total Employees] - [Attrition Employees]
-  Attrition Rate % =DIVIDE([Attrition Employees],[Total Employees],0)*100
-  Retention Rate % =100 - [Attrition Rate %]
-  Average Salary =AVERAGE(Employee[MonthlyIncome])

## Dashboard Interaction
-<a href="https://github.com/janvipatil2601-oss/Data-Analysis-Dashboard/blob/main/sale%20dashboard.pbix">View Dashboard</a>

##  Dashboard
![Screeshort(495)](https://github.com/janvipatil2601-oss/HR-Analytics-Dashboard/blob/main/Screenshot%202026-06-29%20161435.png)

## Project Insight
### 1. Attrition by Department
-  Research & Development department has the highest employee attrition (133 employees).
-  Sales department also experiences significant attrition (93 employees).
-  Human Resources department has the lowest attrition (12 employees). 
### 2. Attrition by Age Group
- 	Employees aged 18–30 years leave the organization the most (100 employees). 
- 	Attrition decreases with increasing age. 
- 	Employees above 50 years are less likely to leave the company. 
### 3. Salary vs Experience Analysis
-	 Employees with more experience generally receive higher salaries. 
-	 Most attrition cases are observed among employees with lower salaries and less experience. 
### 4. Attrition by Job Role
-	 Laboratory Technicians have the highest attrition (62 employees). 
-	 Sales Executives and Research Scientists also show high turnover. 
-  Research Directors have the lowest attrition. 
### 5. Overtime vs Attrition
- 	Employees working overtime have slightly higher attrition (128 employees) compared to those not working overtime (110 employees). 
- 	Overtime may be one of the factors influencing employee turnover. 
### 6. Job Satisfaction vs Attrition
- 	Employees with lower job satisfaction levels tend to leave the organization more frequently. 
- 	Improving job satisfaction can help reduce employee attrition. 
### 7. Attrition by Gender
- 	Male employees account for the majority of attrition (63.45%). 
- 	Female employees contribute 36.55% of total attrition. 
### 8. KPI Cards Insights
- 	Total Employees: 1,480 employees are part of the organization. 
- 	Attrition Employees: 238 employees have left the company. 
- 	Active Employees: 1,242 employees are currently working. 
- 	Attrition Rate: 16.08% of employees have left. 
- 	Retention Rate: 83.92% employees are retained. 
- 	Average Salary: Employees earn an average salary of 6.5K per month.

## Final Conclusion
The HR Analytics Dashboard provides valuable insights into employee attrition and workforce trends. The analysis reveals that younger employees, employees working overtime, and employees with lower job satisfaction are more likely to leave the organization. The Research & Development department and job roles such as Laboratory Technician and Sales Executive show the highest attrition. By improving employee satisfaction, reducing excessive overtime, and implementing effective retention strategies, the organization can reduce attrition and maintain a stable and productive workforce.


