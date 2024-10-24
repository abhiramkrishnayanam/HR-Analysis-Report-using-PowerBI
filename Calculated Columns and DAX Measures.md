# Power BI - Calculated Columns and DAX Measures: README
This README outlines the steps to create calculated columns and DAX measures in Power BI based on the Employee dataset. Follow these instructions to enhance your data model and create insightful visualizations.

## 1. Calculated Columns
## 1.1 Age Group
This calculated column categorizes employees into specific age groups: 20-30, 31-40, 41-50, and 50+.

## DAX Formula:

Age Group = 
IF(Employee[Age] <= 30, "20-30", 
IF(Employee[Age] <= 40, "31-40", 
IF(Employee[Age] <= 50, "41-50", "50+")))

**Steps:**

In Power BI Desktop, go to the Modeling tab.
Select New Column.
Copy and paste the above DAX formula in the formula bar.
Press Enter.

## 1.2 Tenure Band
This calculated column groups employees based on how many years they’ve worked at the company: 0-4 Years, 5-9 Years, and 10+ Years.

## DAX Formula:
dax
Tenure Band = 
IF(Employee[YearsAtCompany] < 5, "0-4 Years", 
IF(Employee[YearsAtCompany] < 10, "5-9 Years", "10+ Years"))



