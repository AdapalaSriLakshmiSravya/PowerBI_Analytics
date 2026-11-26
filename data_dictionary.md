# Data Dictionary

## Source sheets
| Sheet | Rows | Columns |
|---|---|---|
| HR | 1,470 | 35 |
| Employees | 1,470 | EmployeeNumber, Employee Name (source typo: "Emplyee name") |
| Promotion | 72 | Employee Name, Due for promotion (Yes/No) |
| Retrenchment | 1,470 | Employee Name, Will be retrenched (Yes/No) |

## HR sheet columns
| Column | Type | Notes |
|---|---|---|
| Age | Whole | Expected about 18-65 |
| Attrition | Text | Yes/No |
| BusinessTravel | Text | Non-Travel / Travel_Rarely / Travel_Frequently |
| DailyRate, HourlyRate, MonthlyRate | Whole | Rate fields |
| Department | Text | |
| DistanceFromHome | Whole | |
| Education | Whole | Level code |
| EducationField | Text | |
| EmployeeCount | Whole | Constant 1 |
| EmployeeNumber | Whole | Unique key |
| EnvironmentSatisfaction | Whole | 1-4 |
| Gender | Text | |
| JobInvolvement | Whole | |
| JobLevel | Whole | |
| JobRole | Text | |
| JobSatisfaction | Whole | 1-4 |
| MaritalStatus | Text | |
| MonthlyIncome | Whole | Must be > 0 |
| NumCompaniesWorked | Whole | |
| Over18 | Text | |
| OverTime | Text | Yes/No |
| PercentSalaryHike | Whole | |
| PerformanceRating | Whole | |
| RelationshipSatisfaction | Whole | 1-4 |
| StandardHours | Whole | Constant |
| StockOptionLevel | Whole | |
| TotalWorkingYears | Whole | |
| TrainingTimesLastYear | Whole | |
| WorkLifeBalance | Whole | 1-4 |
| YearsAtCompany | Whole | |
| YearsInCurrentRole | Whole | Should be <= YearsAtCompany |
| YearsSinceLastPromotion | Whole | Should be <= YearsAtCompany |
| YearsWithCurrManager | Whole | |

## Calculated columns on Employee Master
| Column | Logic |
|---|---|
| Age Band | <25, 25-34, 35-44, 45-54, 55+ |
| Salary Band | <3K, 3K-5K, 5K-10K, 10K-15K, >15K |
| Tenure Band | 0-2, 3-5, 6-10, 11-15, 16+ |
| Distance Band | 0-5, 6-10, 11-20, 21+ |
| Attrition / Promotion / Retrenchment Flag | 1 if Yes else 0 |
| Employee Risk Score | +1 each: OverTime = Yes, JobSatisfaction <= 2, EnvironmentSatisfaction <= 2, WorkLifeBalance <= 2, Travel_Frequently |
| Risk Category | 0-1 Low, 2 Medium, 3-4 High, 5 Critical |
| Promotion-Retrenchment Conflict | Promotion Flag x Retrenchment Flag |
