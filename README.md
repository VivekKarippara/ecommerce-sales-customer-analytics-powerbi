# ecommerce-sales-customer-analytics-powerbi

## **📊 Global E-Commerce Sales & Customer Analysis (Power BI)**

📖 **Project Overview**  
This project is an end-to-end data analysis and visualization solution built in Power BI for a global e-commerce dataset spanning 14 countries. The goal of this project is to analyze transactional data, evaluate sales manager performance against targets, understand regional purchasing behaviours, and uncover actionable insights to optimize marketing and supply chain strategies.

📂 **Dataset Details**  
The analysis is based on raw data provided in an Excel format, consisting of three main tables:
1. Customers Table
Contains demographic and segmentation data for registered users.
•	Customer ID: Unique identifier for each customer.
•	Customer Country: Operating regions (14 distinct countries).
•	Gender & Age: Demographic markers.
•	Category: Customer classification cohorts (A, B, C, D, E).
2. Orders Table
Contains transactional log data.
•	Order ID: Unique identifier for the transaction.
•	Customer ID: Foreign key linking to the Customers table.
•	Order Datetime: Timestamp of the order (GMT).
•	Order Source: Platform used for the transaction (App, Website, WhatsApp, Other).
•	Sales POC: Point of Contact handling the sale.
•	Order Value: Revenue generated per order (in ₹).
3. Sales Targets Table
Contains yearly performance benchmarks for the sales team.
•	Sales POC: The primary contact.
•	Sales Manager: The supervising manager.
•	Sales Team: Alpha, Beta, Gamma, Delta, Epsilon.
•	2023 Sales Target: Annual revenue goal.


🛠️ Data Modeling & Transformations
To ensure a clean and optimized relational model, the following data transformations were performed using Power Query:
•	Data Cleansing: Standardized data types (e.g., parsing Order Value to numeric, formatting dates).
•	Missing Value Imputation: Handled an isolated system bug on April 1st that resulted in null Order Source records by imputing the statistical mode to maintain data integrity without skewing the distribution.
•	Column Merging: Combined Sales Manager First Name and Sales Manager Last Name into a single Sales Manager column in the Sales Targets table to optimize model size.
•	Relationships
Customers[Customer ID] → Orders[Customer ID] 
Sales Targets[Sales POC] → Orders[Sales POC] 
Model Type
⭐ Star Schema

📈 Dashboard Features & Insights

🎯 Sales Target Analysis
Key Insights
•	Target achievement status of Sales POCs 
•	Sales Team target comparison 
•	Sales Manager performance analysis 
•	% Target completion by team & manager 
KPIs
•	Total Sales 
•	Total Target 
•	Achievement % 
•	Repeat Customer Rate 


Visuals Used
•	Donut Chart 
•	Ribbon Chart 
•	KPI Cards 
•	Clustered Bar Chart 
•	Matrix Table 
•	Column Chart

Insights
•	Countries with highest sales 
•	Highest average order value 
•	Best performing sales managers  
•	Order source preference by region 
•	Total Sales by Team
•	Revenue fluctuations 
•	Peak sales periods 
•	Repeat Customer Rate 
•	Age & gender segmentation 
•	Non-ordering customer percentage 
•	Most used order source across countries 

🛠️ Tools & Technologies
•	Power BI Desktop 
•	Power Query 
•	DAX 
•	Data Modeling 
•	Excel 



•	📌 Key Business Outcomes
•	✔ Identified high-performing sales teams
✔ Analyzed customer retention behaviour
✔ Detected geographic sales trends
✔ Evaluated sales target achievement
✔ Discovered customer segment opportunities
✔ Improved business storytelling through dashboards
•	________________________________________
•	📷 Dashboard Preview
•	Add dashboard screenshots here
•	Example:

⭐ If you liked this project, consider giving it a star!

