Cookie Sales Performance Dashboard 

1. Project Overview

This project focuses on building an interactive Power BI dashboard to analyze cookie sales data. The dashboard provides insights into revenue, cost, customer behavior, and product performance using multiple datasets.

2. Project Objective

●	To analyze sales performance of different cookie types

●	To track revenue, cost, and profitability

●	To understand customer distribution and behavior

●	To build an interactive and visually appealing dashboard

●	To integrate Python visualization within Power BI

3. Business Requirement

The business wants to:
●	Identify top-performing cookie products

●	Monitor sales trends over time

●	Analyze customer distribution by location

●	Track key metrics like revenue, cost, and profit

●	Enable interactive filtering for better decision-making

4. Data Source

The project uses three datasets:
●	Orders dataset (transaction-level data)

●	Customers dataset (customer details)

●	Cookie Types dataset (product-level information)

5. Data Preparation and Cleaning

●	Removed inconsistencies using Trim and Clean functions

●	Verified correct data types (Date, Numeric fields)

●	Checked and handled missing values

●	Ensured consistent naming across tables

6. Data Modelling

A star schema model was created:
●	Orders table as the central fact table

●	Customers and Cookie Types as dimension tables

Relationships:

●	Customers[Customer ID] → Orders[Customer ID]

●	Cookie Types[Cookie Type] → Orders[Product]

Both relationships are One-to-Many with single-direction filtering.

7. Key DAX Measures

●	Total Revenue = SUM(Orders[Revenue])

●	Total Cost = SUM(Orders[Cost])

●	Profit = Total Revenue – Total Cost

●	Total Orders = COUNT(Orders[Order ID])

●	Avg Order Value = Total Revenue / Total Orders

8. Dashboard Development
    
 The dashboard includes:
●	KPI cards for Revenue, Cost, Orders, and Average Order Value

●	Bar chart showing revenue by cookie type

●	Line chart showing sales trends over time

●	Donut chart showing order distribution by city

●	Pie chart comparing revenue and cost

●	Python-based visual for custom analysis

Interactive slicers:

●	Cookie Type

●	City

9. Key Insights

●	Chocolate Chip is the highest revenue-generating product

●	Sales show fluctuations over time indicating demand variation

●	A few cities contribute significantly to total orders

●	Overall profit margin is strong

●	Some cookie types have lower performance and can be improved

10. Conclusion

      The dashboard successfully provides actionable insights into sales performance. It enables stakeholders to monitor business metrics, identify trends, and make data-driven decisions. The integration of Python enhances analytical capabilities beyond standard visuals.

11. Dashboard Screenshots

Index Page:
 <img width="1366" height="768" alt="Index" src="https://github.com/user-attachments/assets/1557beff-0ead-4069-bf5e-22f44bc50698" />

Overview Dashboard:
 <img width="1366" height="768" alt="Overview" src="https://github.com/user-attachments/assets/8b1b5659-7f88-4679-803a-0df14455ac47" />


