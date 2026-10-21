# Like-for-Like (LFL) Performance Analysis

## Summary
An end-to-end Like-for-Like performance analysis comparing 2026 with 2025 by matching trading days rather than simply comparing calendar dates. The analysis was implemented in Databricks using SQL and organized into Gold-layer tables for Current Year, Previous Year, and LFL comparison. Built during the DataMelon Labs Industry Fellowship.

**Tools:** Databricks | SQL | Power BI

## Business Problem
Calendar-date comparisons can be distorted when the number or pattern of trading days differs between periods. The project focused on creating a comparable performance view using matched trading days.

## Work Performed
- Built the LFL analysis in Databricks using SQL
- Matched current-year and previous-year trading days
- Created Gold-layer tables for Current Year, Previous Year, and LFL comparison
- Analyzed LFL sales and transaction growth
- Performed regional, city, department, and monthly momentum analysis

## Key Findings

| Area | Result |
|------|--------|
| Overall LFL sales growth | **+19.33%** |
| Transaction growth | **+20.90%** |
| Regions | West recorded **+21.68%** growth, with all regions showing double-digit growth |
| Cities | Nagpur **+27.13%**, Noida **+26.14%** |
| Departments | Household **+32.38%**, while core categories remained around **18-20%** growth |
| Monthly trend | Growth stayed in the **18-22%** range, with no significant seasonality observed |

## Business Impact
The LFL approach provides a more comparable view of business performance by controlling for differences in trading days. Growth was broad-based across regions, cities, departments, and months rather than being concentrated in a single area.

## Files
- lfl_performance.sql: SQL queries for the Gold-layer tables
- lfl_performance_dashboard.pdf: dashboard exported as PDF
