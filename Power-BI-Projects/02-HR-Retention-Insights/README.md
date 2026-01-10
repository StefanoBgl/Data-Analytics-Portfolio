# 🧑‍💼 HR Retention & Workforce Analysis

The **HR Analysis Dashboard** is an interactive Power BI report designed to deliver strategic insights into workforce composition and employee retention. By leveraging employee-level data across demographics, departments, and job hierarchies, the dashboard supports HR professionals and decision-makers in identifying patterns and implementing data-informed talent strategies.

Built on detailed employee records—including demographics, salary, job information, and exit data—the report offers a comprehensive view of workforce dynamics across time and organizational dimensions.

[View Interactive dashboard](https://bit.ly/3BZjYHg)

## 📌 Key Focus Areas

- **Workforce Overview** — Gender, ethnicity, age, salary, department, and job hierarchy insights  
- **Retention Analysis** — Company-wide and segmented retention rates, demographic attrition patterns



<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/bec950e9-67f7-495a-862f-614df97e7e04" width="500" height="300"/></td>
    <td><img src="https://github.com/user-attachments/assets/3e54d10e-ba00-4445-a4e1-bc82a54a3e53" width="500" height="300"/></td>
    <td><img src="https://github.com/user-attachments/assets/afed7dc5-35ac-4002-9835-559e66cedfa9" width="500" height="300"/></td>
  </tr>
</table>

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

### 📊 Workforce Composition

- Waffle charts for gender, age, and ethnicity
- Lollipop chart for salary comparisons by unit, department, title, and level
- Bar charts for demographic breakdowns
- Workforce breakdown by gender for employees retained vs. left

### 📈 Retention Trends

- Year-over-year KPIs (Retention Rate, Turnover, Exits)
- Correlation analysis between salary and exits
- Time intelligence visuals (retention by year, quarter, month)


## 🧩 Data Model Overview

This report follows a star schema with a central fact table and connected dimension tables for scalable performance and flexible filtering.

### 🔸 Fact Table: `FACT_Employees`
- Full Name
- Hire Date
- Exit Date
- Annual Salary
- Bonus %
- Age
- Demographic identifiers

### 🔹 Dimension Tables
- `DIM_Department`: Department, Business Unit
- `DIM_Location`: Country, Region
- `DIM_JobTitle`: Job Title, Level
- `Calendar`: Date, Month, Year, Quarter

## 📦 Data Source

This is a synthetic dataset curated for educational and portfolio purposes. It does not contain any real or confidential employee data.

## 🧰 Tools & Technologies Used

- Power BI Desktop
- DAX
- Power Query (M)


## 🚀 How to Use

1. Clone this repository or download the ZIP file
2. Open the `.pbip` project in Power BI Desktop
3. Ensure the `Data/` folder is in the root directory for correct data linkage


## 📬 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/stefano-baglio/)
<br>
<a href="mailto:s.baglio.personal@outlook.com">
  <img src="https://img.shields.io/badge/Email-cccccc?style=for-the-badge&logo=gmail&logoColor=black" alt="Email" />
</a>

---

## 🗂️ Folder Structure

```bash
📁 02-HR-Retention-Insights/
│
├── 📄 README.md
├── 📁 pbip
├── 📁 Images
└── 📁 Data

