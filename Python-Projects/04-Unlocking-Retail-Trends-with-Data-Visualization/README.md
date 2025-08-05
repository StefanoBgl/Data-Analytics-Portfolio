# 🛒📈 Unlocking Retail Trends with Data Visualization

This project explores the **Global Superstore** dataset to uncover hidden patterns and strategic insights through data visualization. The objective is to analyze performance across sales, profitability, customer segments, and logistics to inform data-driven decisions in retail operations.

<!-- Row 1: 1st and 4th images side by side -->
<p align="center">
  <img src="https://github.com/user-attachments/assets/1cc85826-783b-465c-975e-a0f1f019a0bb" width="550"/>
  <img src="https://github.com/user-attachments/assets/600a69ee-9a01-4973-8687-ac92e3985030" width="350"/>
</p>

<!-- Row 2: 2nd image full width -->
<p align="center">
  <img src="https://github.com/user-attachments/assets/ecbba33a-bccc-4baf-9fcc-8558c0bcda29" />
</p>

<!-- Row 3: 3rd image full width -->
<p align="center">
  <img src="https://github.com/user-attachments/assets/3f0f6155-81e7-4cd4-bde8-1a16a3b38d02"/>
</p>


## 🗃️ Dataset Overview

The dataset includes detailed records of customer orders with the following attributes:

- **Order Details:** Order ID, Order Date, Ship Date, Ship Mode, Order Priority  
- **Customer Information:** Customer ID, Segment, City, State, Country, Market, Region  
- **Product Details:** Product ID, Category, Sub-Category, Product Name  
- **Performance Metrics:** Sales, Quantity, Discount, Profit, Shipping Cost

Each row represents an item within an order.

## 🛠 Libraries

- pandas
- numpy
- matplotlib
- seaborn
- plotly

## 📊 Insights & Results
    
    📉 Sales are growing, but profit margins remain flat, pointing to pricing or cost inefficiencies.  
    🕐 Standard shipping dominates, yet fulfillment slows with higher priority, highlighting logistical issues.  
    🌍 North America, APAC, and EU lead in volume, while EMEA and Canada show underutilized potential.  
    🪑  Phones and Chairs are profitable, while Tables contain several loss-making products.  
    💸 Some discounts hurt margins, suggesting the need to refine pricing strategies.    
    ⚠️ High-priority orders aren’t consistently faster, revealing service-priority misalignment.


## 🧱 Workflow Overview

### 1. **Feature Engineering**
- Created new metrics such as **Fulfillment Time** and **Profit Margin** to support performance and time-based analyses.

### 2. **Profit Margin Analysis**
- Visualized sales, profit, and profit margin over time.
- While sales increase steadily, profit margins remain stagnant.
- Losses occurred only in January and June 2011 on average.
- Profit margins were lowest in 2011 Q2 and 2012 Q1 and highest in 2013 Q3 and 2014 Q4.

  
### 3. **Distribution of Metrics**
- Analyzed distributions of **Sales**, **Profit**, **Discount**, **Quantity**, and **Shipping Cost**.
- Most orders are low-value and inexpensive to ship.
- Profit values are centered around zero, suggesting room for pricing or cost optimization.

### 4. **Customer & Geographic Analysis**
- Segmented sales by **Segment**, **Market**, **Country**, and **City**.
- Found concentration in specific markets like the US, France, and Australia.
- Regions such as **EMEA** and **Canada** show high customer count but lower engagement, highlighting areas for targeted growth.

### 5. **Ship Mode & Order Priority**
- Standard Class is the dominant ship mode, while Same Day shipping is underused.
- Fulfillment time unexpectedly increases with order priority.
- Critical and High priority orders are not always processed faster than Medium ones.

### 6. **Sub-Category Profitability**
- Technology and Office Supplies lead in both sales and profit.
- The **Tables** sub-category contains several unprofitable products.
- The 10 worst-performing products by cumulative losses were identified.

### 7. **Cost-Discount Analysis**
- Examine Sales and Profit against Discount and Shipping Cost to spot inefficiencies.
- Aggressive discounting hurts profitability in **Tables** sub-category.
- Advised a review of discount strategies, especially for underperforming products.

### 8. **Shipping Performance Analysis**
- Average order-to-ship time is around 4 days, with variability between 2 and 6 days.
- No strong seasonality in shipping performance.
- Canada shows higher fulfillment variability.
- Recommended segmentation of fulfillment data to identify delay drivers, and clearer communication of realistic delivery expectations.

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.


## 🗂️ Folder Structure

```bash
📁 04-Unlocking-Retail-Trends-with-Data-Visualization/
│
├── 📓 Unlocking-Retail-Trends-with-Data-Visualization.ipynb
├── 📄 README.md
└── 📁 Data
