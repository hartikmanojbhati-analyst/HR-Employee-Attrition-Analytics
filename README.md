<div align="center">

# 📊 HR Analytics | Employee Attrition

### An interactive Power BI project exploring workforce composition, employee exits, salary patterns, and factors associated with attrition.

<p>
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=111111" alt="Power BI">
  <img src="https://img.shields.io/badge/Excel-Data%20Analysis-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/CSV-Dataset-4B8BBE?style=for-the-badge&logo=files&logoColor=white" alt="CSV">
  <img src="https://img.shields.io/badge/DAX-Measures-7B61A8?style=for-the-badge" alt="DAX">
</p>

**📌 Portfolio Project** &nbsp; | &nbsp; **📍 HR Analytics** &nbsp; | &nbsp; **📈 4 Interactive Report Pages**

</div>

---

## 👀 Project Preview

> Explore the four-page Power BI report covering HR overview, employee demographics, salary and job analysis, and attrition factors.

| 01 · HR Overview | 02 · Employee Demographics |
|:---:|:---:|
| ![HR Overview](assets/dashboard-screenshots/page-1.png) | ![Employee Demographics](assets/dashboard-screenshots/page-2.png) |
| 03 · Salary & Job Analysis | 04 · Attrition Factors |
| ![Salary and Job Analysis](assets/dashboard-screenshots/page-3.png) | ![Attrition Factors](assets/dashboard-screenshots/page-4.png) |

📄 **[View the complete 4-page dashboard PDF](assets/HR_Analytics_Project.pdf)**  
💻 **[Open the Power BI file](powerbi/HR_Analytics_Project.pbix)**  
🗂️ **[Explore the dataset](data/HR_Analytics_Employee_Attrition_Dataset.csv)**

---

## 🎯 Business Problem

Employee attrition can affect workforce stability, hiring costs, team continuity, and organizational knowledge. This project uses an employee-level dataset to explore:

- How many employees are in the workforce, and how many have left?
- Which departments and job roles show higher observed attrition?
- How does attrition vary across tenure groups and demographic categories?
- How do salary bands, overtime, and satisfaction ratings relate to attrition patterns?

The goal is to turn the dataset into an interactive report that supports clear, evidence-based questions for further HR investigation.

## 📌 Key Metrics

| KPI | Dataset result |
|---|---:|
| 👥 Total employees | **2,000** |
| 🚪 Attrition count | **383** |
| 🟢 Active employees | **1,617** |
| 📉 Attrition rate | **19.15%** |
| 🔁 Retention rate | **80.85%** |
| 💰 Average monthly salary | **₹65,682** |
| 🗓️ Average tenure | **3.49 years** |

<sub>Values above are calculated from the full CSV with no slicers applied. They may change when report filters are selected.</sub>

## 🔎 Key Findings

The following are descriptive findings calculated from the included CSV:

- **Department variation:** Finance has the highest observed attrition rate at **21.12%** among departments in this dataset.
- **Overtime comparison:** The attrition rate is **31.84%** for employees marked `Yes` for overtime and **14.49%** for employees marked `No`.
- **Job satisfaction:** The attrition rate is **24.95%** for satisfaction rating 1 and **12.79%** for rating 4.
- **Early-tenure exits:** **259** employees who left had been at the company for three years or less. This represents **67.62%** of all leavers.

⚠️ **Interpretation:** These are associations and group comparisons. They do not prove that overtime, satisfaction, department, or tenure caused employees to leave.

## 🧭 Dashboard Walkthrough

### 1️⃣ HR Overview
A high-level view of employee headcount, attrition, active employees, attrition rate, average salary, department-level attrition, workforce distribution, age groups, and tenure patterns.

### 2️⃣ Employee Demographics
Explores the employee mix by gender, age group, marital status, and department, with a comparison of employee counts and attrition across gender categories.

### 3️⃣ Salary & Job Analysis
Examines salary distribution, average salary by department, job roles with the highest attrition counts, salary by attrition status, and attrition across salary bands.

### 4️⃣ Attrition Factors Analysis
Compares attrition across education, tenure, work-life balance, job satisfaction, overtime, and environment satisfaction.

## 🛠️ Tools & Skills

| Tool / Concept | How it is used |
|---|---|
| **Power BI Desktop** | Report design, visuals, slicers, and interactions |
| **Power Query** | Data import, inspection, and preparation |
| **DAX** | Measures, calculated columns, KPI calculations |
| **Data visualization** | KPI cards, bar charts, column charts, donut charts, 100% stacked bars |
| **Data analysis** | Group comparisons, distributions, and descriptive insights |
| **GitHub** | Versioned project presentation and documentation |

## 🗃️ Repository Structure

```text
HR-Employee-Attrition-Analytics/
│
├── README.md
├── .gitignore
│
├── assets/
│   ├── HR_Analytics_Project.pdf
│   └── dashboard-screenshots/
│       ├── page-1.png
│       ├── page-2.png
│       ├── page-3.png
│       └── page-4.png
│
├── data/
│   └── HR_Analytics_Employee_Attrition_Dataset.csv
│
├── docs/
│   ├── data-dictionary.md
│   ├── insights-and-findings.md
│   ├── methodology.md
│   └── quality-checks.md
│
└── powerbi/
    └── HR_Analytics_Project.pbix
```

## 🚀 How to Open the Project

1. Clone or download this repository.
2. Open `powerbi/HR_Analytics_Project.pbix` using **Power BI Desktop**.
3. If Power BI asks for the CSV source location, browse to `data/HR_Analytics_Employee_Attrition_Dataset.csv`.
4. Select **Apply changes** if prompted.
5. Use the report tabs and slicers to explore the dashboard.

## 📚 Project Documentation

- 📖 [Data Dictionary](docs/data-dictionary.md) – field names, meanings, and categories.
- 🧪 [Methodology](docs/methodology.md) – project workflow and metric definitions.
- 💡 [Insights & Findings](docs/insights-and-findings.md) – dataset-based observations.
- ✅ [Quality Checks](docs/quality-checks.md) – validation checks and publication notes.

## ⚠️ Data Disclaimer & Limitations

- The dataset is a **sample/synthetic portfolio dataset** and does not represent a real employer or actual employee records.
- The report is intended for learning and portfolio demonstration, not real employment decisions.
- Dashboard values respond to slicers; README metrics show the unfiltered dataset.
- Group differences are descriptive and should not be interpreted as causal relationships.
- Salary is recorded as **monthly income in INR**, not annual compensation.

## 👨‍💻 Author

**Hartik Manoj Bhati**  
B.Tech Computer Science & Engineering (Cyber Security)  
Interested in Data Analytics, Business Intelligence, and data-driven problem solving.

---

<div align="center">

### ⭐ If you find this project useful, consider giving the repository a star.

**Built with Power BI · DAX · Power Query · GitHub**

</div>
