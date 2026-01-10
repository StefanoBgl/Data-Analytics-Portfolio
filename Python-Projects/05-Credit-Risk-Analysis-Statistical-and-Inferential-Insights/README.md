# 💳 Credit-Risk-Analysis-Statistical-and-Inferential-Insights

This project investigates credit behavior across different client demographics using inferential statistics. We aim to identify whether variables such as gender, age, and employment type are associated with significant differences in credit default rates, loan amounts, and loan durations. By applying hypothesis testing and correlation analysis, we seek to uncover meaningful patterns in the data to support data-informed decisions in fair and responsible credit lending.

## 🗃️ Dataset Overview

The dataset includes records for 1,000 credit applicants with the following attributes:

- **Customer Demographics:** Age, Sex, Job (skill level), Housing (own/rent/free)
- **Financial Status:** Saving accounts, Checking account
- **Loan Details:** Credit amount, Duration (months), Purpose
- **Target Variable:** Risk (Good/Bad)

## 🛠 Libraries

- pandas
- numpy
- matplotlib
- seaborn
- scipy.stats (shapiro, mannwhitneyu, chi2_contingency, kruskal)
- statsmodels

## 📊 Insights & Results
    
- 📉 **Financial Drivers:** Duration and Credit Amount are significantly higher among bad-risk borrowers.  
- 🏦 **Strongest Predictors:** Checking and Saving account status show the strongest statistical associations with Risk among categorical variables.  
- 👤 **Demographic Trends:** Men tend to request higher credit amounts and longer durations than women.  
- 🏠 **Housing Factor:** Homeowners generally present a lower credit risk compared to those in "free" or rented housing.  
- ⚖️ **Statistical Validity:** Chi-square tests confirmed a significant association for Checking accounts ($p=0.0002$), while the "Purpose" of the loan was not statistically significant at the 5% level ($p=0.0579$).


## 🧱 Workflow Overview

### 1. **Data Preparation & Missingness**
- Analyzed missing data in **Saving accounts** and **Checking account**.
- Evaluated if data was missing at random by comparing demographic distributions between null and non-null groups.

### 2. **Descriptive Analysis**
- Conducted univariate analysis on numeric variables (Age, Credit Amount, Duration) to understand spread and outliers.
- Visualized categorical distributions to identify the most common loan purposes and job types.

### 3. **Inferential Statistics: Numeric Variables**
- **Normality Testing:** Performed Shapiro-Wilk tests, confirming that Age, Credit Amount, and Duration follow non-normal distributions.
- **Non-Parametric Comparisons:** Used Mann-Whitney U tests to prove that credit amounts and durations differ significantly between "Good" and "Bad" risk groups.

### 4. **Inferential Statistics: Categorical Variables**
- Executed **Chi-Square Tests of Independence** to determine which factors influence credit risk.
- Calculated **Cramér's V** to measure the strength of association, finding moderate effects for account status and housing.

### 5. **Demographic Deep Dives**
- **Gender Analysis:** Explored differences in credit requests between sexes using Kruskal-Wallis tests.
- **Job Analysis:** Identified how skill level impacts the total credit amount requested.

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.

## 🗂️ Folder Structure

```bash
📁 Credit-Risk-Analysis-Statistical-and-Inferential-Insights/
│
├── 📓 Credit Risk Analysis - Statistical and Inferential Insights.ipynb
├── 📄 README.md
└── 📁 Data
    └── 📄 german_credit_data.csv