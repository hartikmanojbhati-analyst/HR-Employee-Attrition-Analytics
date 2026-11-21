# Project Methodology

## 1. Business objective

Explore the employee dataset to describe workforce composition, employee attrition, salary distribution, and how attrition varies across selected employee groups.

## 2. Data source

- File: `data/HR_Analytics_Employee_Attrition_Dataset.csv`
- Grain: one row per employee
- Size: 2,000 rows × 23 columns
- Outcome field: `Attrition` (`Yes`/`No`)
- Salary field: `Monthly_Income_INR` (monthly INR)

The dataset is a sample/synthetic portfolio dataset, not real company data.

## 3. Preparation

The report was developed in Power BI Desktop. The workflow includes importing the CSV, checking column types and categories, validating employee identifiers, and preparing the model for report visuals.

## 4. Analysis areas

1. HR Overview: workforce KPIs, department distribution, gender, age, and tenure.
2. Employee Demographics: employee mix by gender, age, marital status, and department.
3. Salary & Job Analysis: salary bands, average salary by department, job-role attrition counts, salary by attrition status, and salary-band comparison.
4. Attrition Factors: attrition by education, tenure, work-life balance, job satisfaction, overtime, and environment satisfaction.

## 5. Metrics

- Attrition count = distinct employees with `Attrition = "Yes"`.
- Active employees = distinct employees with `Attrition = "No"`.
- Attrition rate = attrition count / total employees.
- Retention rate = active employees / total employees.
- Average salary = average `Monthly_Income_INR`.
- Average tenure = average `Years_At_Company`.

Measures should respect the current slicer/filter context.

## 6. Visual design

The report uses a consistent navy navigation sidebar, pale page background, pastel KPI tiles, white chart panels, and a consistent set of department, job-role, gender, and attrition slicers.

## 7. Validation

Key full-dataset totals and rates were recalculated from the CSV and documented in `insights-and-findings.md`. Dashboard values may differ when slicers are applied. See `quality-checks.md` for known items to verify.
