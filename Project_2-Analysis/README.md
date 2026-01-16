# Excel Data Analytics: Market Analysis of Data Roles and Skills

## Introduction

While exploring opportunities in the data field, I noticed that many career decisions are made with limited insight into how **skills, roles, and compensation** are actually connected. This project was created to address that gap by analyzing job market data to understand which skills are most valuable and how they influence salary outcomes.

The objective of this analysis is to provide practical, data-driven guidance for professionals navigating the data job market.

---

## Questions Explored

To better understand current market dynamics, the following questions were investigated:

1. **Does having more skills lead to higher pay?**
2. **How do salaries vary across geographic regions?**
3. **Which skills appear most frequently in data-related roles?**
4. **What salary levels are associated with the most in-demand skills?**

---

## Excel Skills Applied

This project demonstrates the use of advanced Excel features, including:

- 📊 **Pivot Tables**
- 📈 **Pivot Charts**
- 🧮 **DAX (Data Analysis Expressions)**
- 🔍 **Power Query**
- 💪 **Power Pivot**

---

## Dataset Overview

The analysis is based on real-world job posting data from 2023, focusing on roles within the data and analytics domain. The dataset provides a strong foundation for applying Excel-based analytics techniques.

Key fields include:

- 👨‍💼 Job titles  
- 💰 Salary information  
- 📍 Job location  
- 🛠️ Required skills  

---

## 1️⃣ Do roles with more skills offer higher pay?

### 🔍 Technique Used: Power Query (ETL)

#### Data Extraction
- The raw dataset was imported into Excel using Power Query.
- Two queries were created:
  - One containing job-level information.
  - One listing skills associated with each job ID.

#### Data Transformation
- Columns were cleaned and standardized by:
  - Assigning correct data types
  - Removing unnecessary fields
  - Cleaning text values
  - Trimming excess whitespace
    
    - 📊 data_jobs_all

<img width="366" height="516" alt="image" src="https://github.com/user-attachments/assets/c0f6f4fa-88b8-490a-9acf-d8538359ab2a" />

   - 🛠️ data_job_skills
    
<img width="366" height="523" alt="image" src="https://github.com/user-attachments/assets/5ff9b959-a00a-412b-95a5-2ec689d00026" />

#### Data Loading
- The transformed queries were loaded into the Excel workbook to support modeling and analysis.
  
    - 📊 data_jobs_all
<img width="1914" height="932" alt="image" src="https://github.com/user-attachments/assets/a22f36dc-559b-456a-ba71-7f921300bb24" />
  
    - 🛠️ data_job_skills
<img width="1919" height="973" alt="image" src="https://github.com/user-attachments/assets/7a068a85-ba5f-4174-8fcf-e3fc8e43d965" />

### 📊 Analysis & Insights
- Roles requiring a broader set of skills tend to show higher median salaries.
- Jobs with fewer skill requirements generally fall into lower salary ranges.

<img width="823" height="492" alt="image" src="https://github.com/user-attachments/assets/7c423806-ca1a-4901-9d61-134ff5547638" />

**Why it matters:**  
Building a broader and more specialized skill set can positively influence earning potential, especially for senior and technical roles.

---

## 2️⃣ How do salaries vary by region?

### 🧮 Techniques Used: Pivot Tables & DAX

- A PivotTable was created using the Excel Data Model.
- Job titles were placed in the rows, with salary values aggregated in the values area.
- Median salary was calculated using DAX to reduce the impact of outliers.
- Additional filtering was applied to compare U.S. and non-U.S. roles.

### 📊 Analysis & Insights
- Senior data roles consistently command higher salaries across regions.
- U.S.-based positions generally offer higher median pay, particularly in technical roles.
  
<img width="1133" height="436" alt="image" src="https://github.com/user-attachments/assets/ae0b850e-e524-478f-ab99-a0670bfebd4d" />

**Why it matters:**  
These insights support informed decisions around job targeting, relocation, and salary negotiations.

---

## 3️⃣ What skills are most common in data roles?

### 🔧 Technique Used: Power Pivot

- A data model was created by linking job data with skill data using a shared job identifier.
- 
<img width="1788" height="1264" alt="2_Project_Analysis_Screenshot5" src="https://github.com/user-attachments/assets/875c7e7d-30da-42c8-9cf0-56ec8be56ada" />

- Cleaned data from Power Query enabled reliable relationships between tables.

<img width="1914" height="978" alt="image" src="https://github.com/user-attachments/assets/9ffc3f4b-f8e0-4eab-9ab6-10f08303be76" />

### 📊 Analysis & Insights
- Skills such as SQL and Python appear most frequently across data-related jobs.
- Cloud and modern data technologies show strong representation, reflecting industry trends.

<img width="719" height="463" alt="image" src="https://github.com/user-attachments/assets/6b478d8e-9dd7-4162-a757-756d50bbe14c" />

**Why it matters:**  
Understanding commonly required skills helps professionals prioritize learning and stay aligned with market demand.

---

## 4️⃣ What is the salary impact of the top skills?

### 📊 Technique Used: Advanced Pivot Charts

- A combo PivotChart was created to visualize:
  - Median salary by skill (column chart)
  - Skill prevalence as a percentage (secondary axis)
- The chart was customized to emphasize differences in salary impact.

### 📊 Analysis & Insights
- Technical skills like Python and SQL are associated with higher median salaries.
- General productivity tools correlate with lower pay and lower demand.
  
<img width="809" height="419" alt="image" src="https://github.com/user-attachments/assets/cf079ba9-231c-4c1f-98e7-3e6c2b9f18bb" />

**Why it matters:**  
The analysis highlights which skills offer the strongest return on investment for career growth.

---

## Conclusion

This Excel-based project demonstrates how advanced spreadsheet tools can be used to analyze real-world job market data. By combining Power Query, PivotTables, DAX, and Power Pivot, the project uncovers clear relationships between skills, roles, and compensation.

The findings emphasize the importance of technical specialization—particularly in programming, databases, and cloud technologies—for professionals seeking higher-paying roles in the data field.

