This project involves creating a Power BI Dashboard to analyze and optimize Domino's Pizza sales. The dashboard provides insights into customer traffic trends, order patterns, revenue, and menu performance, helping to enhance staffing, inventory management, and marketing strategies.

Objectives:

Analyze customer traffic trends to identify peak hours for optimized staffing.
Determine the average number of pizzas per order and identify top-selling pizzas to inform inventory management and marketing.
Calculate total revenue and identify seasonal trends for better forecasting and budgeting.
Assess the popularity of various pizzas and identify underperforming items or opportunities for promotion to optimize the menu and increase sales.
Tools and Technology:

SQL: For extracting, manipulating, and analyzing sales data.
SQL Server: For managing the dataset and ensuring efficient data storage and retrieval.
Power BI: For creating interactive and visually appealing dashboards to present key insights.
Key Metrics Analyzed:

Total Revenue: SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;
Average Order Value: SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_order_Value FROM pizza_sales;
Total Pizzas Sold: SELECT SUM(quantity) AS Total_pizza_sold FROM pizza_sales;
Total Orders: SELECT COUNT(DISTINCT order_id) AS Total_Orders FROM pizza_sales;
Average Pizzas Per Order: SELECT CAST(CAST(SUM(quantity) AS DECIMAL(10,2)) / CAST(COUNT(DISTINCT order_id) AS DECIMAL(10,2)) AS DECIMAL(10,2)) AS Avg_Pizzas_per_order FROM pizza_sales;
Power BI Dashboard Features:

Daily and Monthly Trends: Visualize trends in total orders to identify peak periods.
Sales by Category and Size: Show percentage of sales by pizza category and size.
Top and Bottom Performers: Identify top and bottom 5 pizzas by revenue, quantity, and total orders.
Category Analysis: Total pizzas sold by category, focusing on specific months.
This dashboard provides valuable insights into Domino's Pizza sales, enabling better decision-making and strategic planning.
