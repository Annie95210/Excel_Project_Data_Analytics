# Project 2 — Market Analysis of Data Roles & Skills

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

#### Data Loading
- The transformed queries were loaded into the Excel workbook to support modeling and analysis.

### 📊 Analysis & Insights
- Roles requiring a broader set of skills tend to show higher median salaries.
- Jobs with fewer skill requirements generally fall into lower salary ranges.

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

**Why it matters:**  
These insights support informed decisions around job targeting, relocation, and salary negotiations.

---

## 3️⃣ What skills are most common in data roles?

### 🔧 Technique Used: Power Pivot

- A data model was created by linking job data with skill data using a shared job identifier.
- Cleaned data from Power Query enabled reliable relationships between tables.

### 📊 Analysis & Insights
- Skills such as SQL and Python appear most frequently across data-related jobs.
- Cloud and modern data technologies show strong representation, reflecting industry trends.

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

**Why it matters:**  
The analysis highlights which skills offer the strongest return on investment for career growth.

---

## Conclusion

This Excel-based project demonstrates how advanced spreadsheet tools can be used to analyze real-world job market data. By combining Power Query, PivotTables, DAX, and Power Pivot, the project uncovers clear relationships between skills, roles, and compensation.

The findings emphasize the importance of technical specialization—particularly in programming, databases, and cloud technologies—for professionals seeking higher-paying roles in the data field.

