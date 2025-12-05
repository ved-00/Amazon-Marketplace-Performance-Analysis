Amazon Marketplace Performance Analysis

SQL-based analysis of a real-world Amazon sales dataset to uncover category revenue patterns, order-flow dynamics, fulfillment behavior, statewise demand, and operational health signals across the marketplace.



📌 Project Overview

This project analyzes 1.02L+ Amazon marketplace transactions to understand demand patterns, order outcomes, revenue concentration, and region-level distribution.
The goal is to simulate what a Product Ops / Supply Chain Analyst would extract from raw e-commerce data.

All analysis was performed using SQL, running on CSV data imported into a query engine.



🧠 Key Insights (Executive Summary)

Order Funnel Mapping:
Processed 1.02L+ distinct orders, identifying 14.28% cancellations and 60.50% shipped orders, forming a clear order-status funnel.

Revenue Concentration:
Categories showed sharp skew — Kurtas alone contributed ₹3.92Cr+, the highest-earning product segment.

Demand & Network Patterns:
April saw peak throughput with 45,858 orders moving 44,206 units, while Maharashtra accounted for 21.82% of all orders among states.

These results demonstrate category economics, demand seasonality, and network load concentration.



🛠️ Tools Used

SQL (core analysis)

CSVFiddle / SQL Engine for executing queries on CSV

GitHub for version control & documentation



📊 Analysis Components

1️⃣ Top 10 Categories by Revenue
Identified which product categories drive majority of GMV.
Useful for assortment planning & merchandising strategy.

2️⃣ Monthly Fulfillment Performance
Tracks month-over-month delivery vs cancellation rates to detect recurring peak-load issues or fulfillment instability.

3️⃣ Order Status Distribution
Mapped orders across Shipped, Delivered, Cancelled, Pending, Returned, etc.

4️⃣ State-wise Order Share (%)
Computed order concentration across the top 10 states.

5️⃣ Busiest Order Dates
Identified peak shopping days & associated volumes.

6️⃣ Month-wise Orders & Units Summary
Compared throughput (distinct orders) vs. item movement (units).

7️⃣ Fulfillment Method Breakdown
Split orders fulfilled by Amazon vs Merchant.

8️⃣ Courier Status Outcomes
Shipped vs Unshipped vs Cancelled counts from logistics pipeline.

9️⃣ Month-wise Purchases by City
Demand distribution across cities for each month.

🔟 Cancellation Hotspots — by Category
Identifies product categories with unusually high cancellation rates to surface potential listing, sizing, or quality issues.

1️⃣1️⃣ Cancellation Hotspots — by State
Highlights regions with elevated cancellation patterns, useful for spotting courier bottlenecks or state-specific operational failures.

1️⃣2️⃣ Category-wise Return Rate Analysis
Breaks down return/refund rates across categories to pinpoint segments with potential product-quality gaps or expectation mismatches.

1️⃣3️⃣ High-Defect SKUs (Cancellation-Driven)
Ranks SKUs by defect/cancellation rate and revenue at risk to focus remediation on the highest-impact problem products.

1️⃣5️⃣ Courier Status Performance
Evaluates shipped, unshipped, and cancelled proportions per courier status bucket to reveal logistics-pipeline failure points.



📁 Dataset Information

This project uses the Amazon Sale Report dataset, which includes detailed marketplace order records such as order dates, quantities, categories, shipping locations, courier statuses, and revenue amounts.

Because the full dataset is fairly large (68 MB), GitHub cannot preview it directly.
The complete dataset is uploaded as a ZIP file:
