# 🛍️  Understanding Customer Behaviour in Supermarket Sales

This project analyzes a supermarket sales dataset to uncover **customer behavior patterns**, **product performance**, and **strategic business insights**. The goal is to explore how customers interact with the store, what drives sales, and how customer profiles differ based on time, location, and purchasing habits.

The notebook combines **exploratory data analysis (EDA)** with **clustering techniques** to segment customers and guide data-driven decisions.

<div style="display: flex; align-items: center; gap: 10px;">
  <img src="image1_url" width="300"/>
  <img src="image2_url" width="300"/>
</div>



## 🛠️ Workflow Overview

### 1. Data Cleaning & Preparation
- Parsed date and time columns, extracting new features like:
  - Day of the week
  - Hour of transaction
  - Total price per invoice
- Verified data quality
- Encoded categorical variables (e.g., gender, city, payment method) for modeling



### 2. Exploratory Data Analysis (EDA)

#### 🏙️ City & Branch Performance
- Compared revenue across **Mandalay**, **Naypyitaw**, and **Yangon**
- Identified which cities and branches generated the most revenue and sales

#### 👥 Customer Type & Spending
- Found that **members consistently spend more** than normal customers
- Membership is associated with higher average and total purchase amounts

#### 🧴 Product Line Insights
- Ranked product categories by:
  - Total sales
  - Unit price
  - Purchase frequency
- Top-performing lines include **Food & Beverages** and **Health & Beauty**

#### 🕒 Time-Based Patterns
- Sales peak during **midday** and on **weekends**
- Shopping activity varies by hour and weekday, with actionable marketing implications

#### 💳 Payment Preferences
- Analyzed usage of **Cash**, **Ewallet**, and **Credit Card**
- Ewallet users tend to make larger purchases, suggesting potential for tech-based promotions


### 3. Customer Segmentation (Clustering)

Used **K-Means clustering** to group customers based on:
- Total purchase value
- Preferred product line
- Shopping time
- Gender and customer type

#### Result: 3 Segments Identified
1. **Frequent, Low-Spending Customers** – Mostly normal type, visit during weekdays
2. **High-Spending Members** – Loyal and valuable, often shop on weekends
3. **Mid-Range Customers** – Diverse behavior, opportunity for conversion into loyal members

Clusters can be leveraged to guide **targeted promotions and business strategies**.



## 📈 Key Insights

- **Members in Naypyitaw** generate the highest revenue per visit
- **Weekend afternoons** are the busiest hours – ideal for flash sales
- **Ewallet users** spend more on average – may represent younger or more digital-savvy customers
- Clustering reveals **clear behavioral groups** that can support customized offers, product placement, and loyalty programs



## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.


## 🗂️ Folder Structure

```bash
📁 supermarket-sales-analysis/
│
├── 📓 Understanding_Customer_Behavior_through_Sales_Data.ipynb
├── 📄 README.md
└── 📁 Data/

