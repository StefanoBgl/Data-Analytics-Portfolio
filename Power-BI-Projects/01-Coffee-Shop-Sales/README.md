# ☕ Coffee Shop Sales Dashboard

The **Coffee Shop Dashboard** is an interactive Power BI report that provides a comprehensive analysis of a coffee shop’s performance across time, stores, and product categories. Built on transaction data from a 6-month period in 2023, the report is designed to help stakeholders uncover patterns, optimize promotions, and make data-driven decisions.

[View Interactive dashboard](https://bit.ly/3Oih8Qe)

## 📌 Key Focus Areas
1. **General Overview** — Top-level KPIs and sales performance by month, store, and category  
2. **Customer Behaviour** — Patterns in buying time, transaction size, and underperforming product recovery

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/c40ff2c8-2345-4e68-b2e9-61270109664b" width="500" height="300"/></td>
    <td><img src="https://github.com/user-attachments/assets/aec86452-7bad-4687-90b5-0f66367cbf1f" width="500" height="300"/></td>
  </tr>
</table>

## 🔎 Insights & Recommendations

### 1. General Overview
- **Strongest months**: March, May, and June  
- **Weakest months**: January, February, and April  
  > 💡 *Consider targeted campaigns during low-performing months to boost sales (e.g. discounts, seasonal offers).*

- **Top-performing stores**: Astoria and Hell’s Kitchen  
  > 💡 *Maintain support and explore localized initiatives for even greater growth.*

- **Top-selling categories**: Coffee > Tea > Bakery  
  > 💡 *Experiment with seasonal items or bundle deals within these categories to drive revenue.*


### 2. Customer Behaviour
- **Sales peak before 10 AM**  
  > 💡 *Introduce afternoon specials or loyalty bonuses during off-peak hours.*

- **Some low-performing products improved in June**  
  > 💡 *Leverage this trend with limited-time offers or highlight them in combo deals.*

- **Positive correlation between price and transaction quantity**  
  > 💡 *Test dynamic pricing or bundle strategies to maximize sales volume and profit.*


## 🛠️ Analytical Techniques & Visual Highlights

### 📈 Time Series & Trend Analysis
- Sales, Quantity, and Transactions Trend
- Time Intelligence for Monthly Comparisons (% Change vs. Previous Month)
- Monthly Sales vs Average

### 📊 Category & Product Performance
- Product Category Sales vs Average
- Individual Product Performance
- Top 5 vs Bottom 5 Products (DAX-powered slicers)

### 🧠 Behavioral Insights
- Calendar-Based Sales View
- Heatmap of Day & Time
- Correlation Between Transaction Quantity and Unit Price

## 🧩 Data Model Overview

The report uses a clean and optimized **star schema**, connecting a central fact table to supporting dimension tables for rich filtering and scalable performance.

### 🔸 Fact Table: `FACT_Transaction`
- Sales transaction data: date, product ID, store ID, quantity, sales, unit price

### 🔹 Dimension Tables
- `DIM_Product`: Product ID, Name, Category
- `DIM_Store`: Store ID, Name, Location
- `Calendar`: Date, Month, Quarter, Year

## 📦 Data Source

This is a synthetic dataset curated for educational and portfolio purposes. It does not contain any real or confidential employee data.

## 🧰 Tools & Technologies Used

- Power BI Desktop
- DAX
- Power Query (M)

## 🚀 How to Use

1. Clone this repository or download the files
2. Open the `.pbip` project in Power BI Desktop
3. Ensure the `Data/` folder is in the same root directory

## 📬 Contact
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/stefano-baglio/)  
📧 Email: s.baglio.personal@outlook.com

---

## 🗂️ Folder Structure

```bash
📁 01-Coffee-Shop-Sales/
│
├── 📄 README.md
├── 📁 pbip
├── 📁 Images
└── 📁 Data

