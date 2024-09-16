### Adventure_Sales_Analysis_Project

### Project Overview

- Project Name: Adventure Works Sales Trends
- Time Period: 2015–2017 (3 years)
- Objective: To analyze sales trends, product performance, and customer behaviors over time. This analysis will help Adventure Works develop strategies to 
   maximize their sales.- 
- Primary Table: AdventureWorks_Sale_Data — representing combined sales data for 2015, 2016, and 2017.

### Star Schema Structure
### 1. Two Fact Tables(AdventureWorks_Sale_Data and AdventureWorks_Returns)
   
- AdventureWorks_Sale_Data:This fact table contains transactional sales data and links to the dimension tables through foreign keys

  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/sales_table.png?raw=true)

- AdventureWorks_Returns:This table tracks product returns associated with sales.

  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/returns.png?raw=true)

 ### 2. Dimension Tables
    
- AdventureWorks_Customers:This dimension provides customer details linked to sales transactions.
- 
  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/customers.png)
  
- AdventureWorks_Products:This dimension describes products sold in the store.

  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/Product_table.png?raw=true)
  
- AdventureWorks_Product_Subcategories:This dimension categorizes products into subcategories.
  
  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/Product_subcategory.png?raw=true)
    
- AdventureWorks_Product_Categories:This dimension classifies products into categories.
  
  ![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/Productcategory%20.png?raw=true)
  
- AdventureWorks_Territories:This dimension provides geographic data related to sales.
  
  ![](https://raw.githubusercontent.com/calua-83/Sales_Analysis_Project/f1dcb05ebab13e06a2c30dbcab19320fd56134b7/Area.png)
  
## ETL Process
1.Data Source Integration:
- Data from three years (2015-2017) was combined using SQL UNION to create the main AdventureWorks_Sale_Data table.

![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/ETL.png?raw=true)

2.Data Cleaning:
- 	Missing data was handled across all dimensions.
- 	Standardized formats for customer information such as birthdate and income.
- 	Consistency checks were performed for foreign key constraints, ensuring valid relationships between tables.

  ## ER Diagram for Sales Trend Analysis

![](https://github.com/calua-83/Sales_Analysis_Project/blob/main/Sales_Adventure_Works_ER.png)
  

  ## Conclusion
  
  This star schema design efficiently supports sales trend analysis, enabling querying across multiple dimensions such as products, customers, territories, 
  and time. The structure ensures easy maintenance, scalability, and high performance for analytical queries.
  


