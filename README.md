# Farmer_Market_Dashboard
Quantity-Wise Sales Analysis Dashboard (Power BI)

🚀 An interactive Power BI dashboard designed to analyze sales quantity across products, vendors, and customers for better business insights.

🌟 Project Overview

This project focuses on understanding quantity-wise sales performance using interactive visualizations and DAX measures. It helps identify top products, key vendors, and customer purchasing behavior in a simple and intuitive way.

🎯 Objectives

✅ Analyze total quantity sold
✅ Compare product and vendor performance
✅ Understand customer purchase patterns
✅ Enable data-driven decision-making

🛠 Tools & Technologies

📊 Power BI Desktop

🧮 DAX (Data Analysis Expressions)

📄 Excel / CSV Data

🔗 Data Modeling

🔗 Dashboard Visualizations

📈 Dashboard Features

📌 Visualizations Included

🥧 Pie Chart – Quantity by Product

🍩 Donut Chart – Quantity by Vendor

📊 Bar Chart – Product Count by Customer

📉 Column Chart – Quantity by Product

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
