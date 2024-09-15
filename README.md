### Adventure_Sales_Analysis_Project

### Project Overview

- Project Name: Adventure Works Sales Trends
- Time Period: 2015–2017 (3 years)
- Objective: To analyze sales trends, product performance, and customer behaviors over time. This analysis will help Adventure Works develop strategies to 
   maximize their sales.- 
- Primary Table: AdventureWorks_Sale_Data — representing combined sales data for 2015, 2016, and 2017.

### Star Schema Structure
1. I am using Two Fact Tables(AdventureWorks_Sale_Data and AdventureWorks_Returns)
   
- AdventureWorks_Sale_Data:This fact table contains transactional sales data and links to the dimension tables through foreign keys

  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/sales_table.png?raw=true)

- AdventureWorks_Returns:This table tracks product returns associated with sales.

 2. Dimension Tables
    
- AdventureWorks_Customers:This dimension provides customer details linked to sales transactions.

- AdventureWorks_Products:This dimension describes products sold in the store.

- AdventureWorks_Product_Subcategories:This dimension categorizes products into subcategories.
   
- AdventureWorks_Product_Categories:This dimension classifies products into categories.

- AdventureWorks_Territories:This dimension provides geographic data related to sales.

## ETL Process
1.Data Source Integration:
- Data from three years (2015-2017) was combined using SQL UNION to create the main AdventureWorks_Sale_Data table.


2.Data Cleaning:
- 	Missing data was handled across all dimensions.
- 	Standardized formats for customer information such as birthdate and income.
- 	Consistency checks were performed for foreign key constraints, ensuring valid relationships between tables.

  ## ER Diagram for Sales Trend Analysis

  ## Conclusion
  
  This star schema design efficiently supports sales trend analysis, enabling querying across multiple dimensions such as products, customers, territories, 
  and time. The structure ensures easy maintenance, scalability, and high performance for analytical queries.
  


