[README.md](https://github.com/user-attachments/files/28825704/README.md)
# Project 1: Sales Performance Dashboard — Superstore Dataset

**Author:** Mohit Suryawanshi  
**GitHub:** https://github.com/MohitSuryawanshi-97  
**Tools:** Python, Pandas, Matplotlib, Seaborn, SQLite, openpyxl

---

## 📌 Overview
End-to-end analysis of 9,994 Superstore sales records across 3 product categories and 4 regions.
Covers SQL querying, data aggregation, KPI calculation, and a 6-panel dashboard chart.

## 📊 Key Results
- Top categories contribute **62% of total revenue**
- West region has the **highest profit margin** among all regions
- Heavy discounts (>30%) directly correlate with **negative profit** (r ≈ -0.45)
- YoY sales growth tracked across 2020–2023

## 📁 Output Files (generated in `outputs/`)
| File | Description |
|------|-------------|
| `superstore_data.csv` | Full generated dataset (9,994 rows) |
| `sales_summary.xlsx` | Multi-sheet Excel: raw data + aggregations |
| `sales_dashboard.png` | 6-panel analysis dashboard chart |
| `yoy_growth.png` | Year-over-year sales growth bar chart |

## 🚀 How to Run
```bash
pip install pandas numpy matplotlib seaborn openpyxl
python sales_analysis.py
```

## 🗂️ SQL Queries Covered
- Category-wise sales & profit with revenue share %
- Region-wise profit margin using **window functions** (RANK)
- **YoY growth** calculation using LAG()
- Discount impact analysis on profit margin
- Top 5 sub-categories by revenue

## 📈 Charts Produced
1. Total Sales by Category (bar)
2. Profit Margin % by Region (bar)
3. Monthly Sales & Profit Trend 2023 (line)
4. Revenue Share by Segment (pie)
5. Top 10 Sub-Categories by Profit (horizontal bar)
6. Discount vs Profit Scatter (scatter + colorbar)
