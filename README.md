# amazon-sales
Power BI dashboard (2013-2022) shows sales trends, top products, and customer insights with dynamic KPIs and DAX for smart business decisions.

# Project Title:
Sales & Financial Analysis Dashboard with YTD KPIs, Time Intelligence, and Product Insights

# KPI Requirements & Implementation:
KPI	Definition	DAX/Power BI Implementation
✅ YTD Sales (Amount)	Total revenue from Jan 1 to current date in selected year	TOTALYTD(SUM(Sales[Amount]), 'Date'[Date])
✅ OTD Sales	Overall total sales (no time filter)	SUM(Sales[Amount])
✅ YTD Product Sales	Quantity sold YTD per product	TOTALYTD(SUM(Sales[Quantity]), 'Date'[Date])
✅ YTD Reviews	Total number of reviews YTD	TOTALYTD(SUM(Sales[Reviews]), 'Date'[Date])

# Business Domain:
•	Domain: Consumer Electronics / E-commerce
•	Business Type: Product-based, international retail with a focus on audio-video accessories.
•	Business Flow Overview:
o	Customers place online orders across various product categories.
o	Orders are reviewed, shipped, and tracked.
o	Financial records track revenue, expenditure, fund balance, and asset growth.
o	Product-level data includes pricing, quantity sold, customer reviews, and shipment status.

# Chart Requirements:
Chart	Description
📅 Sales by Month	Line or column chart showing monthly trend using Date[Month]
🗓️ Sales by Week	Area or column chart with Date[WeekNum] and weekly aggregation
📂 Sales by Category	Bar chart grouped by Product Category
🏆 Top 5 Products	Horizontal bar chart sorted by quantity sold or total sales
⭐ Top 5 Reviewed Products	Bar chart sorted by total review count

# Documentation Notes:
•	Date Table Includes: Year, Quarter, Month, Week, Day, Month Name, Day Name.
•	Time Intelligence Used: TOTALYTD, SAMEPERIODLASTYEAR, PARALLELPERIOD, DATESMTD, etc.
•	Data Model Relationships: Sales Table linked to Date Table via Order Date.
•	Filter Setup: Year slicers, category slicers, dynamic calendar filtering for performance comparison.

# Conclusion:
The Power BI dashboard offers real-time, interactive insights into both financial and sales performance. By implementing time intelligence, YTD tracking, and product-level analysis, the report empowers decision-makers to:
•	Monitor financial growth and operational efficiency
•	Identify top-performing products
•	Track trends by week/month/year
•	Make inventory and marketing decisions based on reviews and sales volume
This well-documented and validated report follows best practices in data modeling, DAX, and Power Query for optimal performance and user experience.
