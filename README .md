# 📊 Superstore Sales Performance Dashboard
### Interactive Power BI Dashboard | Retail Analytics | 2014 - 2017

---

## 🔍 Project Overview

This project is an end-to-end **Sales Performance Dashboard** built with **Power BI**, analyzing the Superstore retail dataset covering **4 years of sales data (2014–2017)** across the United States.

The dashboard transforms raw retail data into **actionable business insights** to help management make data-driven decisions across sales, profitability, logistics, and customer behavior.

---

## 📁 Dashboard Pages

| Page | Description |
|------|-------------|
| **1. Overview** | KPI Cards, Sales Trend, Regional Performance |
| **2. Product & Region** | Top Products, Profit by Category, Discount Impact, Shipping Analysis |
| **3. Customer** | Segment Analysis, Top 10 Customers, Orders Trend |
| **4. Key Insights** | Findings, Root Causes & Recommendations |

---

## 💡 Key Findings & Recommendations

| # | Finding | Cause | Recommendation |
|---|---------|-------|----------------|
| 1 | Sales grew **46.9% YoY** but Profit Margin only moved **+0.11%** | Excessive discounting | Cap discounts at 20% to protect margins |
| 2 | **Furniture** has the lowest profit margin despite decent sales | High discounts on Furniture | Reduce Furniture discounts or reprice |
| 3 | **Central region** is the slowest in delivery at **4.04 days** | Limited logistics coverage | Add local warehouse or partner with regional carrier |
| 4 | **Consumer segment** = **50.5%** of total revenue | High dependency on one segment | Build loyalty program & grow Corporate segment |
| 5 | **Top 10 customers** drive significant revenue concentration | Limited customer diversification | Launch VIP retention program |
| 6 | Avg Shipping = **3.96 days** — strong operational performance | — | Maintain & focus on improving Central region |

---

## 📊 KPIs Tracked

- 💰 **Total Sales** — $2.30M
- 📈 **Total Profit** — $286.40K
- 🛒 **Total Orders** — 9.99K
- 📊 **Profit Margin %** — 12.47%
- 🧾 **Average Order Value** — $229.86
- 🚚 **Avg Shipping Days** — 3.96 Days

---

## 🛠️ Tools & Techniques

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Dashboard development & visualization |
| **DAX** | KPI calculations, YoY comparisons, Arrow indicators |
| **Power Query** | Data cleaning & transformation |
| **Data Modeling** | Relationships & calculated columns |

---

## ⚙️ DAX Measures Used

```DAX
-- Total Sales
Total Sales = SUM('Orders'[Sales])

-- Profit Margin %
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

-- Year over Year Comparison
Sales LY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Orders'[Order Date]))

-- Growth %
Growth % = DIVIDE([Total Sales] - [Sales LY], [Sales LY], 0)

-- Average Shipping Days
Avg Shipping Days = AVERAGEX('Orders', DATEDIFF('Orders'[Order Date], 'Orders'[Ship Date], DAY))
```

---

## 📂 Dataset

- **Source:** Superstore Dataset (Kaggle)
- **Records:** 9,994 orders
- **Period:** 2014 – 2017
- **Geography:** United States (4 Regions, 49 States)
- **Categories:** Technology, Office Supplies, Furniture

---

## 🖼️ Dashboard Screenshots

### Page 1 — Overview
![Overview](screenshots/page1_overview.png)

### Page 2 — Product & Region
![Product & Region](screenshots/page2_product_region.png)

### Page 3 — Customer
![Customer](screenshots/page3_customer.png)

### Page 4 — Key Insights
![Key Insights](screenshots/page4_insights.png)

---

## 🚀 How to Use

1. Download the `.pbix` file
2. Open with **Power BI Desktop**
3. Use the **Slicers** to filter by Year, Region, and Segment
4. Navigate between pages using the **icon buttons** at the top
5. Hover over charts for **detailed tooltips**

---

## 👤 Author

**Ahmed Hesham**
📧 ahmed.hesham.data@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/ahmed-hesham-data)
🐙 [GitHub](https://github.com/ahmed-hesham-data)

---

## 🔗 Related Projects

- [SQL Sales Analysis](https://github.com/ahmed-hesham-data/Superstore-SQL-Analysis) — Same dataset analyzed with SQL
- [Excel Sales Dashboard](https://github.com/ahmed-hesham-data/excel-sales-dashboard-analysis) — End-to-end Excel analysis

---

*This project is part of my Data Analytics Portfolio — built to demonstrate real-world business analysis skills using Power BI.*
