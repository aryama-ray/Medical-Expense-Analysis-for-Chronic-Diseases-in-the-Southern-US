# 💊 Medical Expense Analysis for Chronic Diseases in the Southern US

## 📌 Overview

This project investigates the **cost drivers** behind the high medical expenses associated with chronic health conditions such as **Blood Pressure, Arthritis, Cardiovascular Disease, and Cancer**. Using the **Medical Expenditure Panel Survey (MEPS)** data, the analysis focuses on:

- Understanding how **healthcare resources are distributed and utilized**
- Evaluating how well **insurance policies support patients**
- Identifying **demographic and socioeconomic disparities** in healthcare costs

---

## 🧠 Objective

To perform data-driven analysis and hypothesis testing to uncover insights into the distribution of healthcare expenses, supporting policy recommendations and optimized resource allocation for chronic disease management in the United States.

---

## 🗃️ Dataset

**Source:** [Medical Expenditure Panel Survey (MEPS)](https://meps.ahrq.gov/mepsweb/)

**Years Considered:** 2020, 2021, 2022

| Year | Records | Features |
|------|---------|----------|
| 2020 | 27,805  | 1,452    |
| 2021 | 28,337  | 1,488    |
| 2022 | 22,432  | 1,420    |

**Final Cleaned Dataset:** `15,549` rows × `62` features

---

## 🧹 Data Processing Workflow

```text
Input Datasets (2020-2022)
        ↓
Data Cleaning
• Renamed columns
• Removed negative values
        ↓
Merge & Filter
• Merged datasets
• Filtered individuals with chronic diseases
        ↓
Feature Selection
• Selected Demographics, Geography, Expenses, Insurance, Disease Codes
        ↓
Handle Missing Data
• Imputation using median/mode by subgroup
        ↓
Outlier Removal
• Z-score based filtering on expenditures
        ↓
Feature Engineering
• Derived Sub-total Expenditure
• Created Critical Comorbidity indicator
        ↓
Final Output
• Preprocessed dataset ready for EDA & modeling
```
---

## 🛠️ Tools & Technologies

Python: pandas, numpy, seaborn, scikit-learn

Power BI: Interactive dashboard visualizations

Jupyter Notebook: EDA and modeling environment

Git & GitHub: Version control

## 🔍 Exploratory Data Analysis & Hypothesis Testing
We explored relationships between chronic disease costs and variables like:

 - Insurance Type

 - Income Group

 - Age Group

 - Disease Type

 - Emergency Visits

### Hypothesis Testing was conducted to assess:

If insurance type influences out-of-pocket expenses

If individuals with multiple comorbidities have significantly higher total expenses

If income level and geography affect expenditure disparities

Statistical Significance: All validated hypotheses had p-value < 0.05.

## Key Insights
Insurance coverage plays a critical role in reducing out-of-pocket expenses.

Age and comorbidity levels are strong predictors of healthcare costs.

Disparities exist in total expenditure based on income and geography.

Policy optimizations can be targeted to underserved demographics to reduce cost burden.

