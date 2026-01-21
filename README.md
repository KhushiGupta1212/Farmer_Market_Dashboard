# Farmer_Market_Dashboard
Quantity-wise Sales Analysis Dashboard (Power BI)
📌 Project Overview

This project presents a Power BI dashboard designed to analyze product sales quantities across customers, vendors, and products. The dashboard helps stakeholders understand purchasing patterns, vendor contributions, and product performance through interactive visualizations.

Objectives

--Analyze total quantity sold by product, vendor, and customer

--Identify top-performing products and vendors

--Understand customer purchasing behavior

--Enable data-driven decision-making using interactive filters

🛠 Tools & Technologies

*Power BI Desktop

*DAX (Data Analysis Expressions)

*Data Modeling

*Microsoft Excel / CSV (Data Source)

*Power Bi query editor

*Dashboard Visualizations

#The dashboard includes the following visuals:

--Pie Chart – Quantity distribution by product name

--Donut Chart – Total quantity by vendor

--Bar Chart – Count of products purchased by customer

--Column Chart – Total quantity sold by product

--Slicer – Customer-wise filtering for interactive analysis

#Business Objective

*The goal of this project is to:

--Analyze quantity sold across products, customers, and vendors

--Identify top-performing products and vendors

--Understand customer purchasing behavior

--Support data-driven decision-making

#Key DAX Measures

1. Total Quantity = SUM(customer_purchases[quantity])
2. Product Count = COUNT(customer_purchases[product_id])
3. Quantity by Vendor =
CALCULATE(
    SUM(customer_purchases[quantity]),
    ALLEXCEPT(customer_purchases, customer_purchases[vendor_id])
)

4. Quantity by Product =
CALCULATE(
    SUM(customer_purchases[quantity]),
    ALLEXCEPT(customer_purchases, customer_purchases[product_id])
)

#How to Use the Dashboard

1️⃣ Clone this repository
2️⃣ Open the .pbix file in Power BI Desktop
3️⃣ Refresh the data (if needed)
4️⃣ Use slicers and visuals to explore insights

#Future Enhancements

🔹 Add KPI cards (Total Sales, Avg Quantity)
🔹 Monthly / Time-series trend analysis
🔹 Top-N product & vendor ranking
🔹 Tooltips with detailed insights
