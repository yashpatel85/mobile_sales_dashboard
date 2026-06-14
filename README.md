# 📱 Mobile Pulse: Comprehensive Smartphone Retail Analytics Dashboard

A dynamic, multi-page Power BI visualization tool built to explore mobile phone retail and e-commerce transactions across India. This report delivers high-level executive overviews, specialized month-to-date (MTD) tracking, and deep-dive Year-over-Year (YoY) comparative matrices.

---

## 📖 Project Overview & Purpose

The **Mobile Pulse Dashboard** is an interactive analytics tool designed to help sales executives, inventory managers, and commercial strategists track retail performance across a portfolio of premier smartphone brands. 

The application features a triple-focus layout:
1. **Executive Performance View:** Monitors brand equity, payment behaviors, customer satisfaction, and regional revenue distribution across major Indian metro hubs.
2. **Month-to-Date (MTD) Engine:** Evaluates run-rate growth velocity dynamically throughout the month to identify pace acceleration or flatlines.
3. **Year-over-Year (YoY) Comparison Suite:** Benchmarks current performance directly against historical *Same Period Last Year* (SPLY) baselines to isolate structural seasonality from single-year events.

This tool empowers decision-makers to transform raw retail ledger entries into strategic actions regarding localized inventory fulfillment, payment gateway optimization, and time-sensitive marketing campaigns.

---

## 🛠️ Tech Stack

The dashboard was engineered using the following tools and technologies:

* **📊 Power BI Desktop** – Core platform used for user interface canvas layouts, visual interactions, and report design.
* **📂 Power Query** – Extract, Transform, and Load (ETL) architecture applied to clean, merge, and organize raw point-of-sale logs.
* **🧠 DAX (Data Analysis Expressions)** – Advanced calculations utilized for complex time-intelligence metrics (`TOTALMTD`, `SAMEPERIODLASTYEAR`), dynamic variances, and stateful conditional sidebar toggles.
* **📝 Data Modeling** – Structured star-schema design connecting core transaction ledgers with specialized date-dimension tables and product-attribute catalogs to support fluid cross-filtering.
* **📁 File Format** – `.pbix` for system deployment and `.png` for repository asset previews.

---

## 🗃️ Data Source & Structure

* **Source:** https://github.com/SatishDhawale/Power_BI_Dashboard/blob/main/Mobile%20Sales%20Data.xlsx
* **Geographic Coverage:** Major commercial hubs in India (Delhi, Mumbai, Bengaluru, Chennai, Kolkata, Hyderabad, etc.).
* **Dataset Schema:** High-velocity transactional records capturing detailed information per sale, including:
  * Transaction timestamps & chronological markers.
  * Device hardware profiles (e.g., Apple iPhone SE, OnePlus Nord, Samsung Galaxy Note 20, Vivo, Xiaomi).
  * Financial metrics (`Total_Sales`, transaction counts, average device retail pricing).
  * Operational markers (customer satisfaction feedback ratings, payment gateways utilized).

---

## 🚀 Key Features & Highlights

### 🎯 Business Problem
The highly volatile nature of the consumer electronics landscape makes it difficult for retail leaders to track baseline growth alongside absolute sales volumes. While aggregate annual or monthly numbers provide visibility into past performance, they fail to reveal when sales momentum slows mid-month or falls behind historical trends. Without granular comparative monitoring across different time dimensions, management cannot identify shortfalls in time to launch mid-month promotional adjustments or address localized operational friction points.

### 🔍 Walkthrough of Dashboard Views

#### View 1: Executive Sales Overview (Page 1)
* **High-Level KPI Banner:** Tracks core health metrics at a glance, including **Total Sales ($769M)**, **Total Quantity Sold (19K)**, **Total Transactions (4K)**.
* **Geographic Revenue Heatmap:** Interactive bubble map tracking total revenue split across primary Indian commercial centers.
* **Monthly Volume Trajectory (Line Chart):** Illustrates month-over-month volume, pinpointing seasonal high points in March and July against lower-volume periods in February and September.
* **Brand Matrix (Table Visual):** High-density reporting matrix providing a performance breakdown across leading manufacturers.
* **Customer Feedback Funnel:** Segregates customer satisfaction responses into explicit buckets (**Good: 2,331**, **Average: 652**, and **Poor: 852**) to safeguard brand health.
* **Payment Allocation Wheel (Donut Chart):** Breaks down transactions across four major consumer payment profiles: **UPI (26.36%)**, **Credit Card (24.69%)**, **Debit Card (24.72%)**, and **Cash (24.22%)**.
* **Device Popularity Ranker (Horizontal Bar Chart):** Tracks revenue-driving hardware variants side-by-side.

#### View 2: Month-to-Date (MTD) Growth Engine (Page 2)
* **Contextual KPI Cards:** Automatically recalibrates to reflect selected month-specific performance snapshots (e.g., **August 2022** showing **$23M Total Sales**, **588 Units Sold**, and **110 Transactions**).
* **Time-Intelligence Sidebar Navigation:** Left-anchored interactive button panels that instantly alternate focus between full-scale dashboards, **Same Period Last Year** historical trend matches, or explicit monthly cutaways (January through December).
* **Hierarchical Time Slicer:** Top-right contextual filter accommodating rapid multi-level drill-downs by Year, Quarter, Month, and Day.
* **Cumulative MTD Growth Curve (Stepped Area/Line Visual):** A highly detailed, day-by-day cumulative timeline plotting revenue growth throughout the chosen month. This visual demonstrates steady revenue escalation from $0.5M on August 1st up to $23.1M by August 31st, helping teams track daily sales momentum.

#### View 3: Same Period Last Year / YoY Performance Analysis (Page 3)
* **Consolidated Metric Cards:** Recalibrated annual perspective displaying **$253M Total Sales**, **6K Units Sold**, and **1K Total Transactions** for the filtered year (2023).
* **Granular YoY Performance Matrix (Table Visual):** A highly detailed daily audit table tracking current `Total_Sales` side-by-side with `Same Period Last Year` historical values down to the exact day of the month (e.g., January 1st through 14th) to catch day-specific variances immediately.
* **Annual YoY Baseline Comparison (Clustered Column Chart):** Displays current-year performance alongside the prior year's baseline, giving executives an immediate sense of macro-level annual growth or contraction.
* **Quarterly Variance Tracking (Clustered Column Chart):** Segregates performance into fiscal quarters (Qtr 1 through Qtr 4) to monitor cyclical corporate growth and highlight which quarters exceeded or fell behind prior-year milestones.
* **Monthly YoY Seasonality Chart (Clustered Column Chart):** Breaks down growth metrics across all twelve calendar months, plotting current performance against historical trends to identify shifting seasonal patterns or campaign-driven revenue surges.

---

## 💡 Business Impact & Insights

* **Velocity Tracking:** The MTD accumulation curve allows regional managers to identify mid-month flatlines early, giving them a window to implement target promos before the month closes.
* **Year-over-Year Growth Diagnostics:** The SPLY dashboard reveals hidden seasonal shifts. For instance, if Qtr 1 sales lag behind the previous year while Qtr 2 sales outpace it, analysts can connect these variances back to product launch timelines or changing promotional windows.
* **Inventory Control & Reordering:** Operations teams can combine day-by-day performance gaps with current MTD unit sales volumes to proactively trigger restocking orders, ensuring high-demand inventory matches consumer purchasing trends.
* **Strategic Campaign Alignment:** Marketing managers can evaluate performance dips across specific months (e.g., February) on Page 1, then pivot to Page 3 to see if those dips are structural annual trends or isolated single-year events. This helps teams build better long-term promotional schedules.
* **Financial Gateway Partnerships:** Knowing that digital payment forms (UPI and Cards) capture over 75% of sales volume, IT infrastructure teams can monitor transaction pacing against payment channels to minimize checkout failures during high-velocity weeks.

---

## 🖼️ Dashboard Previews & Screenshots

### 1. Executive Performance Dashboard
![Executive Overview Screen](https://github.com/yashpatel85/mobile_sales_dashboard/blob/main/Dashboard%20Preview.png)  
*Figure 1: Main executive dashboard layout featuring high-level KPIs, multi-dimensional dropdown slicers, and regional sales distribution across India.*

### 2. Month-to-Date (MTD) Tracking
![MTD Growth View Screen](https://github.com/yashpatel85/mobile_sales_dashboard/blob/main/MTD%20Preview.png)  
*Figure 2: Dedicated Month-to-Date (MTD) trend interface tracking cumulative daily revenue velocity alongside focused seasonal time-intelligence filters.*

### 3. Same Period Last Year (YoY) Analysis
![SPLY YoY Performance Screen](https://github.com/yashpatel85/mobile_sales_dashboard/blob/main/Same%20Perioed%20Last%20%20Year%20Preview.png)  
*Figure 3: Same Period Last Year (SPLY) analysis interface providing deep-dive year-over-year operational comparisons at the annual, quarterly, and daily levels.*

---

## 🛠️ How to Use This Repository

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yashpatel85/mobile_sales_dashboard.git
   ```
2. **Open the Report:** 
   * Ensure you have the latest version of [Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494) installed.
   * Open the `.pbix` file located in the root directory.
3. **Explore Visuals:** Use the left-side navigation panel buttons to toggle between the **Dashboard view**, **MTD Report**, and **Same Period Last Year** pages. Filter by Brand, Model, or Date utilizing the slicers at the top of the canvas.
