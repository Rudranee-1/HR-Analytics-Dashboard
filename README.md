# HR-Analytics-Dashboard


## Project Objective
To help the organization identify patterns and insights that impact employee attrition and performance. This dashboard enables HR teams to take data-driven decisions that can improve employee retention, performance, and satisfaction.

---

## Tools Used
- **Power BI Desktop** – Data modeling & dashboard creation
- **Microsoft Excel** – Initial cleaning of CSV
- **DAX** – Custom measure creation
- **GitHub** – Project documentation and hosting

---

## Data Cleaning & Processing

- Removed **null values** and **duplicate rows**
- Copied raw CSV data into a new sheet to allow **Pivot compatibility**
- Handled categorical fields (e.g., Education, JobRole, AgeGroup)
- Imported clean data into Power BI for modeling and visualization

---

## KPIs & DAX Measures

| KPI | Value |
|-----|-------|
| **Total Employees** | 1,470 |
| **Attrition Count** | 237 |
| **Attrition Rate** | 16.1% |
| **Average Age** | 37 Years |
| **Average Tenure (Years at Company)** | 7.01 Years |
| **Average Income** | ₹6.5K/month |

### Sample DAX Calculations:

```dax
Attrition Rate = 
DIVIDE(
    CALCULATE(COUNT(Employee[EmployeeID]), Employee[Attrition] = "Yes"),
    COUNT(Employee[EmployeeID])
)

Avg Income = AVERAGE(Employee[MonthlyIncome])

Avg Age = AVERAGE(Employee[Age])
```

---

## Visuals Included in Dashboard

- KPI Cards: Attrition Rate, Avg Age, Avg Tenure, Avg Income

- Bar Charts:

  - Attrition by Education Field
  - Attrition by Job Role
  - Attrition by Age Group
  - Attrition by Avg Income Bucket
  - Gender Split
  - Department-wise Filtering
  - Job Role and Department Segmentation

- Slicers: Department, Gender, Education Field, Age Group

## Project Insights

 - Overall Attrition Rate: 16.1% (above ideal range of 10%)
 - Most attrition occurs between 26–35 age group
 - Job Roles with highest attrition:
   Laboratory Technicians (62)
   Sales Executives (57)
   Research Scientists (47)
 - Income Impact:
   Most attrition happens among employees earning below ₹5K
 - Education Field Impact:
   Highest attrition seen in Life Sciences (31.6%) and Medical (10.8%)
 - Gender Split:
   Male employees: 767
   Female employees: 489

## Project Learnings
- Identified key factors contributing to employee attrition
- Improved the hiring process based on data-driven insights
- Enhanced overall employee experience
- Made workforce more productive with performance tracking
- Gained employee trust by acting on HR data insights

## Industry Benchmark Insights

| Metric              | Standard  | Your Data                 |
| ------------------- | --------- | ------------------------- |
| Attrition Rate      | < 10%     | 16.1%                    |
| Avg Income          | ₹6–10K    | ₹6.5K                    |
| Age Group Stability | 35–45 yrs | High attrition at 26–35  |
| Tenure Stability    | > 3 yrs   | Avg 7.01 yrs             |

---

### Dashboard Preview

![HR Analytics Dashboard](https://github.com/Rudranee-1/HR-Analytics-Dashboard/blob/main/HR%20Analytics%20Dashboard.jpg) 




