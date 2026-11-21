# HR Analytics: Employee Attrition

An end-to-end **Power BI HR analytics project** exploring workforce composition, employee attrition, salary patterns, and factors associated with employee exits.

The report is organized into four interactive dashboard pages: **HR Overview**, **Employee Demographics**, **Salary & Job Analysis**, and **Attrition Factors Analysis**.

![HR Overview dashboard](assets/dashboard-screenshots/page-1.png)

## Project at a glance

| Metric | Result |
|---|---:|
| Employees in dataset | 2,000 |
| Employees who left | 383 |
| Active employees | 1,617 |
| Overall attrition rate | 19.15% |
| Retention rate | 80.85% |
| Average monthly salary | ₹65,682 |
| Average tenure | 3.49 years |

> **Dataset note:** The attached dataset is a sample/synthetic employee dataset for portfolio and learning purposes. It does not represent a real employer or real employee records. Findings are descriptive and should not be interpreted as causal.

## Dashboard pages

### 1. HR Overview
Workforce KPIs, department-wise attrition rate, employee distribution by department and gender, age distribution, and attrition by tenure group.

![Page 1: HR Overview](assets/dashboard-screenshots/page-1.png)

### 2. Employee Demographics
Employee distribution by gender, age group, marital status, and department, plus gender-wise employee and attrition counts.

![Page 2: Employee Demographics](assets/dashboard-screenshots/page-2.png)

### 3. Salary & Job Analysis
Salary distribution, average salary by department, top job roles by attrition count, average salary by attrition status, and employee attrition by salary band.

![Page 3: Salary & Job Analysis](assets/dashboard-screenshots/page-3.png)

### 4. Attrition Factors Analysis
Attrition by education, tenure group, work-life balance, job satisfaction, overtime, and environment satisfaction.

![Page 4: Attrition Factors Analysis](assets/dashboard-screenshots/page-4.png)

## Key findings from the CSV

These values are recalculated directly from the CSV included in this repository, with no report slicers applied.

- **Overall attrition:** 383 of 2,000 employees left, an attrition rate of 19.15%.
- **Department:** Finance has the highest department attrition rate at 21.12%; Human Resources is lowest at 16.46%.
- **Tenure:** Employees with less than one year at the company have a 30.48% attrition rate. The rate is 23.07% for 1–2 years.
- **Overtime:** Attrition is 31.84% among employees marked for overtime versus 14.49% among those not marked for overtime.
- **Job satisfaction:** The attrition rate is 24.95% for rating 1 and 12.79% for rating 4.
- **Early exits:** 259 leavers had tenure of three years or less. That is 67.62% of leavers, or 12.95% of the full dataset.

Interpretation requires care: these are associations in this sample. They do not establish that department, tenure, overtime, or satisfaction caused an employee to leave.

## Tools and techniques

- Microsoft Power BI Desktop
- Power Query for data inspection and preparation
- DAX measures and calculated columns
- Interactive slicers and cross-filtering
- KPI cards, column charts, bar charts, donut charts, and 100% stacked bar charts
- CSV data source

## Repository structure

```text
HR-Employee-Attrition-Analytics/
├── README.md
├── .gitignore
├── assets/
│   ├── HR_Analytics_Project.pdf
│   └── dashboard-screenshots/
│       ├── page-1.png
│       ├── page-2.png
│       ├── page-3.png
│       └── page-4.png
├── data/
│   └── HR_Analytics_Employee_Attrition_Dataset.csv
├── docs/
│   ├── data-dictionary.md
│   ├── insights-and-findings.md
│   ├── methodology.md
│   └── quality-checks.md
└── powerbi/
    └── HR_Analytics_Project.pbix
```

## How to use the project

1. Download or clone this repository.
2. Open `powerbi/HR_Analytics_Project.pbix` in Power BI Desktop.
3. If Power BI asks for the source CSV location, point it to `data/HR_Analytics_Employee_Attrition_Dataset.csv` and apply the changes.
4. Use the page tabs and slicers to explore the report.
5. Refer to `assets/HR_Analytics_Project.pdf` for a static four-page report preview.

## Data and metric definitions

- **Attrition count:** Distinct employees whose `Attrition` value is `Yes`.
- **Attrition rate:** Attrition count divided by total employees in the current filter context.
- **Active employees:** Distinct employees whose `Attrition` value is `No`.
- **Retention rate:** Active employees divided by total employees in the current filter context.
- **Average salary:** Average `Monthly_Income_INR` in the current filter context.
- **Early exits (≤3 years):** Leavers whose `Years_At_Company` is less than or equal to 3.

For the full field descriptions and validation notes, see the `docs/` folder.

## Limitations

- The dataset is a sample/synthetic dataset and may contain deliberately generated patterns.
- Dashboard metrics change when slicers are applied. The figures in this README are full-dataset values.
- Correlation or group differences should not be described as causal effects.
- The current PDF contains four dashboard pages. The executive insights page is not included in that PDF.

## Author

**Hartik Manoj Bhati**  
B.Tech Computer Science & Engineering (Cyber Security)  
Portfolio project: HR Analytics – Employee Attrition

---

If you use this project as a portfolio example, be prepared to explain the business question, the data preparation, the DAX measures, the visual choices, and the limits of the findings.
