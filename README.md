# Loan-Approval-Analysis-SQL-PowerBI-Python
End-to-end data analysis project on loan approval prediction using SQL Server, Power BI and Python — covering data cleaning, EDA, visualization and machine learning.

# Loan Approval Decoded — What Banks Really Look For

## Project Overview
An end-to-end data analysis project analyzing 614 loan applications 
to uncover what factors drive loan approval decisions at banks.
Starting from raw uncleaned data, this project covers the complete 
data analytics pipeline — cleaning, transformation, SQL analysis, 
interactive dashboarding and machine learning prediction.
Built using SQL Server, Power BI and Python.

## Project Objectives
- Identify the key factors that influence loan approval decisions
- Analyze demographic patterns across gender, education, 
  marital status and employment type
- Understand the relationship between income, loan amount 
  and repayment capacity
- Segment applicants by risk tier and measure approval rates per tier
- Derive financial metrics like DTI ratio and EMI to assess 
  repayment burden
- Build machine learning models to predict loan approval outcome
- Present findings through an interactive Power BI dashboard

## Key Findings

### Credit & Risk
- Credit history is the #1 predictor of approval — good credit 
  achieves 79% approval vs just 7% for bad credit
- Even high income earners with bad credit get approved only 13% 
  of the time — money cannot compensate for poor credit
- High risk applicants have only 20% approval vs 87% for low risk
- 50 applicants had missing credit history — the largest NULL 
  count in the dataset

### Income & Financial
- Rejected applicants earn MORE on average (₹6,771) than approved 
  ones (₹6,414) — income alone does not drive approval
- Rejected applicants carry higher DTI (8.47%) vs approved (7.57%)
- Rejected applicants have higher average EMI burden (₹482 vs ₹463)
- Approval rates are nearly identical across all income brackets 
  — only a 3% difference between lowest and highest earners
- Rural applicants borrow the most on average but have the 
  lowest approval rate

### Demographics
- Semiurban areas lead with 76% approval — 15% higher than rural
- Graduates consistently achieve 70% approval regardless of 
  whether they are salaried or self employed
- Married applicants have 9% higher approval than unmarried ones
- Self employment has zero impact — both salaried and self 
  employed achieve 68% approval
- Gender gap is minimal — Male 69% vs Female 67%
- Applicants with 2 dependents surprisingly achieve the highest 
  approval at 75%

## Tools & Technologies
- SQL Server — data cleaning, transformation, 17 analysis queries
- Power BI — 3 page interactive dashboard with DAX measures
- Python — EDA, visualization, machine learning models
- Google Colab — Python development environment
- GitHub — version control and project documentation

## Project Structure
## Data Cleaning Steps
1. Identified NULL values across all 13 columns
2. Verified mode for all categorical columns before imputing
3. Fixed data types — converted 3 columns from nvarchar 
   to correct numeric types
4. Imputed categorical NULLs with mode values
5. Imputed LoanAmount NULLs with column average
6. Fixed Dependents encoding — replaced 3+ with 3
7. Capped ApplicantIncome outliers at 3x average (₹16,209)
8. Capped LoanAmount outliers at 3x average (₹439.20)

## Derived Columns Added
| Column | Formula | Purpose |
| Household Income | ApplicantIncome + CoapplicantIncome | Total family income |
| LoanAmount Actual | LoanAmount × 1000 | Loan in actual rupees |
| EMI | LoanAmount Actual / Loan Term | Monthly payment estimate |
| DTI Ratio | (EMI / Household Income) × 100 | Repayment burden % |

## SQL Analysis Modules
| Module | Queries | Focus |
|---|---|---|
| A | Q1-Q5 | Overall and demographic approval rates |
| B | Q6-Q8 | Credit history and risk segmentation |
| C | Q9-Q12 | Income and loan amount insights |
| D | Q13-Q15 | Employment and dependent analysis |
| E | Q16-Q17 | Edge cases and high risk scenarios |

## Power BI Dashboard
### Page 1 — Executive Summary
- Total applications KPI card
- Approval rate gauge
- Approved vs rejected donut chart
- Approval by property area bar chart
- Credit history impact bar chart

### Page 2 — Demographic Breakdown
- Approval by gender
- Approval by education pie chart
- Approval by marital status
- Approval by dependents column chart
- Approval by income bracket funnel

### Page 3 — Risk & Financial Analysis
- Risk tier donut chart
- Loan amount histogram
- Good vs bad credit KPI cards
- Average DTI by loan status
- Average EMI by loan status

## Machine Learning Models
| Logistic Regression |
| Decision Tree | 
| Random Forest | 

## Dataset
- Source: Kaggle — Finance Loan Approval Prediction Data
- 614 rows, 13 original columns
- 4 derived columns added during cleaning
- Link: https://www.kaggle.com/datasets/krishnaraj30/
  finance-loan-approval-prediction-data

## Author
Nandhitha Kannan
