# Validation Checklist (pass/fail)

- [ ] HR rows = 1,470 and DISTINCTCOUNT(EmployeeNumber) = 1,470 (`Row Check` = 0)
- [ ] No duplicate EmployeeNumber (Remove Duplicates preview removes 0)
- [ ] Promotion table: 72 rows, no duplicate names
- [ ] Retrenchment table: no duplicate names
- [ ] Unmatched merge rows documented and signed off (expected Promotion nulls = 1,398)
- [ ] `Invalid Promotion Flags` and `Invalid Retrenchment Flags` = 0
- [ ] Attrition, OverTime Yes/No only; BusinessTravel has 3 values; satisfaction fields 1-4
- [ ] `Min Age` plausible (about 18-65); `Min Income` > 0
- [ ] `Inconsistent Role Tenure` = 0 (else investigate)
- [ ] `Inconsistent Promotion Tenure` = 0 (else investigate)
- [ ] Risk Category counts sum to total employees, no blanks
- [ ] KPI cards reconcile with an Excel PivotTable on the raw HR sheet
- [ ] Every Promotion-Retrenchment Conflict = 1 row reviewed with the business
- [ ] Drill-through to Employee Detail works, Back button visible
- [ ] Insight text worded as "associated with", never "causes"
