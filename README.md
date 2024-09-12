<h1 align="center">Sales Insights - Data Analysis using Tableau & SQL</h1>
About Project

Conducted a data analysis project for an India-based hardware company to enhance sales insights.
Created ETL mappings using SQL to clean and transform data, and designed a star schema data model in Tableau.
Developed a Tableau dashboard to visualize sales trends and provide actionable business insights.
Technologies Used

SQL
Tableau
Project - India-Based Hardware Company Sales Insights - Data Analysis performed on Tableau & SQL

Objective: Deliver a dashboard providing real-time sales insights to support decision-making and increase revenue.
Approach:
Purpose: Achieve actionable insights and automate data processes to save time.
Stakeholders: Sales Director, IT Team, Customer Service Team, Data & Analytics Team.
End Result: Automated dashboard offering up-to-date sales insights, improving decision-making and potentially increasing revenue by 7%.
Success Criteria: Effective dashboards, improved decision-making, and reduction in manual data gathering time.
Data Analysis Using SQL

Show all customer records: SELECT * FROM customers;
Show total number of customers: SELECT count(*) FROM customers;
Show transactions for Chennai market: SELECT * FROM transactions WHERE market_code='Mark001';
Show distinct product codes sold in Chennai: SELECT DISTINCT product_code FROM transactions WHERE market_code='Mark001';
Show transactions where currency is USD: SELECT * FROM transactions WHERE currency="USD";
Show transactions in 2020: SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date WHERE date.year=2020;
Show total revenue in 2020: SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date WHERE date.year=2020 AND transactions.currency IN ("INR", "USD");
Show total revenue in January 2020: SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date WHERE date.year=2020 AND date.month_name="January" AND transactions.currency IN ("INR", "USD");
Show total revenue in Chennai for 2020: SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date WHERE date.year=2020 AND transactions.market_code="Mark001";
Data Analysis Using Tableau

Tableau Public Dashboards: Revenue & Profit Analysis

Creating Star Schema in Tableau:

Tableau Dashboard - Revenue Analysis

Tableau Dashboard - Profit Analysis

