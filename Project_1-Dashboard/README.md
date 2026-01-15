# 📊 Excel Data Analytics: Salary Dashboard
![Excel](https://img.shields.io/badge/Tool-Microsoft%20Excel-green)
![Status](https://img.shields.io/badge/Project-Completed-blue)
![Focus](https://img.shields.io/badge/Focus-Data%20Analytics-orange)
![Final_Dashboard](https://github.com/user-attachments/assets/e63a7b7f-7570-4f6d-b996-48af8b1fcaf5)

## Overview
This project is an interactive Salary Dashboard built in Microsoft Excel as part of my Excel for Data Analytics course.

The dashboard analyzes job market salary data across roles, countries, work types, platforms, and employment conditions, enabling users to explore salary trends and make data-driven insights.

### Dashboard File
My final dashboard is in [1_Salary_Dashboard](1_Salary_Dashboard.xlsx)

## 🛠️ Tools & Technologies
- **Microsoft Excel**
  - Charts
  - Advanced Formulas and Functions
  - Data Validation & drop-down filters
- **Analytical Techniques**
  - Data structuring
  - Interactive reporting
  - Trend comparison

## 📁 Workbook Structure
| Sheet Name | Description |
|----------|-------------|
| **Data** | Raw dataset with job roles, salary details, location, skills, and benefits |
| **Salary_Calculator** | Main interactive dashboard |
| **Data_Validation** | Controls drop-downs and filter logic |
| **Jobs** | Job role classifications |
| **Country** | Country-based analysis |
| **Type** | Salary type (Yearly) |
| **Platform** | Job posting platforms |

## 📊 Dashboard Features
### 📉 Charts

#### 📊 Data Science Job Salaries - Bar Chart
<img width="436" height="289" alt="image" src="https://github.com/user-attachments/assets/c474da80-7bd2-4948-b93c-676cf9dd3d3d" />

- 🛠️ **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 **Design Choice:** Horizontal bar chart for visual comparison of median salaries.
- 📉 **Data Organization:** Sorted job titles by descending salary for improved readability.
- 💡 **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

#### 🗺️ Country Median Salaries - Map Chart

![Map_Chart](https://github.com/user-attachments/assets/0af33e51-42f5-460c-bb4a-c6083a34a53e)

- 🛠️ **Excel Features:** Utilized Excel's map chart feature to plot median salaries globally.
- 🎨 **Design Choice:** Color-coded map to visually differentiate salary levels across regions.
- 📊 **Data Representation:** Plotted median salary for each country with available data.
- 👁️ **Visual Enhancement:** Improved readability and immediate understanding of geographic salary trends.
- 💡 **Insights Gained:** Enables quick grasp of global salary disparities and highlights high/low salary regions.

### 🧮 Formulas and Functions

#### 💰 Median Salary by Job Titles

```
=MEDIAN(
  IF((jobs[job_title_short]=A2)*
    (jobs[salary_year_avg]<>0)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type]))),
    jobs[salary_year_avg]))
```

- 🔍 **Multi-Criteria Filtering:** Checks job title, country, schedule type, and excludes blank salaries.
- 📊 **Array Formula:** Utilizes `MEDIAN()` function with nested `IF()` statement to analyze an array.
- 🎯 **Tailored Insights:** Provides specific salary information for job titles, regions, and schedule types.
- 🔢 **Formula Purpose:** This formula populates the table below, returning the median salary based on job title, country, and type specified.

🍽️ Background Table

<img width="388" height="317" alt="image" src="https://github.com/user-attachments/assets/def9cf6b-dd14-48d5-b603-d6941e9776f8" />

📉 Dashboard Implementation

<img width="495" height="703" alt="image" src="https://github.com/user-attachments/assets/6010c78f-7075-4b25-b92c-600b5467453c" />

#### ⏰ Count of Job Schedule Type

```
=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#)))*(J2#<>0)))
```

- 🔍 **Unique List Generation:** This Excel formula below employs the `FILTER()` function to exclude entries containing "and" or commas, and omit zero values.
- 🔢 **Formula Purpose:** This formula populates the table below, which gives us a list of unique job schedule types.

🍽️ Background Table

<img width="315" height="100" alt="image" src="https://github.com/user-attachments/assets/ecab4952-5861-48a2-9824-2af41b051376" />

📉 Dashboard Implementation:

<img width="571" height="711" alt="image" src="https://github.com/user-attachments/assets/36a6adfe-f381-4886-a1c5-34c653637b8a" />

### ❎ Data Validation

#### 🔍 Filtered List

- 🔒 **Enhanced Data Validation:** Implementing the filtered list as a data validation rule under the `Job Title`, `Country`, and `Type` option in the Data tab ensures:
    - 🎯 User input is restricted to predefined, validated schedule types
    - 🚫 Incorrect or inconsistent entries are prevented
    - 👥 Overall usability of the dashboard is enhanced

![Data_Validation](https://github.com/user-attachments/assets/c474bee3-5b68-42c4-a352-626bca99d638)

---
## 📈 Business Questions Answered
- Which roles offer the highest salaries?
- How do salaries vary across countries?
- Which platforms show better salary offerings?

---
## 📌 Key Takeaway
This project demonstrates how **Excel alone** can be used as a powerful analytics and visualization tool—mirroring real-world business dashboards without external BI software.
