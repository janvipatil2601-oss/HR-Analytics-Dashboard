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

## Dashboard 
-<a href="https://github.com/janvipatil2601-oss/Data-Analysis-Dashboard/blob/main/sale%20dashboard.pbix">View Dashboard</a>

##  Dashboard
![Screeshort(495)](https://github.com/janvipatil2601-oss/HR-Analytics-Dashboard/blob/main/Screenshot%202026-06-29%20161435.png)

