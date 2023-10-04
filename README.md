# Business_360_Power_BI
Welcome to the AtliQ Hardware Data Analytics project repository! In this project, we have implemented data analytics using Power BI to empower AtliQ Hardware with the ability to make data-driven decisions, surpass competitors in the market, and drive growth in various aspects of their business, including finance, sales, marketing, and supply chain management.

Project Overview:	

AtliQ Hardware specializes in manufacturing and distributing a wide range of hardware products including PCs , mouse, printers, and more through various channels/ mediums i.e. direct, retail and distributor. 
It's customers spans across the globe and includes renowned companies like Amazon, Croma, Neptune, Staples, and Walmart.

AtliQ Hardware is currently facing some challenges in Latin America, where they operate their business. Until now, they've been making important decisions based on surveys and instincts.
However, as the company has grown, they've started collecting more data. They've realized that this data can be incredibly valuable for making better decisions. To make sense of this data, they've decided to hire a Data Analyst. 

The management believes that by analyzing this information, they can make smarter and more accurate choices to improve their business in Latin America. Essentially, they want the Data Analyst to help them turn this wealth of data into actionable insights, ultimately improving their business operations in the region.


Tech stacks :

1. SQL

2. PowerBi Desktop

3. Excel

4. DAX language

5. DAX studio (for optimizing the report) 


Learnings :

1. What questions should be asked before staring the project 

2. Creating calculated columns
 
3. creating measure using DAX language
 
4. Data modeling
 
6. Using Bookmarks to switch between two visuals
   
8. Page navigation with buttons

9. Using divide function to prevent zero division errors

10. creating date table using m language
 
11. Using KPI indicators
 
12. Conditional formatting the values in visuals using icons or background color

13. Data validation techniques

14. PowerBi services

15. Publishing reports to PowerBi services

16. Setting up personal gateway to set up the auto refresh of data 

17. Collaboration, workspace, access permissions in PowerBi services and more.


Business related terms :

1. Gross price 

2. Pre-invoice deductions 

3. Post-Invoice deductions 

4. Net Invoice sale 

5. Gross Margin 

6. Net sales 

7. Net profit 

8. COGC - cost of goods sold 

9. YTD - Year to Date 

10. YTG - Year to Go 

11. Direct channel

12. Retailer channel

13. Distributors channel

14. Consumer

Lets kick off our project, but before starting the project it's important to understand all the what's and why's and all other questions 

Questions to ask before starting with dashboard :

  objective of building this PowerBi dashboard? 

  success of the project would be based on what criteria? 

  What's the dead-line of the project? 

  do the stakeholders expects pre-view before the actual release? 

  what are all fears the stakeholder have in terms of building this dashboard? 

  Who would be our audience/stakeholder and what role they play in the project success? 

  What can go wrong while building this project? 

  is there any inputs from stakeholders in terms of design and views of the dashboard? 

After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

Understanding data:

It's important to have a good understanding of available data.

available data as follow -

Dimension table : It contain the static data.

Fact table : It contain data about the transactions.

gdb041 DB: Tables stored in this database as follow:

--> dim_customer : 

It contains details of customers i.e 27 distinct markets(ex India, USA), 75 distinct customers, 2 types of platforms(E-commerse, Brick & Motors) , 3 channels (Retailer, Direct, Distributor)

--> dim_market 

This table stores market information 27 distinct market(ex India, Spain), 7 sub-zones, and 4 regions(APAC, EU, NAN, LaTAM) details

--> dim_product 

This tales contains product details such as Divisions (P & A, N & S), Categories, varients

--> fact_forecast_monthly 

This table is used to forecast the customer’s need in advance, which can help in Higher customer satisfaction, Reduced cost in warehouses for storage purpose.

--> fact_sales_monthly 

This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value. 


gdb056 DB :
Tables stored in this Database as follows: 

--> freight_cost 

This table has details of travel cost and other cost for each market with fiscal year 

--> gross_price 

Has the details of gross prices with product code 

--> manufacturing_cost 

Has the details of manufacturing cost with product code with year 

--> Pre_invoice_dedutions 

Has the details of pre invoice deductions percentage for each cutomer with year 

--> Post_invoice_deductions 

Post invoice deductions and other deductions details 


Importing data into PowerBi 

As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential 
