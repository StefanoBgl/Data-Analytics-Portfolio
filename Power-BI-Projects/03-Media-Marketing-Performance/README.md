# 📣 Media Campaign Performance Dashboard

The **Media Campaign Dashboard** is an interactive Power BI report designed to evaluate the financial and operational performance of marketing campaigns across various platforms. It delivers actionable insights into key performance indicators (KPIs), highlights successes and inefficiencies, and supports data-driven marketing decisions through clear visual storytelling.

This project analyzes multi-channel campaign data over time, offering a comprehensive view of performance by campaign, platform, and time dimension.

[Interactive dashboard](https://bit.ly/media-campaign-dashboard-app)

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

### 💰 Financial Performance Analysis

- KPI Target Tracking: Evaluate financial KPIs against targets by month, campaign, and platform to assess goal achievement and budget impact
- **Campaign Profitability Overview**: Assess profitability metrics by campaign to support ROI analysis and budget allocation decisions

### 🚀  Operational Performance Analysis

- **Performance Trends**: Monitor **Click-Through Rate** (CTR), **Impression-to-Conversion Rate** (ICR), and **Conversion Rate** (CR) trends over time to track engagement and efficiency
- **Monthly Benchmarking**: Compare CTR, ICR, and CR against monthly averages to identify performance peaks and gaps
- **Pipeline Decomposition**: Break down the full conversion pipeline for CTR, ICR, and CR to understand stage-specific behavior
- **Funnel Analysis**: Visualize the complete journey from impression to conversion to evaluate overall campaign effectiveness
- **Heatmap by Campaign & Weekday**: Analyze CTR, ICR, and CR across campaigns and days of the week to uncover temporal performance patterns

## 🧩 Data Model Overview

The report uses a clean and optimized star schema, connecting a central fact table to supporting dimension tables for rich filtering and scalable performance. All relationships are one-to-many from dimensions to the fact table, forming a robust analytical model.

### 🔸 Fact Table: `Metrics`
Contains performance data of each campaign across time and platforms:

### 🔹 Dimension Tables
- Campaign
- Platform
- Calendar

---

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.

---

## 🗂️ Folder Structure

```bash
📁 03-Media-Marketing-Performance/
│
├── 📄 README.md
├── 📁 pbip
├── 📁 Images
└── 📁 Data
