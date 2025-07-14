# Tableau-Project

OBJECTIVE 
 
1. Analyse Overall Workforce Composition: 
To monitor the total number of employees, active employees, and their distribution 
across various age groups and departments. 
2. Measure Attrition Trends: 
To evaluate attrition count and attrition rate over time and identify departments or 
demographics with higher turnover. 
3. Understand Demographic Influence on Attrition: 
To examine how factors such as gender, age group, and education field relate to 
employee attrition. 
4. Assess Job Satisfaction Levels: 
To analyze job satisfaction ratios across different employee segments to identify areas 
needing improvement. 
5. Visualize Department-wise Attrition: 
To detect which departments, experience higher attrition and may require targeted 
engagement or retention initiatives. 
6. Support Strategic Workforce Planning: 
To provide data-driven insights that help HR professionals in developing policies for 
employee retention, training, and engagement. 
7. Enhance Decision-Making: 
To equip HR managers with a visual tool that simplifies complex employee data, 
enabling faster and more informed decision-making.


DATA ANALYSIS 
 
I. PROCEDURE 
 
 
1. Data Importing: 
• Source: The dataset was imported into Tableau from a structured data file (e.g., Excel, CSV). 
• Connection: Using Tableau’s data connection interface, the file was loaded into the 
workspace for exploration. 
• Preview: The schema and structure of the data were reviewed in Tableau’s Data Source 
tab to understand available fields (e.g., Age, Gender, Department, Attrition, Job Satisfaction, 
Education Field). 
2. Data Cleaning: 
• Missing Values Handling: 
o Checked for nulls or missing entries in key columns (e.g., Age, Attrition, Department). 
o Rows with critical missing values were either filled with default values (where 
logical) or excluded from analysis. 
• Inconsistent Formatting: 
o Standardized categorical values (e.g., “Male” vs. “male” → “Male”). 
o Date formats were checked and converted if required. 
• Data Type Verification: 
o Ensured fields had correct data types: 
▪ Age as integer 
▪ Attrition as string (Yes/No) 
▪ Job Satisfaction as ordinal numeric 
▪ Hire Date and Exit Date (if present) as date fields 
3. Data Transformation: 
• Calculated Fields Created: 
o Attrition Count: Count of records where Attrition = 'Yes' 
o Attrition Rate: 
SUM(IF [Attrition] = 'Yes' THEN 1 ELSE 0 END) / COUNT([Employee ID]) 
o Active Employees: Count of employees with Attrition = 'No' 
o Average Age: Calculated using AVG([Age]) 
o Age Group: Created a custom field to group ages 
 
• Data Grouping & Binning: 
o Binned age groups for better visualization. 
o Grouped departments and education fields as needed to simplify visuals. 
• Field Renaming: 
o Renamed technical field names to user-friendly labels (e.g., Emp_ID to 
Employee ID, Edu_Field to Education Field). 
4. Data Visualization (Dashboard Building): 
• KPIs Displayed (Using Tiles or Cards): 
o Employee Count 
o Attrition Count 
o Attrition Rate 
o Active Employees 
o Average Age 
• Charts Used: 
o Pie Chart: Department-wise Attrition Distribution 
o Bar Chart: Number of Employees by Age Group 
o Heat Map: Job Satisfaction Ratio across various employee segments 
o Bar Chart: Education Field-wise Attrition 
o Bar Chart (Segmented): Attrition Rate by Gender across Age Groups 
• Interactivity: 
o Filters added for Gender, Department, and Education Field to allow dynamic 
data exploration. 
o Tooltip customization for detailed insight

<img width="1556" height="877" alt="HR Analytics Dashboard" src="https://github.com/user-attachments/assets/51fb6532-cdc5-4174-9d33-3eca9ffd9c2f" />


