# E-Commerce-Performance-Insights
🛒 Advanced Power BI Dashboard | E-Commerce Analytics Suite
# 🛒 E-Commerce Performance Insights
### Advanced Power BI Dashboard Suite | Enterprise Analytics

## 📊 Overview
A comprehensive 5-page Power BI dashboard built on a 
10-million-row e-commerce dataset, featuring enterprise-grade 
Row Level Security, advanced DAX measures, and 30+ 
interactive visualizations.

## 🗂️ Dashboard Pages
| Page | Key Features |
|------|-------------|
| Executive Overview | AI Smart Narrative, 6 KPIs, Geographic map |
| Sales & Revenue | Brand Profitability Scorecard, Payment analysis |
| Customer Intelligence | Sankey Chart, CLV Distribution, RFM analysis |
| Product Performance | Waffle Chart, Category Matrix, Treemap |
| Logistics & Delivery | Choropleth map, Dual-axis trend, Funnel chart |

## 🔐 Enterprise Features
- **Row Level Security (RLS)** — 4 roles: Admin, Consumer, Corporate, VIP
- **Bidirectional security filters** across all related tables
- **Dynamic DAX measures** — YoY%, MoM%, 3MMA, CLV, Repeat Rate
- **Custom visuals** — Sankey Chart, Waffle Chart, Word Cloud, Funnel

## 📈 Key Metrics Tracked
- Total Revenue: 978.52M
- Total Orders: 4M
- On-Time Delivery Rate: 97.24%
- Average Review Score: 4.03
- Gross Margin: 25.70%
- Active Sellers: 500

## 🛠️ Technical Stack
- **Tool:** Microsoft Power BI Desktop
- **Data Model:** Star schema with 10 tables
- **DAX Measures:** 25+ custom calculations
- **Dataset Size:** 10 million rows (Customers table)
- **Security:** Row Level Security with 4 roles
- **Custom Visuals:** Sankey, Waffle Chart, Word Cloud, Drill-down Funnel

## 📐 Data Model
- Calendar (Date table — marked as Date Table)
- Customers (10M rows)
- Orders
- Order Items
- Order Payment
- Order Reviews
- Products
- Sellers
- Geo Location

## 🎯 Advanced DAX Measures
```dax
Revenue YoY % = 
DIVIDE(
    [Total Revenue] - [Revenue PY],
    [Revenue PY]
)

Revenue 3MMA = 
AVERAGEX(
    DATESINPERIOD('Calendar'[Date],
    MAX('Calendar'[Date]),-3,MONTH),
    [Total Revenue]
)
```

## 🔒 Row Level Security Setup
Four security roles implemented:
- **Admin** — Full data access
- **Consumer** — Filtered to Consumer segment (~623M revenue)
- **Corporate** — Filtered to Corporate segment (~177M revenue)  
- **VIP** — Filtered to VIP segment (~177M revenue)

## 📸 Dashboard Screenshots
[Add your 5 page screenshots here]

## 🚀 How To Use
1. Download the .pbix file
2. Open in Power BI Desktop
3. Data is embedded — no additional setup needed
4. Use navigation buttons to switch between pages
5. Use slicers to filter by Year, Month, Segment

## 👩‍💻 Author
**Anisha Jain**
- GitHub: [@anishajain734](https://github.com/anishajain734)
- LinkedIn: [in/anisha-jain-762514176](https://linkedin.com/in/anisha-jain-762514176)
- Email: ajain64@uw.edu
