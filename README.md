# 🛍️ E-Commerce Sales & Profitability Dashboard | Power BI Project

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://learn.microsoft.com/en-us/dax/)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://www.microsoft.com/excel)

## 📌 Project Overview
An interactive Power BI dashboard built on **500 orders (1,500 order-line records)** from an Indian e-commerce business, analyzing sales, profit, and quantity across product categories, states, customers, and payment modes for the 2018 financial year. Two CSV sources (`Orders.csv` and `Details.csv`) are joined on `Order ID` and modeled with DAX to power a single-page executive dashboard with quarter and category slicers.

**Goal:** Identify which products, states, and customers are actually profitable — not just high-revenue — so the business can fix or drop loss-making lines and double down on what works.

## 🎯 Business Problem
Revenue alone hides the real picture in e-commerce, where returns, discounts, and category mix can quietly erase margin. This dashboard answers:
- Which states and sub-categories are profitable vs. loss-making?
- Which months lost money, and why?
- Which product category drives the most order volume?
- Which payment mode is most used, and does that affect fulfillment cost/strategy?
- Who are the top customers by spend?

## 📊 Dataset
| Field | Detail |
|---|---|
| Orders analyzed | 500 orders / 1,500 order-line items |
| Period | January – December 2018 |
| Source files | [`Orders.csv`](./data/Orders.csv), [`Details.csv`](./data/Details.csv) |
| Fields | Order ID, Order Date, CustomerName, State, City, Amount, Profit, Quantity, Category, Sub-Category, PaymentMode |

## 🛠️ Tools & Approach
1. **Excel/Power Query** – Cleaned and merged `Orders.csv` and `Details.csv` on `Order ID`.
2. **DAX** – Built measures for Sum of Amount, Sum of Profit, Sum of Quantity, and Average Order Value (AOV).
3. **Power BI** – Designed a single-page dashboard with KPI cards, quarter slicers, a profit-by-month trend chart, and category/payment-mode breakdowns by donut and bar visuals.

## 📈 Dashboard Preview
![E-Commerce Dashboard](./images/powerbi%20learning%20dashboard.png)

## 🔍 Key Insights (from the actual 1,500-row dataset)
- **Total Revenue: ₹4.38L (438K)** generated **₹37K in profit** — an overall margin of just **8.4%**, signaling thin margins that leave little room for error in pricing or discounting.
- **Average Order Value: ₹121** across all 500 orders, useful as a baseline to track whether future pricing or upsell strategies move the needle.
- **Madhya Pradesh and Maharashtra are the top 2 profit states** (₹7,382 and ₹6,963), together contributing **over 38% of total profit** from just 2 of 19 states — a clear case for concentrating regional marketing spend.
- **Andhra Pradesh and Rajasthan are net loss-making** (-₹280 and -₹323 in profit) despite generating revenue, meaning at least 2 states are actively hurting the bottom line.
- **Clothing drives 62.6% of total quantity sold** (3,516 of 5,615 units), more than 3x Electronics (20.6%) and Furniture (16.8%) combined relative share — confirming Clothing as the core volume driver.
- **Printers and Bookcases are the most profitable sub-categories** (₹8,606 and ₹6,516), while **Furnishings, Electronic Games, and Kurti are net loss-makers** (-₹806, -₹644, -₹401) — these 3 sub-categories alone erase nearly ₹1,851 in profit and are candidates for repricing or delisting.
- **4 of 12 months ran at a net loss** (May, July, September, December), with May the worst at **-₹3,730**, while November was the strongest month at **+₹10,253** — a seasonal pattern worth investigating for promotions or cost spikes.
- **COD is the most-used payment mode at 39.4% of quantity sold**, nearly double UPI (18.8%), which matters for cash-flow and return-rate risk planning.

## 🚀 How to Use This Project
```bash
git clone https://github.com/ankitabisht-data-analyst/ecommerce-sales-profitability-dashboard-powerbi.git
```
1. Open [`POWERBI_PROJECT_LEARNING.pbix`](./powerbi/POWERBI_PROJECT_LEARNING.pbix) in Power BI Desktop.
2. Refresh the data source to point to [`Orders.csv`](./data/Orders.csv) and [`Details.csv`](./data/Details.csv).
3. Use the Quarter and Category slicers to explore the data interactively.

## 📈 Skills Demonstrated
`Power BI` `DAX` `Power Query` `Data Cleaning` `Data Modeling` `Profitability Analysis` `Data Visualization` `KPI Reporting` `Dashboard Design`

## 📬 Contact
**Ankita Bisht** — Data Analyst
[LinkedIn](https://www.linkedin.com/in/ankita-bisht09) · [GitHub](https://github.com/ankitabisht-data-analyst)

⭐ If you found this project useful, consider giving it a star!
