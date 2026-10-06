# Loan Default & Financial Risk Analysis – Power BI

### Dashboard Link

[View Live Dashboard](https://app.powerbi.com/groups/e4c01094-6937-4fd5-86b5-754b4c828690/reports/f9852f8c-fe1a-4fd1-a083-d921180d6318/f1c3b39f85521f79474a?experience=power-bi)

---

## Problem Statement

This project focuses on analyzing **loan applications, loan amounts, customer demographics, financial profiles, and loan default behavior** using Microsoft Power BI.

The dashboard helps analyze important financial and customer-related patterns such as:

- Loan Amount by Purpose
- Average Income by Employment Type
- Default Rate by Employment Type
- Average Loan Amount by Age Group
- Default Rate by Year
- Median Loan Amount by Credit Score
- Education-wise Loan Analysis
- Age Group and Marital Status Analysis
- Mortgage and Dependents Analysis
- YOY Loan Amount Change
- YOY Default Loans Change
- YTD Loan Amount
- Financial Risk Analysis

The main objective is to transform raw loan data into an **interactive financial analytics dashboard** that can help identify lending patterns and potential risk areas.

---

## Dataset

The project uses a loan default dataset containing **255,347 records and 19 columns**.

### Main Columns

- LoanID
- Age
- Income
- LoanAmount
- CreditScore
- MonthsEmployed
- NumCreditLines
- InterestRate
- LoanTerm
- DTIRatio
- Education
- EmploymentType
- MaritalStatus
- HasMortgage
- HasDependents
- LoanPurpose
- HasCoSigner
- Default
- Loan Date

---

## Tools & Technologies

- **Microsoft Power BI Desktop**
- **Power BI Service**
- **Power Query**
- **DAX**
- **SQL Server**
- **Power BI Dataflow**
- **CSV / Excel**

---

## Steps Followed

- **Step 1:** Loaded the loan dataset into SQL Server.

- **Step 2:** Created a Power BI Dataflow and imported the required data into Power BI Desktop.

- **Step 3:** Used Power Query Editor to analyze, clean and transform the data according to dashboard requirements.

- **Step 4:** Converted the Loan Date column into a proper date format.

- **Step 5:** Created a **Year** column from the Loan Date.

```DAX
Year =
YEAR('Loan_default'[Loan_Date_DD_MM_YYYY])
```

- **Step 6:** Created an **Age Group** column to categorize customers into different age groups:

  - Teen
  - Adults
  - Middle Age Adults
  - Senior Citizens

- **Step 7:** Created **Credit Score Bins**:

  - Very Low
  - Low
  - Medium
  - High

- **Step 8:** Created **Income Brackets**:

  - Low Income
  - Medium Income
  - High Income

- **Step 9:** Used SQL Server to load, analyze and validate the data.

- **Step 10:** Created different DAX measures according to the analysis requirements.

- **Step 11:** Created interactive charts, cards, tables, decomposition tree and other Power BI visuals.

- **Step 12:** Created YOY and YTD calculations for time-based analysis.

- **Step 13:** Published the report to Power BI Service.

- **Step 14:** Configured Dataflow, Scheduled Refresh and Incremental Refresh.

---

# DAX Measures & Calculations

Several DAX measures and calculated columns were created for the analysis.

### Average Income by Employment Type

Used to analyze the average income of customers across different employment categories.

### Default Rate by Employment Type

Used to compare the default rate among different employment types.

### Average Loan Amount by Age Group

Used to compare average loan amounts across different age groups.

### Median Loan Amount by Credit Score

Used to analyze the median loan amount across different credit score categories.

### Loan Count by Education

Used to analyze the number of loans across different education categories.

### YOY Loan Amount Change

Used to calculate the year-over-year percentage change in loan amount.

### YOY Default Loans Change

Used to analyze the year-over-year change in default loans.

### YTD Loan Amount

Used to calculate the Year-to-Date loan amount using DAX time-intelligence functions.

### Decomposition Tree

Used to break down loan amount based on:

- Income Bracket
- Employment Type

---

# Dashboard Pages

## Page 1 – Loan Default & Overview

This page provides an overall analysis of loan performance and default behavior.

### Key Analysis

- Loan Amount by Purpose
- Average Income by Employment Type
- Default Rate (%) by Employment Type
- Average Loan Amount by Age Group
- Default Rate (%) by Year

### Page 1 Dashboard

<img width="1160" height="653" alt="Loan Default & Overview Dashboard" src="https://github.com/user-attachments/assets/2710c2f6-62c2-4e5e-a1f6-bf8d92f79392" />

---

## Page 2 – Applicant Demographics & Financial Profile

This page focuses on applicant demographics and financial characteristics.

### Key Analysis

- Median Loan Amount by Credit Score Category
- Average Loan Amount by Age Group and Marital Status
- Total Loan Amount by Credit Score Bins
- Loan Amount by Mortgage / Dependents
- Number of Loans by Education Type

### Page 2 Dashboard

<img width="1161" height="655" alt="Applicant Demographics & Financial Profile Dashboard" src="https://github.com/user-attachments/assets/c60757c4-965e-4c44-a30c-db1b7b8c8aed" />

---

## Page 3 – Financial Risk Metrics

This page focuses on financial risk and time-based analysis.

### Key Analysis

- YOY Loan Amount Change by Year
- YOY Default Loans Change by Year
- YTD Loan Amount by Credit Score Bins and Marital Status
- Loan Amount by Income Bracket
- Employment Type Analysis
- Decomposition Tree for Financial Risk Analysis

### Page 3 Dashboard

<img width="1157" height="651" alt="Financial Risk Metrics Dashboard" src="https://github.com/user-attachments/assets/43b6ac32-ba0a-4f7b-800b-4face5360689" />

---

# Interactive Analysis

The dashboard allows users to analyze loan data across multiple dimensions:

- Year
- Age Group
- Credit Score
- Income Bracket
- Employment Type
- Education
- Marital Status
- Mortgage
- Dependents
- Loan Purpose

The interactive Power BI visuals make it possible to explore relationships between different customer and loan characteristics.

---

# Power BI Service

The report was published to **Power BI Service**.

The project includes:

- Power BI Dataflow
- Scheduled Refresh
- Incremental Refresh
- Report Publishing

These features help maintain and refresh the dashboard data efficiently.

---

# Key Insights

### 1. Loan Amount by Purpose

Loan amounts were analyzed across different loan purposes to understand which categories contribute most to the overall loan portfolio.

### 2. Average Income by Employment Type

Average income was compared across different employment categories to understand differences in customer financial profiles.

### 3. Default Rate by Employment Type

Default rates were analyzed across employment types to identify groups with relatively higher or lower default risk.

### 4. Average Loan Amount by Age Group

Average loan amounts were compared across different age groups to understand borrowing behavior.

### 5. Default Rate by Year

Default rates were analyzed across different years to identify changes in default behavior over time.

### 6. Credit Score Analysis

Loan amounts were analyzed across:

- Very Low
- Low
- Medium
- High

credit score categories to understand the relationship between credit profile and lending.

### 7. Education Analysis

The number of loans was analyzed across different education categories.

### 8. Financial Risk Analysis

YOY and YTD measures were created to analyze changes in loan activity and default behavior over time.

### 9. Income & Employment Analysis

The Decomposition Tree was used to explore loan amount based on **Income Bracket** and **Employment Type**.

---

# Skills Demonstrated

- Data Cleaning
- Data Transformation
- SQL Server
- Power Query
- DAX
- Data Modeling
- Time Intelligence
- YOY Analysis
- YTD Analysis
- Financial Risk Analysis
- Data Visualization
- Interactive Dashboard Development
- Power BI Service
- Dataflow
- Scheduled Refresh
- Incremental Refresh

---

# Project Workflow

```text
Loan Dataset
     ↓
SQL Server
     ↓
Data Validation & Analysis
     ↓
Power BI Dataflow
     ↓
Power Query
     ↓
Data Transformation
     ↓
DAX Measures & Calculated Columns
     ↓
Interactive Power BI Dashboard
     ↓
Power BI Service
     ↓
Scheduled / Incremental Refresh
```

---

# Project Files

```text
Loan-Default-PowerBI-Project/
│
├── README.md
├── Loan_default.csv
├── Column Definitions.xlsx
├── Loan Dataset Link.xlsx
└── Loan data analysis Power BI project.pbix
```

---

# Project Outcome

This project demonstrates an end-to-end **loan data analytics workflow** using SQL Server and Power BI.

The final dashboard combines **data cleaning, transformation, SQL validation, DAX calculations, financial risk analysis, time intelligence and interactive visualization** to provide a comprehensive view of loan and default behavior.

---

# Author

**Jay Prakash Patel**

B.Tech CSE (AIML) | SOIT RGPV Bhopal


