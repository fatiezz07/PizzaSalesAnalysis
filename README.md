<h1>🍕 Pizza Sales Analysis - Business Intelligence Dashboard</h1>

### [Live Dashboard](https://github.com/yourusername/pizza-sales-analysis)

<h2>Description</h2>
Comprehensive business intelligence project analyzing 2 years of pizza sales data ($817,860 total revenue) using SQL for data extraction and Excel for interactive dashboard creation. The project demonstrates end-to-end data analysis capabilities, from raw transactional data processing to actionable business insights and strategic recommendations for operational optimization.

<br />

<h2>Languages and Tools Used</h2>

- <b>SQL (Microsoft SQL Server)</b> - Data extraction, aggregation, and KPI calculations
- <b>Microsoft Excel</b> - Interactive dashboard creation with pivot tables and charts  
- <b>Data Visualization</b> - Chart design, color theory, and user experience optimization
- <b>Business Intelligence</b> - KPI identification, trend analysis, and strategic insights

<h2>Skills Demonstrated</h2>

- <b>Data Analysis</b> - Statistical analysis, pattern recognition, correlation identification
- <b>SQL Proficiency</b> - Complex queries, window functions, date/time operations, CTEs
- <b>Dashboard Development</b> - Interactive filters, dynamic charts, professional styling
- <b>Business Acumen</b> - Strategic recommendations, ROI analysis, operational insights

<h2>Key Performance Indicators (KPIs):</h2>

<p align="center">
<b>Total Revenue:</b> $817,860 | <b>Average Order Value:</b> $38.31 | <b>Total Orders:</b> 21,350
<br/>
<b>Total Pizzas Sold:</b> 49,574 | <b>Avg Pizzas Per Order:</b> 2.32
</p>

<h2>Project walk-through:</h2>

<p align="center">
<b>Main Dashboard Overview:</b> <br/>
<img src="https://i.imgur.com/dashboard_main.png" height="80%" width="80%" alt="Pizza Sales Dashboard Main View"/>
<br />
<br />
<b>KPI Summary Cards:</b>  <br/>
<img src="https://i.imgur.com/kpi_cards.png" height="80%" width="80%" alt="Key Performance Indicators"/>
<br />
<br />
<b>Daily Trend Analysis (Peak Days: Weekends):</b> <br/>
<img src="https://i.imgur.com/daily_trends.png" height="80%" width="80%" alt="Daily Sales Trends"/>
<br />
<br />
<b>Hourly Trend Analysis (Peak Hours: 12-1PM, 5-8PM):</b>  <br/>
<img src="https://i.imgur.com/hourly_trends.png" height="80%" width="80%" alt="Hourly Sales Patterns"/>
<br />
<br />
<b>Sales by Pizza Category (Classic: 26.91% of revenue):</b>  <br/>
<img src="https://i.imgur.com/category_analysis.png" height="80%" width="80%" alt="Pizza Category Performance"/>
<br />
<br />
<b>Sales by Pizza Size (Large: 45.89% of revenue):</b>  <br/>
<img src="https://i.imgur.com/size_analysis.png" height="80%" width="80%" alt="Pizza Size Distribution"/>
<br />
<br />
<b>Top 5 Best Sellers (Classic Deluxe Pizza leads):</b>  <br/>
<img src="https://i.imgur.com/best_sellers.png" height="80%" width="80%" alt="Top Performing Pizzas"/>
<br />
<br />
<b>Bottom 5 Worst Sellers (Optimization opportunities):</b>  <br/>
<img src="https://i.imgur.com/worst_sellers.png" height="80%" width="80%" alt="Underperforming Products"/>
<br />
<br />
<b>Interactive Filter Controls:</b>  <br/>
<img src="https://i.imgur.com/filter_controls.png" height="80%" width="80%" alt="Dashboard Filters and Slicers"/>
</p>

<h2>SQL Query Examples:</h2>

```sql
-- Total Revenue Calculation
SELECT SUM(total_price) AS Total_Revenue 
FROM pizza_sales;

-- Daily Order Patterns
SELECT DATENAME(DW, order_date) AS order_day, 
       COUNT(DISTINCT order_id) AS total_orders
FROM pizza_sales
GROUP BY DATENAME(DW, order_date);

-- Top 5 Best Selling Pizzas
SELECT TOP 5 pizza_name, 
       SUM(quantity) AS Total_Pizza_Sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Pizza_Sold DESC;
```

<h2>Key Business Insights:</h2>

- **🕐 Peak Performance**: Weekends generate highest order volumes, with Friday-Saturday showing 40% higher sales
- **⏰ Optimal Hours**: 12-1 PM (lunch) and 5-8 PM (dinner) represent 65% of daily orders  
- **🍕 Product Winners**: Classic pizzas drive 26.91% of revenue; Large size pizzas dominate at 45.89%
- **📈 Growth Opportunities**: Thursday shows 25% lower sales, indicating promotional potential
- **💰 Revenue Optimization**: Average order value of $38.31 suggests successful upselling strategies

<h2>Strategic Recommendations:</h2>

- **Operational**: Increase staffing during peak hours (12-1 PM, 5-8 PM) and weekends
- **Marketing**: Target Thursday promotions to boost mid-week performance  
- **Menu**: Focus inventory on Classic and Supreme categories (52% of total sales)
- **Pricing**: Promote Large pizza upgrades to maximize revenue per transaction
- **Analytics**: Implement real-time dashboard for continuous performance monitoring


**Contact Information:**
- **Email:** Businesstalibi@gmail.com
- **LinkedIn:** [linkedin.com/in/fati-talibi](https://www.linkedin.com/in/fati-talibi)  
- **Phone:** (309) 350-7172
- **Location:** Rock Island, IL

*Seeking Business Intelligence and Data Analytics opportunities to drive data-driven decision making!*
