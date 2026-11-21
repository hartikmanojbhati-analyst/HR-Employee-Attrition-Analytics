# Quality Checks and Publication Notes

## CSV checks

- Rows: 2,000
- Columns: 23
- Distinct employee IDs: 2,000
- Duplicate employee IDs: 0
- Missing cells: 0
- Attrition categories: No, Yes
- Overtime categories: No, Yes

## Items to verify in Power BI before publishing

1. **Page 4 Early Attrition KPI:** The PDF displays 22.12%. For tenure ≤3 years, the CSV gives 259 leavers, equal to 67.62% of leavers or 12.95% of all employees. Confirm the measure's numerator, denominator, filter context, and title.
2. **Page 2 visual title:** The PDF's upper-right donut is labelled “Attrition Trend by Years at Company” but displays marital-status categories. Rename it to “Employees by Marital Status” if that is the intended visual.
3. **Page 3 salary totals:** The CSV sum is ₹131,365,000; the PDF rounds it to ₹131.37M. This is the sum of monthly income values in the dataset, not an annual payroll amount.
4. **Page 3 salary-by-department:** Ensure labels are formatted as INR and use the actual average from the current filter context.
5. **Page 4 satisfaction labels:** The report uses Very Low, Low, Medium, High for ratings 1–4. Keep this mapping consistent across job, work-life balance, and environment satisfaction.

## GitHub publication

- Check that the PBIX opens and its source path is correctly configured.
- Ensure the PDF screenshots match the final PBIX.
- Do not commit private or real employee data. The included CSV is a sample/synthetic dataset.
- Add a license only if you have chosen terms for reuse. Do not add a license by default.
- If GitHub rejects a file due to size, use Git LFS for the PBIX or PDF.
