# 📊 E-Commerce Performance & Customer Lifetime Value Dashboard (Power BI)

An end-to-end interactive Business Intelligence solution built in **Microsoft Power BI** to analyze Wix/Shopify store transactions, customer segmentation, product catalog performance, and customer retention dynamics.

---

## 🎯 Project Objective
The goal of this project is to transform raw e-commerce transactional data into actionable business insights. By modeling sales, product, and date dimensions into a cohesive star schema, this dashboard helps stakeholders answer three core questions:
1. **How is the business performing overall?**
2. **Who are our customers, where are they located, and what are they buying?**
3. **How well are we retaining customers, and how much value do repeat buyers generate?**

---

## 📑 Dashboard Architecture (3 Report Pages)

### 1. Executive Sales Overview
* **Top KPIs:** Total Revenue (`₹45.98L`), Total Orders (`7,431`), Average Order Value / AOV (`₹618.89`), and Repeat Purchase Rate (`46.02%`).
* **Visuals:**
  * **Daily Revenue Trend:** Line chart tracking daily sales velocity and demand spikes.
  * **Revenue by Product Type:** Horizontal bar chart highlighting top-performing categories (`Running Shoes`, `Tennis Shoes`, `Walking Shoes`).
  * **Revenue by Payment Gateway:** Donut chart breaking down checkout preferences (`Shopify Payments`, `PayPal`, `Gift Card`).
  * **Revenue by Day of Week:** Sequential column chart analyzing weekday vs. weekend purchasing behavior.

### 2. Customer & Product Insights
* **Top KPIs:** Total Unique Customers (`4,431`), Returning Customers (`2,039`), Repeat Purchase Rate (`46.02%`), and AOV (`₹618.89`).
* **Visuals:**
  * **New vs. Returning Customers:** Donut chart comparing first-time buyers (`53.98%`) against repeat buyers (`46.02%`).
  * **Top 10 VIP Customers by Revenue:** Top-N DAX filtered bar chart isolating the highest-spending customer accounts (led by Customer ID `1556`).
  * **Top 10 Cities by Revenue:** Geographic breakdown identifying core urban revenue hubs (`Washington`, `Houston`, `New York City`).

### 3. Customer Retention & Value
* **Top KPIs:** Repeat Purchase Rate (`46.02%`), Returning Customers (`2,039`), AOV (`₹618.89`), and Revenue from Returning Customers (`₹31.20L`).
* **Visuals:**
  * **Revenue: New vs. Returning Customers:** Comparative column chart demonstrating the revenue gap between repeat and first-time buyers.
  * **Repeat Purchase Trend:** Line chart tracking daily revenue generated exclusively by returning customers.
  * **Product Preferences of Returning Customers:** Bar chart identifying which product lines drive long-term customer loyalty.

---

## 🛠️ Data Modeling & DAX Measures
* **Data Model:** Relational Star Schema connecting the core fact table (`shopify_sales`) with a custom Date dimension (`Dim_Date`).
* **Key DAX Measures Implemented:**
  * `Total Revenue` & `Total Orders`
  * `Average Order Value (AOV)`
  * `Total Customers`, `Returning Customers`, & `New Customers`
  * `Repeat Purchase Rate (%)`
  * `Revenue from Returning Customers` & `Revenue from New Customers`

---

## 💡 Key Business Insights & Recommendations
1. **Retention Drives Profitability:** While returning customers represent **46.02%** of total headcount, they generate nearly **68% (`₹31.20 Lakhs`)** of total revenue. Retaining existing buyers yields more than double the revenue of new customer acquisition.
2. **Footwear Catalog Dominance:** Running, Tennis, and Walking Shoes drive over **70%** of overall sales and represent the highest repeat-purchase affinity.
3. **Checkout Optimization:** Shopify Payments (`58.45%`) and PayPal (`17.62%`) process over three-quarters of all revenue, making seamless integration on these gateways essential.
4. **Actionable Strategy:** Launch automated post-purchase email retention flows 30–60 days after a customer's first footwear purchase and focus targeted ad spend on top-converting metro cities (`Washington`, `Houston`, `New York City`).

---

## 📂 Repository Contents
* `Wix Shopify.pbix` — Complete Power BI Desktop report file with data model, DAX measures, and 3 interactive pages.
* `Shopify_Sales_Dashboard.pdf` — Exported static PDF report of all 3 dashboard sheets.
* `Presentation_Script.docx` — 10-minute executive walkthrough script and business summary.
* `README.md` — Project documentation.

---

## 🚀 How to Use
1. Clone this repository or download `Wix Shopify.pbix`.
2. Open the file in **Microsoft Power BI Desktop** (free to download).
3. Interact with the slicers, hover over charts for dynamic tooltips, and click on specific bars/slices to cross-filter metrics across each page.