# 📊 Dynamic Retail Dashboard in Excel

## Overview
The **Dynamic Retail Dashboard** is an interactive and data-driven tool built in Excel to visualize and analyze retail data. It connects to datasets hosted on GitHub, uses Power Query for data transformation, and presents insights through dynamic charts and KPIs. The dashboard solves key business questions, enabling informed decision-making.

---

## 📁 Datasets Used

### 1. Orders Table

Contains details of customer orders, including product, shipping, and financial metrics.

**Sample Data:**

| Order ID       | Returned | Order Date   | Ship Date   | Ship Mode     | Customer Name | Segment   | Country       | Market | Sales   | Profit  | Discount |
|----------------|----------|--------------|-------------|----------------|----------------|-----------|----------------|--------|---------|---------|----------|
| CA-2012-124891 | No       | 31-07-2020   | 31-07-2020  | Same Day      | Rick Hansen    | Consumer  | United States | US     | 2309.65 | 762.18  | 0        |
| IN-2013-77878  | Yes      | 05-02-2021   | 07-02-2021  | Second Class  | Justin Ritter  | Corporate | Australia     | APAC   | 3709.40 | -288.77 | 0.1      |
| IN-2013-71249  | No       | 17-10-2021   | 18-10-2021  | First Class   | Craig Reiter   | Consumer  | Australia     | APAC   | 5175.17 | 919.97  | 0.1      |

### 2. Returns Table

Tracks returned orders along with the associated markets.

**Sample Data:**

| Returned | Order ID       | Market        |
|----------|----------------|---------------|
| Yes      | MX-2013-168137 | LATAM         |
| Yes      | US-2011-165316 | LATAM         |
| Yes      | ES-2013-1525878| EU            |
| Yes      | CA-2013-118311 | United States |

### 3. People Table

Contains sales representative names and their regions.

**Sample Data:**

| Person            | Region  |
|-------------------|---------|
| Anna Andreadi     | Central |
| Chuck Magee       | South   |
| Kelly Williams    | East    |
| Matt Collister    | West    |
| Deborah Brumfield | Africa  |

---

## ✅ Problem Statements Solved

### 1. Key Performance Indicators (KPIs)
**Objective:** Calculate and display Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.

**Steps:**
- Import the Orders Table into Excel using Power Query.
- Create calculated columns for:
  - `Profit Margin = Profit / Sales`
  - `Total Orders = Count of Order ID`
- Use Excel formulas to calculate:
  - `Total Sales = SUM(Sales)`
  - `Total Profit = SUM(Profit)`
  - `Total Quantity = SUM(Quantity)`
- Build a dynamic KPI table using symbols for visual appeal.

**📸 Screenshot:**  
![KPI Summary](images/kpi-summary.png)

---

### 2. Sales and Profit Analysis
**Objective:** Visualize sales and profit trends over time.

**Steps:**
- Create a Pivot Table grouped by Year and Month.
- Add Sales and Profit values.
- Use a Line Chart to display trends.
- Apply slicers for interactive filtering.

**📸 Screenshot:**  
![Sales Trend](images/sales-trend.png)

---

### 3. Category-Wise Profit
**Objective:** Analyze profitability across product categories.

**Steps:**
- Pivot Table using Category and Profit.
- Sort descending by Profit.
- Visualize with a Bar Chart.
- Add slicers for interactivity.

**📸 Screenshot:**  
![Category Profit](images/category-profit.png)

---

### 4. Segment-Wise Sales Share (%)
**Objective:** Show sales share by customer segment.

**Steps:**
- Pivot Table with Segment and Sales.
- Calculate percentage using formula.
- Display with Pie/Donut Chart and labels.

**📸 Screenshot:**  
![Segment Share](images/segment-wise-sales.png)

---

### 5. Sales by Country
**Objective:** Analyze sales by country.

**Steps:**
- Pivot Table with Country and Sales.
- Sort descending.
- Apply Heatmap or use Map Chart.

**📸 Screenshot:**  
![Country Sales](images/sales-by-country.png)

---

### 6. Top 5 Subcategories
**Objective:** Identify top 5 subcategories.

**Steps:**
- Pivot Table with Sub-Category and Sales.
- Sort descending.
- Filter Top 5.
- Visualize using Column Chart.

**📸 Screenshot:**  
![Top Subcategories](images/top-subcategories.png)

---

## ⚙️ Dynamic Features

- 🔄 **Dynamic Charts** – Auto-update with slicers.
- ⚙️ **Power Query Integration** – Streamlined data transformation.
- 📌 **KPI Table** – Instant visibility of key metrics.

---

## 🚀 Next Steps for Extension

- 📦 Return Analysis by product or market.
- 👥 Customer segmentation by profitability.
- 🌐 Deep Market vs Product performance insights.

---

## 🎯 Significance

This dashboard empowers retail businesses to:
- Track KPIs and trends effectively.
- Understand segment, category, and regional performance.
- Make data-driven decisions quickly and confidently.

---

## 📂 Visuals Directory

All referenced screenshots are stored in the `/images` folder of this repository.

---

## 👨‍💻 Author

**Santhosh Kumar P**  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/santhosh-kumar-p-77272928b)

---

## 📝 License

This project is shared for educational and demonstration purposes only.
