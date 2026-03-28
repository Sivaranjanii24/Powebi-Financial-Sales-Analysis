# 📊 Power BI Project: Finance Power BI Financial Sales Dashboard

## 🧠 Project Overview
This Power BI dashboard analyzes the **Sample Superstore dataset**, a retail dataset containing sales, profit, and order details.

The project focuses on uncovering insights into **financial performance, profitability, sales trends, and regional analysis** to support data-driven decision-making.

---

## 🗂️ Dataset & Source Information
- **Source:** Sample Superstore Dataset  
- **File Type:** Excel (converted for Power BI)

### Key Fields Used:
- Order Date  
- Sales  
- Profit  
- Quantity  
- Region  
- Category & Sub-Category  
- Customer Segment  

---

## 🧰 Tools & Technologies Used
- Power BI Desktop  
- Power Query  
- DAX (Data Analysis Expressions)  
- Microsoft Excel  

---

## 📈 Dashboard Features & Sections

### 🔹 Sales Overview
- KPIs: Total Sales, Total Profit, Total Quantity  
- Monthly & Yearly Sales Trends  
- Overall performance summary  

### 🔹 Profit Analysis
- Profit by Category & Sub-Category  
- Loss-making products identification  
- Profit vs Discount analysis  

### 🔹 Regional Analysis
- Sales & Profit by Region  
- Top and underperforming regions  

### 🔹 Category Performance
- Category-wise sales contribution  
- Sub-category breakdown  
- Interactive filters for analysis  

---

## 🧮 Sample DAX Measures

```DAX
Total Sales = SUM(Orders[Sales])

Total Profit = SUM(Orders[Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Sales YoY Growth % =
VAR CurrentYear = [Total Sales]
VAR PreviousYear =
    CALCULATE(
        [Total Sales],
        SAMEPERIODLASTYEAR(Orders[Order Date])
    )
RETURN
    DIVIDE(CurrentYear - PreviousYear, PreviousYear)
```

---

## 💡 Key Insights
- Sales show steady growth with seasonal variations  
- High discounts reduce profitability  
- Technology category generates highest sales  
- Some regions have high sales but low profit  

---

## 📁 Project Files
- Project Final 1.pbix — Power BI Dashboard  
- Sample - Superstore.xlsx — Dataset  
- README.md — Documentation  

---

## 📂 Project Access
https://github.com/Sivaranjanii24/Powebi-Financial-Sales-Analysis

---

## 🚀 How to Use
1. Download the `.pbix` file  
2. Open in Power BI Desktop  
3. Use filters and visuals to explore insights  

---

## 🧑‍💻 Author
**Sivaranjani M**  
Aspiring Data Analyst | Power BI | SQL | Excel  
📧 sivaranjani0924@gmail.com
