# ☕ Coffee Shop Sales Dashboard

The **Coffee Shop Dashboard** is an interactive Power BI report that provides a comprehensive analysis of a coffee shop’s performance across time, stores, and product categories. Built on transaction data from a 6-month period in 2023, the report is designed to help stakeholders uncover patterns, optimize promotions, and make data-driven decisions.

## 📌 Key Focus Areas
1. **General Overview** — Top-level KPIs and sales performance by month, store, and category  
2. **Customer Behaviour** — Patterns in buying time, transaction size, and underperforming product recovery
   
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/9931d245-d98a-493b-982a-76e4b53067eb" width="500" height="300"/></td>
    <td><img src="https://github.com/user-attachments/assets/f5777bd4-d9d4-4ab3-992f-e0cf736d5465" width="500" height="300"/></td>
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

The report employs a variety of interactive and visually engaging techniques to uncover patterns and drive insights:

### 📈 Time Series & Trend Analysis
- **Sales, Quantity, and Transactions Trend**: Line charts display performance progression over time.  
- **Time Intelligence for Monthly Comparisons**: Measures like % Sales Change allow comparison with the previous month.  
- **Monthly Sales vs Average**: Bar charts highlight seasonal peaks and drops against the average.

### 📊 Category & Product Performance
- **Product Category Sales vs Average**: Highlights over- or under-performing categories.  
- **Individual Product Performance**: Identifies rising or declining products.  
- **Top 5 vs Bottom 5 Products**: DAX-powered slicers allow segmented views.

### 🧠 Behavioral Insights
- **Calendar-Based Sales View**: Visualizes daily sales patterns.  
- **Heatmap of Day & Time**: Reveals peak hours across weekdays.  
- **Correlation Between Transaction Quantity and Unit Price**: Explores pricing impact on customer behavior.

## 🧩 Data Model Overview

The report uses a clean and optimized **star schema**, connecting a central fact table to supporting dimension tables for rich filtering and scalable performance. All relationships are one-to-many from dimensions to the fact table, forming a robust analytical model.

### 🔸 Fact Table: `FACT_Transaction`
Contains all sales transaction data:
- Date of purchase  
- Product & store references  
- Sales, quantity, and unit price  

### 🔹 Dimension Tables
- **`DIM_Product`**
- **`DIM_Store`**
- **`Calendar`**
  
---

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.

---

## 🗂️ Folder Structure

```bash
📁 01-Coffee-Shop-Sales/
│
├── 📄 README.md
├── 📁 pbip
├── 📁 Images
└── 📁 Data

