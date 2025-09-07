# 🛒 Online Retail Sales Data Analysis  

## 📌 Project Summary  
This project analyzes **online retail sales transactions** using **Excel/Google Sheets**.  
The dataset includes product details, pricing, customer regions, and order dates.  
The main objective is to perform **data cleaning, transformation, revenue analysis, trend exploration, and profit margin calculations** to uncover business insights such as:  
- High-revenue regions  
- Seasonal sales patterns  
- Top profit-generating products  
- Data validation and lookup efficiency  

---

## ✅ Analyses Performed  

### 1. Data Cleaning and Transformation  
- Identified and highlighted **null values** in `Quantity`, `Price_Per_Unit`, and `Total_Amount` using **Conditional Formatting**.  
- Filled missing numeric values with **rounded column averages**.  
- Removed extra spaces in product names using **TRIM()**.  
- Converted all product names in the `Product` column to **UPPERCASE** for consistency.  

---

### 2. PivotTable Analysis  
- Built a **PivotTable** to calculate `Total_Amount` grouped by `Customer_Region`.  
- Identified the **region with the highest revenue**.  
- Applied **Data Bars** (Conditional Formatting) to highlight regional revenue visually.  

---

### 3. Lookup Operations  
- Used **VLOOKUP** to find `Total_Amount` where `Order_ID = 1015`.  
- Used **INDEX + MATCH** to retrieve the `Category` where `Order_ID = 1027`.  
- Compared both methods and documented differences:  
  - `VLOOKUP` is simpler but limited (requires left-to-right lookup).  
  - `INDEX/MATCH` is more flexible (works in any direction).  

---

### 4. Trend Analysis  
- Plotted a **Line Chart** of `Total_Amount` over `Order_Date`.  
- Analyzed revenue trends across time periods.  
- Highlighted seasonal **spikes and dips in sales**.  

---

### 5. Profit Margin Calculation  
- Added a calculated column:  
  ```text
  Profit_Margin = Total_Amount - (Quantity × Price_Per_Unit × 0.6)
  ```  
- Applied Conditional Formatting to highlight products with **Profit Margin > ₹5000**.  
- Sorted data by `Profit_Margin` in descending order.  
- Extracted the **Top 3 profit-generating products** into a summary table.  

---

## 📈 Deliverables  
- **Cleaned dataset** (nulls handled, trimmed, uppercase formatting).  
- **PivotTable** showing revenue by region.  
- **Line chart** showing sales trends over time.  
- **Lookup comparisons** (VLOOKUP vs INDEX/MATCH).  
- **Profit margin analysis** with top 3 products.  

---

## 🛠️ Tools Used  
- **Excel / Google Sheets**  
- Functions: `TRIM`, `UPPER`, `AVERAGE`, `VLOOKUP`, `INDEX`, `MATCH`  
- PivotTables, Conditional Formatting, Line Charts  

---
