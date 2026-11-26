# Report Pages and Visuals

## Page 1: HR Executive Dashboard
| Visual | Type | Fields |
|---|---|---|
| 9 KPI cards | Card | Total Employees, Attrition Employees, Attrition Rate, Retention Rate, Promotion Due, Retrenchment Employees, Promotion + Retrenchment Conflict, Average Monthly Income, Overtime % |
| Headcount by Department | Bar | Department; Total Employees |
| Attrition by Department | Bar | Department; Attrition Rate |
| Attrition by Overtime | Clustered bar | OverTime; Attrition Rate |
| Attrition by Age Band | Bar | Age Band (sorted by Age Band Sort); Attrition Rate |
| Promotion vs Retrenchment | Clustered column | Department; Promotion Due, Retrenchment Employees |
| Key alert | Card | Highest Attrition Department |

## Page 2: Attrition Analysis
Headline card: Attrition Rate. Bar charts (Value = Attrition Rate) by: Department, Job Role, Age Band, Job Level, OverTime, Business Travel, Tenure Band. Slicers: Gender, Marital Status. Optional Decomposition Tree (Analyze: Attrition Rate; Explain by: Department, Job Role, OverTime, Age Band, Business Travel, satisfaction fields).

## Page 3: Employee Engagement
| Visual | Type | Fields |
|---|---|---|
| 4 satisfaction cards | Card / gauge | Average Job / Environment / Relationship Satisfaction, Average Work-Life Balance |
| Satisfaction vs Attrition (x4) | Clustered bar | Satisfaction field (1-4); Attrition Rate (or field parameter) |
| Overtime vs Satisfaction | Matrix | Rows: OverTime; Columns: satisfaction field; Values: average score / Attrition Rate |

## Page 4: Workforce & Compensation
Headcount by Job Level and Job Role (bars); cards for Average and Median Monthly Income; Average Monthly Income by Salary Band (sorted by Salary Band Sort); Income vs Attrition (Axis: Attrition; Value: Average Monthly Income); Tenure distribution (Axis: Tenure Band; Value: Total Employees).

## Page 5: Promotion & Retrenchment
Cards: Promotion Due, Retrenchment Employees, Promotion + Retrenchment Conflict (red/orange background). Stacked columns by Department, Job Role, Job Level with Promotion Due and Retrenchment Employees. Matrix: Employee Name (filtered to either flag = 1) with Average Performance Rating and Average Tenure.

## Page 6: HR Risk & Employee Detail
| Visual | Type | Fields |
|---|---|---|
| Risk distribution | Donut / bar | Risk Category; Total Employees |
| High-risk segments | Matrix heatmap | Rows: Department; Columns: Job Role; Values: High Risk %; colour scale |
| Risk matrix | Scatter / matrix | OverTime x satisfaction band, colour = Average Risk Score |
| Detail table | Table | Employee Name, Department, Job Role, Risk Category, Promotion Flag, Retrenchment Flag |

## Cross-page visuals
- Matrix: Department > Job Role with Total Employees, Attrition Rate, Average Monthly Income, Average Risk Score
- Scatter: X Average Monthly Income, Y Average Tenure, Details Employee Name / Job Role, Legend Attrition
- Heatmap: Department x Job Role by Attrition Rate (matrix + conditional formatting)

## Slicers (sync Department, Job Role, Job Level across all pages)
Department, Job Role, Job Level, Gender, Age Band, Marital Status, Business Travel, OverTime, Education Field, Performance Rating, Job/Environment/Relationship Satisfaction, Work-Life Balance, Promotion Status, Retrenchment Status, Risk Category.

## Employee Detail (drill-through)
Drill-through field: EmployeeNumber (optionally Employee Name, Department, Job Role). Header cards: Employee Name, EmployeeNumber, Department, Job Role. Detail: Age, Gender, Job Level, Monthly Income, OverTime, Business Travel, the 3 satisfaction scores, Work-Life Balance, Performance Rating, Total Working Years, Years at Company, Years in Current Role, Years Since Last Promotion, Attrition, Promotion Flag, Retrenchment Flag, Risk Score, Risk Category. Keep the Back button visible.
