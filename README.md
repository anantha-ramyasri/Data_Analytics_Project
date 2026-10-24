# 📊 HR Analytics Dashboard – Power BI

An interactive HR Analytics Dashboard built using Microsoft Power BI to analyze employee data, understand employee attrition, and identify workforce trends.

## 📌 Project Overview

The HR Analytics Dashboard provides insights into employee demographics, attrition patterns, job satisfaction, salary distribution, and employee tenure.

The dashboard presents key HR metrics through KPI cards, charts, and tables, helping users understand workforce trends and make data-driven HR decisions.

## 🎯 Project Objectives

- Analyze overall employee attrition.
- Understand attrition across education fields and job roles.
- Identify age groups with higher attrition.
- Examine attrition by salary range and years of service.
- Analyze job satisfaction across different job roles.
- Present HR metrics in an interactive visual dashboard.

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| Microsoft Power BI | Dashboard development and data visualization |
| Power Query | Data cleaning and transformation |
| DAX | Calculated measures and HR metrics |
| Data Modeling / Power Pivot | Relationships and data analysis |
| Data Visualization | Presenting HR insights through charts and KPI cards |

## 📈 Key Performance Indicators (KPIs)

The dashboard displays the following key metrics:

| KPI | Value |
|---|---:|
| Total Employees | 1.47K |
| Total Attrition | 237 |
| Attrition Percentage | 16% |
| Average Age | 37 |
| Average Salary | 6.50K |

*Note: Values are displayed as shown in the dashboard and may be rounded.*

## 📊 Dashboard Visualizations

### 1. Education-Wise Attrition
Analyzes employee attrition across different educational backgrounds to identify patterns among education fields.

### 2. Job-Wise Attrition
Compares attrition across job roles to understand which roles contribute more to employee turnover.

### 3. Attrition by Age
Shows attrition across age groups to identify workforce segments with higher employee turnover.

### 4. Attrition by Number of Years
Analyzes employee attrition based on years of service to identify tenure-related patterns.

### 5. Attrition by Salary Hike
Examines attrition across salary hike categories to explore the relationship between salary increases and employee turnover.

### 6. Attrition by Job Satisfaction
Presents job satisfaction ratings across job roles to compare satisfaction levels among employees.

## 🧹 Data Preparation

Data preparation is an important step in developing the dashboard.

- Cleaned and transformed the dataset using Power Query.
- Checked data types and prepared fields for analysis.
- Used relevant employee attributes to build visualizations.
- Created calculated measures for key HR metrics.

## 🧮 Key Measures

The dashboard includes measures for total employees, total attrition, attrition percentage, average age, and average salary.

Example DAX measures:

**Total Employees**
```dax
Total Employees = DISTINCTCOUNT('Data'[emp no])
```

**Total Attrition**
```dax
Total Attrition =
CALCULATE(
    DISTINCTCOUNT('Data'[emp no]),
    'Data'[Attrition] = "Yes"
)
```

**Attrition Percentage**
```dax
Attrition Percentage =
DIVIDE(
    [Total Attrition],
    [Total Employees],
    0
) * 100
```

*Adjust the table and column names to match your actual Power BI model. These examples assume that `Attrition` contains the text values `Yes` and `No`.*

## 💡 Key Insights

The dashboard helps HR teams explore:

- Overall employee attrition and workforce size.
- Differences in attrition across age groups and education fields.
- Job roles with comparatively higher employee turnover.
- Potential relationships between salary hikes and attrition.
- Job satisfaction patterns across different roles.
- Employee tenure patterns associated with attrition.

These insights can support further investigation into employee retention and workforce planning.

## 🚀 Skills Demonstrated

- Power BI dashboard development
- Data cleaning and transformation
- Power Query
- DAX measures
- KPI creation
- Data visualization
- HR data analysis
- Business intelligence and reporting

## 👩‍💻 Project By

**Anantha Ramya Sri**

Aspiring Data Analyst

---

⭐ *This project demonstrates how HR data can be transformed into an interactive dashboard for workforce analysis and data-driven decision-making.*
