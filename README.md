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
