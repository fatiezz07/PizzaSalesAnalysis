<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pizza Sales Analysis Dashboard</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f8f9fa;
        }
        
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px;
            border-radius: 10px;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .header h1 {
            margin: 0;
            font-size: 2.5em;
            font-weight: 700;
        }
        
        .subtitle {
            margin-top: 10px;
            font-size: 1.2em;
            opacity: 0.9;
        }
        
        .section {
            background: white;
            margin: 20px 0;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .kpi-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .kpi-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }
        
        .kpi-value {
            font-size: 2em;
            font-weight: bold;
            margin: 10px 0;
        }
        
        .kpi-label {
            font-size: 0.9em;
            opacity: 0.9;
        }
        
        .insights-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .insight-card {
            background: #f8f9fa;
            border-left: 4px solid #667eea;
            padding: 20px;
            border-radius: 5px;
        }
        
        .insight-card h4 {
            margin: 0 0 10px 0;
            color: #667eea;
            font-weight: 600;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
        }
        
        .tech-badge {
            background: #667eea;
            color: white;
            padding: 5px 12px;
            border-radius: 15px;
            font-size: 0.9em;
            font-weight: 500;
        }
        
        .code-block {
            background: #2d3748;
            color: #e2e8f0;
            padding: 20px;
            border-radius: 5px;
            overflow-x: auto;
            margin: 15px 0;
            font-family: 'Courier New', monospace;
            font-size: 0.9em;
            line-height: 1.4;
        }
        
        .recommendations {
            background: linear-gradient(135deg, #48bb78 0%, #38a169 100%);
            color: white;
            padding: 25px;
            border-radius: 10px;
            margin: 20px 0;
        }
        
        .recommendations h3 {
            margin-top: 0;
        }
        
        .rec-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .rec-item {
            background: rgba(255,255,255,0.1);
            padding: 15px;
            border-radius: 5px;
        }
        
        .rec-item h4 {
            margin: 0 0 10px 0;
            font-size: 1.1em;
        }
        
        .contact-section {
            background: linear-gradient(135deg, #2d3748 0%, #4a5568 100%);
            color: white;
            text-align: center;
            padding: 30px;
            border-radius: 10px;
        }
        
        .contact-links {
            margin: 20px 0;
        }
        
        .contact-links a {
            color: #90cdf4;
            text-decoration: none;
            margin: 0 15px;
            font-weight: 500;
        }
        
        .contact-links a:hover {
            color: #63b3ed;
            text-decoration: underline;
        }
        
        .tags {
            text-align: center;
            margin: 20px 0;
        }
        
        .tag {
            background: #e2e8f0;
            color: #2d3748;
            padding: 3px 8px;
            border-radius: 10px;
            font-size: 0.8em;
            margin: 2px;
            display: inline-block;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        
        th, td {
            border: 1px solid #e2e8f0;
            padding: 12px;
            text-align: left;
        }
        
        th {
            background: #f7fafc;
            font-weight: 600;
            color: #2d3748;
        }
        
        .highlight {
            background: #fef5e7;
            border-left: 4px solid #f6ad55;
            padding: 15px;
            margin: 15px 0;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>🍕 Pizza Sales Analysis Dashboard</h1>
        <div class="subtitle">A comprehensive business intelligence project analyzing 2 years of pizza sales data using SQL and Excel</div>
    </div>

    <div class="section">
        <h2>📊 Project Overview</h2>
        <p>This project demonstrates end-to-end data analysis capabilities by examining pizza sales performance across multiple dimensions including time trends, product categories, and customer ordering patterns. The analysis provides actionable insights for business optimization and strategic decision-making.</p>
    </div>

    <div class="section">
        <h2>🎯 Key Performance Indicators (KPIs)</h2>
        <div class="kpi-grid">
            <div class="kpi-card">
                <div class="kpi-value">$817,860</div>
                <div class="kpi-label">Total Revenue</div>
            </div>
            <div class="kpi-card">
                <div class="kpi-value">$38.31</div>
                <div class="kpi-label">Average Order Value</div>
            </div>
            <div class="kpi-card">
                <div class="kpi-value">49,574</div>
                <div class="kpi-label">Total Pizzas Sold</div>
            </div>
            <div class="kpi-card">
                <div class="kpi-value">21,350</div>
                <div class="kpi-label">Total Orders</div>
            </div>
            <div class="kpi-card">
                <div class="kpi-value">2.32</div>
                <div class="kpi-label">Avg Pizzas Per Order</div>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>🔍 Key Insights Discovered</h2>
        <div class="insights-grid">
            <div class="insight-card">
                <h4>🕐 Temporal Patterns</h4>
                <ul>
                    <li><strong>Peak Days:</strong> Weekends show highest order volumes</li>
                    <li><strong>Peak Hours:</strong> 12-1 PM and 5-8 PM represent peak ordering windows</li>
                    <li><strong>Opportunity:</strong> Thursday shows potential for targeted promotions</li>
                </ul>
            </div>
            <div class="insight-card">
                <h4>🍕 Product Performance</h4>
                <ul>
                    <li><strong>Top Category:</strong> Classic pizzas drive 26.91% of total sales</li>
                    <li><strong>Size Preference:</strong> Large pizzas generate 45.89% of revenue</li>
                    <li><strong>Best Seller:</strong> Classic Deluxe Pizza leads in quantity sold</li>
                </ul>
            </div>
            <div class="insight-card">
                <h4>💰 Revenue Distribution</h4>
                <ul>
                    <li><strong>Category Split:</strong> Classic (26.91%) > Supreme (25.46%)</li>
                    <li><strong>Size Analysis:</strong> Large dominates revenue share</li>
                    <li><strong>Upselling:</strong> Price-conscious opportunities identified</li>
                </ul>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>🛠️ Technical Implementation</h2>
        
        <h3>Tools & Technologies</h3>
        <div class="tech-stack">
            <span class="tech-badge">SQL Server</span>
            <span class="tech-badge">Microsoft Excel</span>
            <span class="tech-badge">Advanced Dashboard Design</span>
            <span class="tech-badge">Data Visualization</span>
            <span class="tech-badge">Business Intelligence</span>
        </div>

        <h3>Data Processing Pipeline</h3>
        <ol>
            <li><strong>Data Extraction:</strong> Complex SQL queries for KPI calculation</li>
            <li><strong>Data Transformation:</strong> Date/time parsing and categorical grouping</li>
            <li><strong>Visualization:</strong> Interactive Excel dashboard with multiple chart types</li>
            <li><strong>Insights Generation:</strong> Business intelligence interpretation</li>
        </ol>
    </div>

    <div class="section">
        <h2>🔧 SQL Query Highlights</h2>
        
        <h3>Revenue Analysis</h3>
        <div class="code-block">
-- Total Revenue Calculation
SELECT SUM(total_price) AS Total_Revenue 
FROM pizza_sales;
        </div>

        <h3>Time-Based Trends</h3>
        <div class="code-block">
-- Daily Order Patterns
SELECT DATENAME(DW, order_date) AS order_day, 
       COUNT(DISTINCT order_id) AS total_orders
FROM pizza_sales
GROUP BY DATENAME(DW, order_date);
        </div>

        <h3>Product Performance</h3>
        <div class="code-block">
-- Top 5 Best Selling Pizzas
SELECT TOP 5 pizza_name, 
       SUM(quantity) AS Total_Pizza_Sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Pizza_Sold DESC;
        </div>
    </div>

    <div class="recommendations">
        <h3>📈 Business Recommendations</h3>
        <div class="rec-grid">
            <div class="rec-item">
                <h4>Operational Optimization</h4>
                <ul>
                    <li>Increase weekend and peak hour staffing</li>
                    <li>Prioritize Classic and Supreme pizza ingredients</li>
                    <li>Target Thursday promotions to boost mid-week sales</li>
                </ul>
            </div>
            <div class="rec-item">
                <h4>Revenue Enhancement</h4>
                <ul>
                    <li>Promote Large size upgrades (45.89% of revenue)</li>
                    <li>Consider reformulating underperforming items</li>
                    <li>Create meal deals around high-performing pizzas</li>
                </ul>
            </div>
            <div class="rec-item">
                <h4>Data-Driven Insights</h4>
                <ul>
                    <li>Implement quarterly performance tracking</li>
                    <li>Analyze order patterns by demographics</li>
                    <li>Forecast demand based on historical trends</li>
                </ul>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>📁 Repository Structure</h2>
        <div class="code-block">
pizza-sales-analysis/
│
├── data/
│   ├── raw_data/
│   │   └── pizza_sales.csv
│   └── processed_data/
│       └── kpi_results.xlsx
│
├── sql_queries/
│   ├── kpi_queries.sql
│   ├── trend_analysis.sql
│   └── product_performance.sql
│
├── dashboard/
│   ├── pizza_sales_dashboard.xlsx
│   └── dashboard_screenshots/
│
├── documentation/
│   ├── data_dictionary.md
│   ├── analysis_methodology.md
│   └── business_recommendations.md
│
└── README.md
        </div>
    </div>

    <div class="section">
        <h2>🚀 Future Enhancements</h2>
        <div class="highlight">
            <ul>
                <li>Integration with real-time sales data</li>
                <li>Customer segmentation analysis</li>
                <li>Seasonal trend forecasting</li>
                <li>Profit margin analysis by product</li>
                <li>Geographic sales distribution mapping</li>
                <li>A/B testing framework for promotions</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2>🎓 Skills Demonstrated</h2>
        <table>
            <tr>
                <th>Technical Skills</th>
                <th>Analytical Skills</th>
            </tr>
            <tr>
                <td>
                    <ul>
                        <li>SQL Proficiency: Complex aggregations, date functions</li>
                        <li>Data Visualization: Dashboard design, chart selection</li>
                        <li>Business Intelligence: KPI identification, trend analysis</li>
                        <li>Excel Mastery: Advanced formulas, pivot tables</li>
                    </ul>
                </td>
                <td>
                    <ul>
                        <li>Pattern Recognition: Temporal and categorical trends</li>
                        <li>Business Acumen: Data to actionable recommendations</li>
                        <li>Problem Solving: Data quality and analysis challenges</li>
                        <li>Storytelling: Complex data in accessible formats</li>
                    </ul>
                </td>
            </tr>
        </table>
    </div>

    <div class="contact-section">
        <h2>📞 Contact & Collaboration</h2>
        <p><strong>Fatima Ezzahra Talibi</strong></p>
        <p>Business Intelligence and Analytics Intern</p>
        <div class="contact-links">
            <a href="mailto:Businesstalibi@gmail.com">📧 Email</a>
            <a href="https://www.linkedin.com/in/fati-talibi">💼 LinkedIn</a>
            <a href="tel:+1-309-350-7172">📱 Phone</a>
        </div>
        <p>📍 Rock Island, IL</p>
        <p><em>Open to collaborations, feedback, and opportunities in Business Intelligence and Data Analytics!</em></p>
    </div>

    <div class="tags">
        <span class="tag">#BusinessIntelligence</span>
        <span class="tag">#DataAnalysis</span>
        <span class="tag">#SQL</span>
        <span class="tag">#Excel</span>
        <span class="tag">#Dashboard</span>
        <span class="tag">#KPI</span>
        <span class="tag">#DataVisualization</span>
        <span class="tag">#BusinessAnalytics</span>
    </div>
</body>
</html>
