# 🧑‍💼 HR Retention & Workforce Analysis

The **HR Analysis Dashboard** is an interactive Power BI report designed to deliver strategic insights into workforce composition and employee retention. By leveraging employee-level data across demographics, departments, and job hierarchies, the dashboard supports HR professionals and decision-makers in identifying patterns and implementing data-informed talent strategies.

Built on detailed employee records—including demographics, salary, job information, and exit data—the report offers a comprehensive view of workforce dynamics across time and organizational dimensions.

## 📌 Key Focus Areas

- **Workforce Overview** — Gender, ethnicity, age, salary, department, and job hierarchy insights  
- **Retention Analysis** — Company-wide and segmented retention rates, demographic attrition patterns

---

## 🔎 Insights & Recommendations

### 1. Workforce Overview

- **Gender Distribution**: The company maintains a relatively balanced gender workforce.  
    > 💡 *Continue fostering inclusive policies to promote equity in leadership roles.*

- **Ethnic Representation**:
  
  - Asian employees are the most represented group, while Black employees are the least.  
  - The majority of the workforce is based in the U.S. branch.
  <br/>
  
  > 💡 *Strengthen mentorship and diversity initiatives for underrepresented groups.*

- **Age Distribution**: Over 80% of employees fall between 30 and 59 years old.  
  > 💡 *Recommendation:* Develop succession planning and early career programs to build a strong leadership pipeline.

- **Salary Distribution**:
  - Minimal salary variance across departments and business units.  
  - Notable disparities exist at the job title and level, with senior roles earning significantly more.
  <br/>
  
  > 💡 Conduct regular pay equity audits, especially across job titles, to ensure transparency and address potential disparities in career progression.


### 2. Retention Rate Analysis

- **Overall Retention Trends**:
  - Company-wide retention has been below 90% since 2013.  
  - However, annual retention rates are consistently high (e.g., 97.8% in 2021), due to differences in calculation methodology: the overall retention rate considers the average number of employees, which can fluctuate significantly across time frames.
  <br/>
  
  > 💡 *Clarify retention KPIs by distinguishing between long-term and annual trends.*

- **Salary and Retention Correlation**: Retention is negatively correlated with salary at the department level but positively correlated at job title and level.  
  > 💡 *Review compensation alignment between job responsibilities and retention objectives.*

- **Demographic Insights**: Higher turnover is observed among Black employees and staff located in the Asian branch.  
  > 💡 *Launch targeted retention programs such as ERGs, feedback initiatives, and cultural inclusion efforts.*


## 🛠️ Analytical Techniques & Visual Highlights

This dashboard employs interactive and high-impact visualizations to enable intuitive HR analysis:

### 📊 Workforce Composition

- **Workforce breakdown** by gender for working employees, employees left, average and median salary
- **Waffle charts** for gender, age, and ethnicity
- **Lollipop chart** for salary across business unit, department, job title and job level
- **Bar charts** for gender, age, and ethnicity


### 📈 Retention Trends

- **Year-over-year KPIs** (Retention Rate, Turnover, employees left)
- **Correlation between salary brackets and exit trends** by business unit, deparment, job level and job title
- **Time intelligence Retetion Rate** breakdown by year, quarter, month


## 🧩 Data Model Overview

The report uses a clean and optimized star schema, connecting a central fact table to supporting dimension tables for rich filtering and scalable performance. All relationships are one-to-many from dimensions to the fact table, forming a robust analytical model.

### 🔸 Fact Table: `FACT_Employees`
Contains employee records with demographic and employment details:
- Full name
- Hire date
- Exit date
- Annual salary
- Bonus %
- Age

### 🔹 Dimension Tables
- **`DIM_Department`**
- **`DIM_Location`**
- **`DIM_JobTitle`**
- **`Calendar`**

---

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.

---

## 🗂️ Folder Structure

```bash
📁 02-HR-Retention-Insights/
│
├── 📄 README.md
├── 📁 pbip
└── 📁 Data/

