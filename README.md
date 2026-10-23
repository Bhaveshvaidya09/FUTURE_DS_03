# Marketing Funnel & Conversion Analytics Command Center 📊

![Track Code](https://img.shields.io/badge/Track%20Code-DS%20%28Data%20Science%20%26%20Analytics%29-blue?style=for-the-badge)
![Task](https://img.shields.io/badge/Task-03%20%20Marketing%20Funnel%20Analytics-teal?style=for-the-badge)
![Repository Name](https://img.shields.io/badge/Repository-FUTURE__DS__03-darkgreen?style=for-the-badge)

---

## ❓ Problem Statement
In Direct-to-Consumer (D2C) e-commerce, acquiring user traffic without understanding multi-stage funnel drop-offs leads to severe ad spend inefficiency, high Customer Acquisition Costs (CAC), and unmitigated revenue leakage. Analyzing **120,000 user sessions** from the D2C Marketing Funnel dataset revealed major conversion bottlenecks:
* **Baseline Session-to-Purchase Conversion Rate:** **`6.82%`** (8,181 completed purchases out of 120,000 sessions).
* **Net Recognized Sales Revenue:** **`$17,016,599.15`** ($17.02 Million) across a 6-month period.
* **Unrecovered Gross Revenue Exposure:** **`$22.3 Million+`** locked in abandoned cart and checkout sessions.
* **Primary Drop-off Bottleneck:** **`65.13%`** of users who view products exit before adding items to their cart.

---

## 💡 Problem Solution
Engineered an end-to-end **Growth Analytics & Revenue Recovery Pipeline** across Python, SQL Server (SSMS), and Power BI:
1. **Automated ETL & Star Schema Engine:** Processed 120,000 raw session records using Python, derived 1/0 binary stage flags, calculated funnel depth levels, and structured a 5-table Star Schema database.
2. **Enterprise SQL Data Warehouse:** Modeled database `MarketingFunnelAnalytics` in SSMS with 5 master production views and 10 advanced T-SQL queries (CTEs, `DENSE_RANK()`, `LAG()`, `SUM OVER()`).
3. **Executive Command Center:** Developed an interactive Power BI dashboard featuring centralized DAX measures, dynamic slicers, and an operational **High-Intent Abandoned Session Watchlist**.

---

## 📌 Executive Summary & Financial Exposure
* **Total Sessions Tracked:** **`120,000 Sessions`**
* **Net Recognized Sales Revenue:** **`$17,016,599.15`** ($17.02 Million)
* **Overall Funnel Conversion Rate:** **`6.82%`**
* **Average Order Value (AOV):** **`$2,080.01 / purchase`**
* **High-Intent Cart Drop-off Rate:** **`65.13%`** (Product View $\rightarrow$ Cart Addition)

---

## 🖼️ Power BI Executive Dashboard Preview

![Executive Dashboard Preview](./dashboard.ss)

---

## 🛠️ Tech Stack & Usage

| Tool / Layer | Specific Implementation & Usage |
| :--- | :--- |
| 🐍 **Python** | Extracted raw session logs, standardized dates, derived 1/0 binary stage flags (`visited_website_flag` to `purchase_completed_flag`), derived funnel depth levels, and built 4 Dimension & 1 Fact Star Schema CSVs in `Data/Processed/`. Generated `chart_funnel_waterfall.png` & `chart_channel_performance.png`. |
| 🛢️ **SQL Server (SSMS)** | Modeled relational database `MarketingFunnelAnalytics` into a **Star Schema** (1 Fact, 4 Dimensions). Compiled 5 production master views (`vw_Funnel_Customer_360_Master`, `vw_Cart_Checkout_Dropoff_Watchlist`, etc.) and 10 T-SQL queries using CTEs, `DENSE_RANK()`, `LAG()`, and cumulative sums. |
| 📊 **Power BI** | Relational Star Schema data model with SSMS database views, 7 centralized **DAX measures** (`Total Traffic Volume`, `End-to-End Conversion Efficiency %`, `Net Recognized Sales Revenue`, `High-Intent Cart Abandonment Rate %`), 4 dynamic slicers, and interactive problem-solving charts. |

---

## 📈 Key Insights & Actionable Playbook

1. **Product Page Conversion Optimization (CRO):** 65.13% of product-interested users exit before adding items to cart.  
   *👉 Action:* Implement sticky "Add to Cart" CTAs, trust badges, customer reviews, and clear shipping timelines on mobile product pages.
2. **Automated Abandoned Cart & Checkout Email Recovery:** Target 18,975 abandoned sessions ($22.3M order value exposure).  
   *👉 Action:* Deploy an automated 3-part recovery email sequence (1 hr reminder, 24 hr social proof, 48 hr 5% discount code).
3. **High-ROI Channel Reallocation:** Email Marketing yields the highest conversion efficiency (**7.31%** vs 6.72% for Paid Ads).  
   *👉 Action:* Embed exit-intent lead capture popups offering 10% off to convert Paid Search traffic into owned email subscribers.
4. **Mobile Checkout Friction Reduction:** Mobile accounts for **70.0% of total traffic** (84,006 sessions) converting at ~6.78%.  
   *👉 Action:* Integrate Express Checkout wallets (Apple Pay, Google Pay, UPI, One-Click Pay) to eliminate mobile form-fill friction.

---

## 📁 Repository Structure
