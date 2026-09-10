# 📊 SuperStore Sales Dashboard | Power BI

> An interactive **Power BI dashboard** analyzing **SuperStore sales data (2019–2020)** — covering revenue, profit, order volume, customer segments, product categories, regional performance, and payment behavior. Built using **Power Query**, **DAX**, and a **star-schema data model** to transform 9,994 retail transactions into actionable business insights, including a **15-day sales forecast**.

---

<p align="center">
  <img src="Images/SuperStore%20Sales%20Dashboard%20Banner.png" width="100%">
</p>

---

# 📌 Project Overview

Retail businesses generate thousands of transactions every day — orders, shipments, returns, payments, and profits across dozens of product lines and regions. Converting this raw data into strategic insight is what separates stores that grow from those that stagnate.

This project presents an **interactive Power BI dashboard** built on **two years of SuperStore sales data (2019–2020)**. It provides a comprehensive view of sales performance, profitability, customer segments, product hierarchy, geographical distribution, and payment preferences — all explorable through dynamic slicers and DAX-driven calculations. A built-in **15-day sales forecast** helps anticipate short-term demand.

---

# 🎯 Project Objectives

- Analyze overall sales, profit, and order performance
- Track monthly sales and profit trends across 2019–2020
- Compare sales by product category and sub-category
- Evaluate performance by customer segment
- Identify top-performing regions and states
- Analyze payment mode preferences
- Examine shipping mode distribution and shipping efficiency
- Build a 15-day sales forecast for short-term planning
- Enable dynamic filtering using Year, Region, Category, and Segment slicers

---

# 📊 Dashboard Preview

<p align="center">
  <img src="Images/Screenshot%20Dashboard%20Light.png" alt="SuperStore Sales Dashboard – Main View" width="100%">
</p>

<p align="center">
  <img src="Images/Screenshot%20Dashboard%20Forecast.png" alt="SuperStore Sales Forecast – 15 Days" width="100%">
</p>

---

# 📁 Dataset Information

The dataset contains **order-level retail transaction records** across **2019–2020**.

Each record includes:

- Row ID
- Order ID
- Order Date
- Ship Date
- Ship Mode
- Customer ID
- Customer Name
- Segment
- Country
- City
- State
- Region
- Product ID
- Category
- Sub-Category
- Product Name
- Sales
- Quantity
- Profit
- Returns
- Payment Mode

**Total Records Analyzed:** 9,994
**Total Sales Analyzed:** $1.57M
**Total Profit Analyzed:** $175.26K
**Total Orders:** 22K
**Average Ship Days:** 4

---

# 🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- Power Query (Data Cleaning & Transformation)
- DAX (Calculated Measures & KPIs)
- Star-Schema Data Modeling
- Bing Maps (Geographic Visualization)
- Interactive Slicers & Cross-Filtering Visuals
- Built-in Forecasting (Analytics Pane)

---

# 📐 Data Modeling

The project follows a **star-schema style data model** where a consolidated sales fact table is connected with supporting dimension tables.

Main tables include:

- **SuperStore Sales** (Fact table — combined 2019–2020 data)
- **Date Table** (Custom calendar for time intelligence)
- **Region / State / City** (Geographic dimensions)
- **Product Hierarchy** (Category → Sub-Category → Product)
- **Customer Segments** (Consumer, Corporate, Home Office)

A custom **Date Table** was created to support month-over-month and year-over-year analysis, enabling accurate time-based slicers and forecasting.

---

# ⚙️ DAX Measures

Several custom DAX measures were created to support dynamic KPIs and visualizations.

### Financial Measures

- Total Sales
- Total Profit
- Total Orders
- Average Ship Days
- Profit Margin %

### Analytical Measures

- Sales by Category Contribution %
- Sales by Sub-Category Contribution %
- Sales by Region Share
- Sales by Segment Share
- Sales by Payment Mode Share
- Sales by Ship Mode Share
- Sales Forecast (15 Days)

### Time Intelligence Measures

- Sales MTD / YTD
- Profit MTD / YTD
- Prior Year Sales
- Year-over-Year Growth %

Key functions used:

- `SUM()`
- `SUMX()`
- `DIVIDE()`
- `CALCULATE()`
- `FILTER()`
- `ALL()`
- `SELECTEDVALUE()`
- `TOTALYTD()`
- `SAMEPERIODLASTYEAR()`

---

# 📈 Dashboard Features

### Executive KPI Cards

- Total Sales — **$1.57M**
- Total Profit — **$175.26K**
- Total Orders — **22K**
- Average Ship Days — **4**

---

### Interactive Visualizations

- Sales by Payment Mode (Donut Chart)
- Sales by Region (Donut Chart)
- Sales by Segment (Donut Chart)
- Sales by Month (Line/Area Chart — 2019 vs 2020)
- Profit by Month (Line/Area Chart — 2019 vs 2020)
- Sales by Ship Mode (Bar Chart)
- Sales by Category (Bar Chart)
- Sales by Sub-Category (Bar Chart)
- Sales by State (Geographic Map)
- Sales Forecast – 15 Days (Forecast Line Chart)
- Top 10 States by Sales (Horizontal Bar Chart)

---

# 💡 Key Business Insights

### 💰 Financial Performance

- Generated **$1.57M** in total sales and **$175.26K** in profit across the period.
- Peak sales occurred in **November and December**, indicating strong seasonal demand.
- Highest profit was recorded in **December**, confirming a profitable Q4 trend.

---

### 🗂️ Category Analysis

- **Office Supplies** contributed the highest sales (**$0.64M**).
- **Technology** followed with **$0.47M**.
- **Furniture** contributed **$0.45M**.

---

### 📦 Sub-Category Analysis

- **Phones** led sub-category sales at **$0.20M**.
- **Chairs** followed at **$0.18M**.
- **Binders** ranked third at **$0.17M**.
- **Storage** contributed **$0.15M**.

---

### 🚚 Shipping Analysis

- **Standard Class** dominated shipping with **$0.91M** in sales.
- **Second Class** — **$0.31M**
- **First Class** — **$0.24M**
- **Same Day** — **$0.10M**

---

### 👥 Customer Segment Analysis

- **Consumer** segment: **48%** of total sales
- **Corporate** segment: **33%**
- **Home Office** segment: **19%**

---

### 🌍 Regional Analysis

- **West** region: **33%** of total sales
- **East** region: **29%**
- **South** region: **22%**
- **Central** region: **16%**

---

### 🗺️ Geographic Analysis

- **California** is the top-performing state with **$0.34M** in sales.
- **New York** followed with **$0.19M**.
- **Texas** contributed **$0.12M**.
- Other notable states: Washington, Pennsylvania, Ohio, Illinois, Florida, Michigan, North Carolina.

---

### 💳 Payment Mode Analysis

- **Cash on Delivery (COD)** — **43%**
- **Online** — **35%**
- **Cards** — **22%**

---

### 📅 Sales Forecast

- A **15-day rolling forecast** projects short-term sales based on historical patterns, showing expected demand continuation into January 2021.

---

# 🎯 Strategic Insights

- **Q4 seasonality** is a major driver of annual revenue — inventory and staffing should be scaled accordingly.
- **Office Supplies** dominate volume, but **Technology** likely offers higher margins — a balanced portfolio strategy is recommended.
- **COD dominance (43%)** suggests an opportunity to incentivize digital payments for faster cash flow.
- **California and New York** alone contribute ~34% of sales — geographic diversification could reduce risk.
- **Same Day shipping** is underutilized (10%) — a potential upsell opportunity for premium customers.

---

# 🎨 Dashboard Highlights

- Professional Dark Navy UI Theme
- Custom SuperStore Banner
- Interactive Year, Region, Category & Segment Slicers
- Dynamic KPI Cards
- Cross-Filtering Visuals
- Geographic Map Visualization
- Built-in Forecasting
- Clean Executive Dashboard Design

---

# 🚀 Skills Demonstrated

- Data Cleaning & Transformation
- Star-Schema Data Modeling
- Advanced DAX Programming
- Time Intelligence Calculations
- KPI Development
- Retail & Sales Analytics
- Forecasting
- Geographic Analytics
- Dashboard Design
- Interactive Reporting
- Business Intelligence

---

# 📂 Repository Structure

```
SuperStore-Sales-Dashboard-PowerBI/
│
├── Dashboard/
│   └── SuperStore Sales Dashboard.pbix
│
├── Dataset/
│   └── SuperStore_Sales_Dataset.csv
│
├── Images/
│   ├── SuperStore Sales Dashboard Banner.png
│   ├── Screenshot Dashboard Light.png
│   └── Screenshot Dashboard Forecast.png
│
├── Documents/
│   ├── Dashboard Requirements.pdf
│   ├── Dashboard Summary.pdf
│   └── DAX & KPI's.pdf
│
└── README.md
```

---

# 🌟 Project Highlights

✔ Interactive SuperStore Sales Dashboard
✔ Advanced DAX & Time Intelligence
✔ Dynamic KPI Cards
✔ Sales & Profit Trend Analysis
✔ Category & Sub-Category Breakdown
✔ Geographic Sales Mapping
✔ Payment & Shipping Mode Analytics
✔ 15-Day Sales Forecast
✔ Responsive Dashboard Design

---

# 📚 Key Learnings

Throughout this project, I strengthened my skills in:

- Building efficient **star-schema data models**
- Writing reusable **DAX measures for KPIs and time intelligence**
- Designing **interactive retail dashboards**
- Developing **sales and profit forecasting** using Power BI's analytics pane
- Applying **business intelligence concepts** to retail sales data
- Using **geographic mapping** for regional performance analysis

---

# ✅ Conclusion

This project demonstrates how **Power BI** can transform two years of raw retail transaction data into meaningful business insights through interactive dashboards and advanced DAX. By combining sales KPIs, profit trends, category performance, customer segmentation, geographic analysis, and short-term forecasting, the dashboard provides a **centralized analytical view of SuperStore operations**, supporting faster decision-making for retail managers, analysts, and business stakeholders.

---

## 👨‍💻 Author

**Sabbir Uddin Akash**

- 💼 Aspiring Data Analyst
- 📊 Power BI | SQL | Excel | Python
- 🌐 Portfolio: [Sabbir Uddin Akash](https://sabbirakash.github.io)
- 💻 GitHub: [sabbirakash](https://github.com/sabbirakash)
- 🔗 LinkedIn: [Sabbir Uddin Akash](https://www.linkedin.com/in/sabbirakash)

If you found this project useful, consider giving it a ⭐.

---

## 📌 GitHub Repository Description

> Interactive Power BI dashboard analyzing 2 years of SuperStore sales data — covering revenue, profit, categories, regions, customer segments, and a 15-day sales forecast using DAX, Power Query & star-schema modeling.

---

## 🏷️ GitHub Topics

```
powerbi
power-bi-dashboard
data-analytics
dax
power-query
business-intelligence
sales-dashboard
retail-analytics
data-visualization
superstore-dataset
sales-forecast
star-schema
portfolio-project
data-analyst
dashboard-design
```
