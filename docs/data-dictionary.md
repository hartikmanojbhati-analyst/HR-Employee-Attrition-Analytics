# Data Dictionary

The source file contains **2,000 rows and 23 columns**. Each row represents one employee record in the sample dataset.

| Column | Data type | Description |
|---|---|---|
| `Employee_ID` | Text | Unique employee identifier. |
| `Age` | Whole number | Employee age in years. |
| `Gender` | Text | Gender category recorded in the dataset. |
| `Marital_Status` | Text | Marital status category. |
| `Department` | Text | Employee department. |
| `Job_Role` | Text | Employee job role. |
| `Education` | Text | Education level category. |
| `Education_Field` | Text | Field of education. |
| `Business_Travel` | Text | Business travel frequency/category. |
| `Distance_From_Home_KM` | Whole number | Distance from home in kilometres. |
| `Monthly_Income_INR` | Whole number | Monthly income in Indian rupees. |
| `Overtime` | Text | Overtime indicator (`Yes`/`No`). |
| `Job_Satisfaction` | Whole number | Job satisfaction rating, 1–4. |
| `Environment_Satisfaction` | Whole number | Environment satisfaction rating, 1–4. |
| `Work_Life_Balance` | Whole number | Work-life balance rating, 1–4. |
| `Relationship_Satisfaction` | Whole number | Relationship satisfaction rating, 1–4. |
| `Performance_Rating` | Whole number | Performance rating. |
| `Training_Times_Last_Year` | Whole number | Number of training sessions in the previous year. |
| `Total_Working_Years` | Whole number | Total working experience in years. |
| `Years_At_Company` | Whole number | Tenure at the current company in years. |
| `Years_In_Current_Role` | Whole number | Years in the current role. |
| `Years_With_Current_Manager` | Whole number | Years with the current manager. |
| `Attrition` | Text | Whether the employee left (`Yes`/`No`). |

## Categories and interpretation

- Satisfaction fields use numeric ratings from 1 to 4. In the report, these are displayed as Very Low, Low, Medium, and High.
- `Overtime` contains `Yes` and `No` only.
- `Gender`, `Department`, `Job_Role`, `Education`, and `Marital_Status` are categorical fields.
- `Monthly_Income_INR` is a monthly salary value, not annual compensation.

## Data handling

The CSV is a sample/synthetic portfolio dataset. Do not treat it as real employee data or use it to make actual employment decisions.
