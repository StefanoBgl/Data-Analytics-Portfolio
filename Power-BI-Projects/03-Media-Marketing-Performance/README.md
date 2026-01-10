# 📣 Media Campaign Performance Dashboard

The **Media Campaign Dashboard** is an interactive Power BI report designed to evaluate the financial and operational performance of marketing campaigns across various platforms. It delivers actionable insights into key performance indicators (KPIs), highlights successes and inefficiencies, and supports data-driven marketing decisions through clear visual storytelling.

This project analyzes multi-channel campaign data over time, offering a comprehensive view of performance by campaign, platform, and time dimension.

[View Interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiYmE0NjJlYWUtYzQ1Yy00YjRlLWIwMjYtMDExMzY5MTQxMDVmIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

## 📌 Key Focus Areas

- **Financial Results** — Monthly trends, campaign outcomes, and platform effectiveness  
- **Performance** — Conversion funnels, CTR/ICR/CR trends, and granular weekday analysis

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/1e7bf28d-c591-4a5d-bfb6-21af456b0a50" width="500" height="300"/></td>
    <td><img src="https://github.com/user-attachments/assets/2ec8ff35-5616-4519-9695-4266988aafcf" width="500" height="300"/></td>
  </tr>
</table>

---

## 🔎 Insights & Recommendations

### 1. Financial Results

#### 📆 Last Month's Performance

- All KPIs reached their **highest values** in the most recent month.
- **Campaigns:** Only 3 of 7 met targets, *New Arrivals*, *Trending Now*, and *Must-Haves*, while
  *Flash Sale*, *Best Sellers*, and *Limited Edition* underperformed.
- **Platforms:** *Google Ads*, *LinkedIn*, and *Instagram* led performance, while *Facebook* and *Website* fell short.

> 💡 *Conduct post-campaign analyses for underperforming efforts and test new formats on low-performing platforms.*

#### 📊 Past Performance Trends

- Most months hit monthly goals, except **March 2024** and **December 2023**, which marked performance lows.
- **Top Months:** January and February 2024, with minimal campaign-level misses.
- Platforms like *Website* and *Twitter* consistently failed to meet performance benchmarks.
- Financial performance has been inconsistent, with volatility across months and marketing channels.

> 💡 *Prepare contingency strategies for historically weak months and reevaluate the ROI of low-performing platforms.*

> 💡 *Develop predictive benchmarks and implement A/B testing to reduce volatility and stabilize performance.*


### 2. Operational Performance

#### 📈 Trend Performance

- The **Click-Through-Rate (CTR)** has improved overall, despite initial dips and some fluctuations.
- Both **Impression-to-Conversion Rate (ICR)** and **Conversion Rate (CR)** show upward trends with minor monthly irregularities.

> 💡 *Continue current optimizations and reduce fluctuations through better segmentation and creative testing.*

#### ⏬ Funnel Analysis

- In the last month, **3.3% of impressions** converted.
- Monthly conversion rates remained stable, without major changes across months.

> 💡 *Optimize top-of-funnel efforts like targeting and audience reach to lift total conversions.*

#### 📊 Platform & Campaign Breakdown

- **Instagram** delivered the most efficient conversion funnel (via *Limited Edition*, *New Arrivals*, *Flash Sale*).
- **Google Ads** had the weakest conversion pipeline (*Exclusive Offers*, *Trending Now*, *Best Sellers*).

> 💡 *Scale successful Instagram campaigns and pause or rework inefficient Google Ads strategies.*

#### 📉 Overall Performance vs. Monthly Average

- Impressions, clicks, and conversions exceeded the monthly average only **in December 2023 and January 2024**.

> 💡 *Identify drivers of peak months (e.g., seasonality, promotions) and replicate those strategies.*

#### 📅 Weekday Effectiveness

**Conversion Rate (CR)**:
- Best Sellers → **Monday**
- Limited Edition → **Wednesday**
- New Arrivals → **Tuesday**

**Click-Through Rate (CTR)**:
- Top campaigns: *Limited Edition*, *Exclusive Offers*, *Must-Haves*
- No clear weekday trends

**ICR (Impression-to-Conversion Rate)**:
- Best performance for *Limited Edition* on **Wednesday**, **Tuesday**, and **Saturday**

💡 *Plan campaign pushes around high-performing weekdays to maximize effectiveness.*


## 🛠️ Analytical Techniques & Visual Highlights

### 💰 Financial Performance

- KPI Target Tracking by month, campaign, and platform
- Campaign-level ROI & profitability metrics

### 🚀 Operational Performance

- CTR, ICR, and CR trend analysis
- Monthly benchmarking against averages
- Funnel performance breakdown (from impression to conversion)
- Heatmaps by campaign and weekday for temporal analysis

## 🧩 Data Model Overview

The report is structured using a star schema for optimized performance and flexible filtering.

### 🔸 Fact Table: `Metrics`
- Campaign ID, Platform ID, Date
- Impressions, Clicks, Conversions, CTR, ICR, CR
- Costs, Revenue, Profit

### 🔹 Dimension Tables
- `DIM_Campaign`: Campaign name, type, status
- `DIM_Platform`: Platform name, channel category
- `Calendar`: Date, Month, Quarter, Year

## 📦 Data Source

This is a synthetic dataset curated for marketing analytics demonstration and learning purposes. It does not reflect real campaign performance.

## 🧰 Tools & Technologies Used

- Power BI Desktop
- DAX
- Power Query (M)

## 🚀 How to Use

1. Download or clone this repository
2. Open the `.pbip` project using Power BI Desktop
3. Ensure the `/Data` folder with the Excel file is in the root directory

## 📬 Contact


[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/stefano-baglio/)
<br>
<a href="mailto:s.baglio.personal@outlook.com">
  <img src="https://img.shields.io/badge/Email-cccccc?style=for-the-badge&logo=gmail&logoColor=black" alt="Email" />
</a>

---

## 🗂️ Folder Structure

```bash
📁 03-Media-Marketing-Performance/
│
├── 📄 README.md
├── 📁 pbip
├── 📁 Images
└── 📁 Data
