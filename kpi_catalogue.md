# KPI Catalogue

| KPI | Definition |
|---|---|
| Total Employees | Distinct EmployeeNumber in current filter |
| Attrition Employees | Employees with Attrition = Yes |
| Attrition Rate | Attrition Employees / Total Employees (ratio in the supplied population) |
| Retention Employees / Rate | Total minus attrition, and its share |
| Promotion Due / Rate | Employees flagged due for promotion, and share |
| Retrenchment Employees / Rate | Employees flagged for retrenchment, and share |
| Promotion + Retrenchment Conflict | Employees flagged in both lists (data-quality exception) |
| Average / Median Monthly Income | Mean / median MonthlyIncome |
| Average Age, Average Tenure | Mean Age, mean YearsAtCompany |
| Overtime Employees / Overtime % | OverTime = Yes, and share |
| Average Job / Environment / Relationship Satisfaction | Mean of 1-4 scores |
| Average Work-Life Balance | Mean of 1-4 score |
| High Risk Employees / High Risk % | Risk Score >= 3, and share |
| Average Performance Rating | Mean PerformanceRating |
| Average Years Since Promotion | Mean YearsSinceLastPromotion |
| Highest Attrition Department | Department with the top Attrition Rate |

Rule: every rate uses [Total Employees] (distinct population in the current filter context) as the denominator.
