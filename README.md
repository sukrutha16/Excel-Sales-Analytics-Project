# Sales and Financial Analytics using Excel

## Objective
Analyze the sales and financial performance of AtliQ Hardware, a computer peripherals manufacturer selling products through brick-and-mortar stores, e-commerce platforms, and its own store, across various countries. The goal was to generate insightful reports like customer performance, market vs. target, and profit & loss (P&L) statements for the years 2019, 2020, and 2021.

---

## Procedure

### 1. Data Preparation
- **Data Import:** Imported datasets in CSV format:
  - `dim_customer`
  - `dim_market`
  - `dim_product`
  - `fact_sales_monthly`
- **Data Cleaning (Power Query):**
  - Removed duplicates
  - Corrected spelling errors
  - Split columns
  - Replaced null values
  - Standardized data types
- **Data Modeling:**
  - Built a data model by connecting tables using primary and foreign key relationships.

### 2. Sales Analytics
#### **Customer Performance Report**
- Created a pivot table with calculated DAX measures:
  - **Net Sales**
  - **Yearly Net Sales (2019, 2020, 2021)**
  - **Growth Percentage (2021 vs. 2020)**
- Applied filters for market, division, and region to derive granular insights.

#### **Market vs. Target Report**
- Imported `ns_targets_21.csv` for target data.
- Created DAX measures:
  - **Target Sales 2021**
  - **Target vs. Net Sales (%)**
- Visualized market-wise Net Sales, Target Sales, and percentage differences using conditional formatting.

### 3. Financial Analytics
#### **Data Import**
- Imported `fact_sales_monthly_with_cost.csv` containing additional columns:
  - Freight Cost
  - Manufacturing Cost

#### **Metrics Calculation (Power Pivot):**
- **Total COGS:** Manufacturing Cost + Freight Cost
- **Gross Margin (GM):** Net Sales - Total COGS
- **Gross Margin % (GM%):** GM / Net Sales

#### **P&L Statement Reports:**
- **Yearly Analysis:**
  - Metrics: Net Sales, Total COGS, GM, and GM% for 2019, 2020, and 2021.
  - Insights: GM% was highest in 2019, while Net Sales, COGS, and GM peaked in 2021.
- **Monthly and Quarterly Analysis:**
  - Highlighted consistent sales peaks in November and December across all three years.

---

## Tools and Features Used
- **Excel Functionalities:**
  - Power Query
  - Power Pivot
  - DAX
  - Pivot Tables
- **Visualization Techniques:**
  - Conditional formatting to emphasize key trends and insights.

---

## Key Business Insights
1. **Sales Growth:**
   - The PC division experienced a remarkable growth of **313.7%** in 2021 compared to 2020.
   - November and December consistently showed higher sales and profitability.

2. **Top Performers:**
   - **Top 5 Countries (2021 Sales):** India, USA, South Korea, Canada, and the UK.
   - **Top 10 Products (2021 vs. 2020 Growth)**
   - **Top 5 & Bottom 5 Products by Quantity Sold.**

3. **Financial Trends:**
   - GM% was highest in 2019, but Net Sales, COGS, and GM peaked in 2021.

4. **Actionable Insights:**
   - Identified top-performing divisions, markets, and products for strategic planning.
   - Financial analysis helped understand cost dynamics and profitability improvements.

---

## Conclusion
This project demonstrates advanced Excel skills in data analysis, modeling, and visualization. It provides actionable insights for AtliQ Hardware, enabling data-driven decisions to optimize business performance.

