# Insights and Findings

All figures below are recalculated from the repository CSV (`data/HR_Analytics_Employee_Attrition_Dataset.csv`) with no slicers applied.

## Overall workforce

- Total employees: **2,000**
- Attrition count: **383**
- Active employees: **1,617**
- Attrition rate: **19.15%**
- Retention rate: **80.85%**

## Department comparison

| Department | Employees | Leavers | Attrition rate |
|---|---:|---:|---:|
| Finance | 161 | 34 | 21.12% |
| Human Resources | 158 | 26 | 16.46% |
| IT | 277 | 47 | 16.97% |
| Operations | 209 | 39 | 18.66% |
| Research & Development | 632 | 125 | 19.78% |
| Sales | 563 | 112 | 19.89% |

Finance has the highest department attrition rate (21.12%). Human Resources has the lowest (16.46%). This comparison is descriptive and does not explain why the rates differ.

## Tenure

| Tenure group | Attrition rate |
|---|---:|
| <1 | 30.48% |
| 1–2 | 23.07% |
| 3–5 | 15.81% |
| 6–10 | 13.88% |
| >10 | 13.89% |

Employees with less than one year of tenure have the highest observed attrition rate (30.48%).

## Overtime

| Overtime | Employees | Leavers | Attrition rate |
|---|---:|---:|---:|
| No | 1463 | 212 | 14.49% |
| Yes | 537 | 171 | 31.84% |

The overtime group has a higher observed attrition rate (31.84%) than the non-overtime group (14.49%). This is an association, not evidence that overtime caused attrition.

## Job satisfaction

| Rating | Display label | Employees | Leavers | Attrition rate |
|---:|---|---:|---:|---:|
| 1 | Very Low | 513 | 128 | 24.95% |
| 2 | Low | 515 | 93 | 18.06% |
| 3 | Medium | 503 | 102 | 20.28% |
| 4 | High | 469 | 60 | 12.79% |

The lowest satisfaction rating has an observed attrition rate of 24.95%; the highest rating has 12.79%.

## Salary

| Metric | Value |
|---|---:|
| Total monthly salary across records | ₹131,365,000 |
| Average monthly salary | ₹65,682 |
| Median monthly salary | ₹65,000 |
| Minimum monthly salary | ₹22,000 |
| Maximum monthly salary | ₹122,000 |

The sum of monthly salaries is a one-month aggregate across the sample, not annual payroll expense.

## Early-tenure leavers: metric definition

There are **259** leavers with tenure of three years or less:
- As a share of all leavers: **67.62%**.
- As a share of all employees in the dataset: **12.95%**.

The Page 4 PDF displays an Early Attrition KPI of **22.12%**. That value does not match either of the two clearly defined calculations above. Recheck the DAX measure and label before publishing or presenting that KPI.

## Interpretation

These patterns can guide questions for further analysis, such as onboarding experience, workload, role expectations, and manager support. They do not establish cause and effect. The dataset is synthetic/sample data and should not be used for real HR decisions.
