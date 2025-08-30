# 🔍💳 Credit Risk Analysis - Statistical and Inferential Insights

This project explores the **German Credit** dataset using **statistical inference** to identify factors associated with credit risk.  
The analysis investigates how **loan characteristics** (credit amount, duration) and **customer attributes** (savings, checking accounts, housing, job, age, purpose, etc.) influence the likelihood of default.  

The goal is to uncover **meaningful patterns** in credit behavior, evaluate **predictors of risk**, and provide a solid statistical foundation for future credit risk modeling.

<!-- Row 1: first image -->
<p align="center">
  <img src="https://github.com/user-attachments/assets/de67d589-20b6-44ff-90e1-0f9e422a35cc"/>
</p>

<!-- Row 2: second image -->
<p align="center">
  <img src="https://github.com/user-attachments/assets/e13533ee-de81-4447-820a-e90aa92f064e"/>
</p>

## 🗃️ Dataset Overview

The dataset contains records of **1,000 credit applicants** with 20 attributes, both numerical and categorical.  
Key variables include:

- **Credit Characteristics:** Credit amount, Duration, Purpose  
- **Financial Accounts:** Checking account, Saving account  
- **Demographics:** Sex, Age group, Job, Housing  
- **Target:** Risk (good / bad)

Each row represents an applicant’s credit profile and outcome.

## 🛠 Libraries

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scipy  
- statsmodels  

## 📊 Insights & Results
    
📈 **Bad-risk borrowers** request larger loan amounts and longer durations.  
🏦 **Checking** and **Saving accounts** show the strongest associations with credit risk (small-to-moderate effects).  
🏠 **Housing** and 👤 **Age group** are significant but weaker predictors, while **Job** and **Purpose** show no strong association.  
⚖️ Credit risk is **moderately imbalanced**, requiring careful handling in predictive modeling.  

## 🧱 Workflow Overview

### 1. **Exploratory Data Analysis**
- Examined distributions of credit amount and duration (right-skewed, long-tailed).  
- Identified imbalance in the risk variable.  
- Detected male-biased dataset, majority homeowners, and many applicants with low savings.  

### 2. **Missing Values Analysis**
- Investigated missingness in **Saving** and **Checking accounts**.  
- Found distributions to be similar between missing and non-missing → likely **MCAR** (Missing Completely at Random).  

### 3. **Normality & Variance Testing**
- Applied **Shapiro–Wilk** and **Levene’s** tests.  
- Found strong deviations from normality → justified use of **non-parametric tests**.  

### 4. **Hypothesis Testing**
- **Mann–Whitney U** for Credit Amount & Duration vs Risk → bad-risk borrowers request larger loans and longer durations.  
- **Kruskal–Wallis** for Credit Amount across Job, Housing, Age groups → significant differences for Job and Housing, not for Age.  
- **Chi-Square** for categorical predictors vs Risk → Checking and Saving accounts strongest, Housing and Age significant, Job/Purpose not significant.  
- **Cramér’s V** used to assess strength of associations.  

### 5. **Interaction Analysis**
- Built OLS model with log-transformed Credit Amount.  
- Tested interactions between Sex, Age group, and Housing.  
- Found weak/moderate evidence for Age×Housing interaction, others non-significant.  

### 6. **Key Conclusions**
- Credit Amount and Duration are **key risk predictors**.  
- Checking and Saving accounts are **strong categorical signals**.  
- Housing and Age matter, but weaker; Sex and Job are not practical predictors.  
- Risk interacts with Savings and Housing, leading to volatile borrowing patterns among bad-risk customers.  


## 📬 Contact
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/stefano-baglio/) or reach out via email: **s.baglio.personal@outlook.com**


## 🗂️ Folder Structure

```bash
📁 05-Credit-Risk-Analys-Statistical-and-Inferential-Insights
│
├── 📓 Credit-Risk-Analys-Statistical-and-Inferential-Insights.ipynb
├── 📄 README.md
└── 📁 Data

