# retailco-sales-dashbaord


Tool: Power BI | Track: BI Intermediate | Industry: Retail

_Business Problem_

RetailCo is a mid-sized Nigerian retailer operating 15 stores across Lagos, Abuja, Port Harcourt, Kano, and other major cities, selling electronics, home appliances, and furniture. Their Sales Director, Mrs. Adeyemi, and her team relied on Excel spreadsheets that took 2 days to update manually, meaning decisions were always made on stale data or gut feeling.
My task as the incoming BI Analyst was to build an interactive dashboard that lets Mrs. Adeyemi open her laptop on Monday morning and make 3 confident business decisions in under 5 minutes without calling anyone.

_Tools & Skills Used_

Power BI · DAX · Power Query · Data Modeling (Star Schema) · Time Intelligence · Data Visualization

_My Process_

Data Modeling-  
I worked with 6 data sources: Sales Transactions (10,000 rows), Stores, Products, Sales Reps, Customers, and a Calendar table. I built a star schema with the Sales Transactions table as the central fact table, connected to all 5 dimension tables via one-to-many relationships. Foreign key columns were hidden from Report View to keep the model clean.

DAX Measures- 
I created 15+ measures across two categories:
	· Basic: Total Sales, Total Profit, Profit Margin %, Average Order Value, Total Orders, MoM Sales Growth %
	· Time Intelligence: Sales YTD, Previous Year Sales, YoY Growth % using SAMEPERIODLASTYEAR() and CALCULATE() to enable period comparisons

Dashboard Design 
The report is structured across two pages:
	· Page 1 — Executive Summary: Top-line KPIs, monthly sales trend, top and bottom performing products, and cities with highest costs
	· Page 2 — Store Performance: Store-level target vs. actual, sales rep rankings, profit by category, and regional sales breakdown
        
_Key Business Insights_

	1. RetailCo generated $4.95bn in total sales with an 18.3% profit margin — however, MoM growth sits at just 6.81%, suggesting growth is slowing and needs attention at the store level.
	2. Sales peaked in October and dipped sharply in July — this seasonal pattern suggests RetailCo should plan promotional campaigns in Q3 to protect against the mid-year slump.
	3. Lagos Island leads all stores with $825M in monthly sales — nearly 60% above the next best store, indicating a concentration risk if that one store underperforms.
	4. Electronics dominates profit by category — Appliances and Furniture trail significantly, raising the question of whether underperforming categories need pricing or stocking strategy reviews.
	5. Top sales rep Chukwudi Eze closed 424 orders — nearly 3x the volume of lower-ranked reps, suggesting best practices from top performers aren't being shared across the team.
<img width="957" height="541" alt="image" src="https://github.com/user-attachments/assets/54752c92-c1f8-4728-bc42-1e47758d6417" />
