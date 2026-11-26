# Power Query Steps

1. Load sheets HR, Employees, Promotion, Retrenchment (`../powerquery/HR_Employees_Promotion_Retrenchment.m`).
2. Set data types (whole numbers for numeric HR fields, text for categorical).
3. Rename "Emplyee name" to "Employee Name" in Employees, Promotion, Retrenchment.
4. Trim, Clean and Proper-case every Employee Name (function `Clean_Name`).
5. Column Quality/Distribution check on Age, Attrition, MonthlyIncome, YearsAtCompany, OverTime, BusinessTravel, satisfaction fields.
6. Left-outer merge Employees on EmployeeNumber, then Promotion and Retrenchment on Employee Name.
7. Record unmatched counts. Name the result Employee Master; disable load on the other queries.
