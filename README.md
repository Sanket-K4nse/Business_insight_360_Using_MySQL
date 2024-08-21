# Business Insights with MySQL: Atliq Hardware Dataset

Welcome to the Atliq Hardware Business Insights project! This repository showcases how to harness the power of MySQL to generate comprehensive business reports and valuable insights from the Atliq Hardware dataset.

## Project Overview :

In this project, I've utilized MySQL to explore and analyze the Atliq Hardware dataset, focusing on deriving actionable business insights. The goal is to assist decision-makers by creating various reports that highlight key performance indicators, sales trends, customer behaviors, and inventory management. By leveraging SQL's querying and data manipulation capabilities, this project delivers a set of data-driven reports that can inform strategic decisions and optimize business operations.
Also created Views, Stored Procedures, Functions, Tables and Run queries using CTE all the works shown below in the screenshot.

## Key Features :

- **Sales Analysis:** Track sales performance over time, identify top-selling products, and evaluate regional sales trends.
 
- **Customer Insights:** Understand customer purchasing patterns, identify high-value customers, and segment the customer base for targeted marketing.
 
- **Inventory Management:** Monitor stock levels, identify slow-moving inventory, and optimize reorder points to ensure efficient supply chain management.
 
- **Profitability Reports:** Analyze profit margins across different product categories, regions, and time periods to maximize business profitability.
 
- **Custom Queries:** A collection of custom SQL queries tailored to extract meaningful insights from the dataset.


## Tools and Technologies :


- **MySQL:** For querying, data analysis, and report generation.
 
- **Atliq Hardware Dataset:** A rich dataset containing detailed records of sales, customers, products, and inventory.


## Snapshot of FUNCTIONS :

- **1. Create get_fiscal_year and get_fiscal_quarter function to call in a query**

![Screenshot 2024-08-21 221615](https://github.com/user-attachments/assets/33359114-17c9-4f77-9731-f364c6486176)
![Screenshot 2024-08-21 221626](https://github.com/user-attachments/assets/f94b9e2d-3f44-4bab-8826-bf1374bb8d3b)


## Snapshot of QUERIES AND RESULT :

- **1. GENERATE A REPORT BASED ON THESE BELOW COLUMNS
-- month
-- product name
-- variant
-- sold quantity
-- gross price per item
-- gross price total**

  
![Screenshot 2024-08-21 174710](https://github.com/user-attachments/assets/527d327f-e3ce-40aa-9a79-9fc2d76f477e)


![Screenshot 2024-08-21 174728](https://github.com/user-attachments/assets/5a124118-acdd-415f-ac89-e99d78f3399b)



- **2. Generate a yearly report for Croma India where there are two columns
-- DATE
-- Total Gross Sales amount In that CALEANDER_DATE from Croma**
  
![Screenshot 2024-08-21 185258](https://github.com/user-attachments/assets/1eac0e09-8b0e-4842-a345-6c44ccf04aa4)
![Screenshot 2024-08-21 185309](https://github.com/user-attachments/assets/0143c64c-e1ca-42c1-9155-9c63f3e6be8b)


- **3. Generate a yearly report for Croma India where there are two columns
-- Fiscal Year
-- Total Gross Sales amount In that year from Croma**


![Screenshot 2024-08-21 185907](https://github.com/user-attachments/assets/9333d7e4-cf75-4a9b-9529-45a4e2bdcb0b)
![Screenshot 2024-08-21 185854](https://github.com/user-attachments/assets/5fb97247-5856-4c90-82e1-6b8a2882c14d)


- **4. Find gross sales for fact sales monthly**

![Screenshot 2024-08-21 191116](https://github.com/user-attachments/assets/0abf85b9-9083-4e55-893b-101424918b7c)
![Screenshot 2024-08-21 191124](https://github.com/user-attachments/assets/6c5de212-4771-43de-bb6b-62069ad2dc96)


- **5. Find net sales % coontributiion per customer**

![Screenshot 2024-08-21 193858](https://github.com/user-attachments/assets/6f530963-2950-419e-a3d0-16b3af0a6128)


- **6. Find net sales % per region**

![Screenshot 2024-08-21 193912](https://github.com/user-attachments/assets/edbdedf8-a4da-47dc-bc3c-9d8192951d72)


- **7. Get top 3 products in each division by their quantity sold**

![Screenshot 2024-08-21 193922](https://github.com/user-attachments/assets/9bc39612-d0c1-434e-a284-b5291510f068)
![Screenshot 2024-08-21 193946](https://github.com/user-attachments/assets/49faf04f-a083-4d9f-ae25-f29de2b0b55d)


- **8. Retrieve the top 2 markets in every region by their gross sales amount in fy=2021**

![Screenshot 2024-08-21 194859](https://github.com/user-attachments/assets/fa89a260-a576-41ee-988a-040fe78b2950)


- **9. Using CTE calculate net error % and absolute error% and forecast_accuracy**

  
![Screenshot 2024-08-21 210108](https://github.com/user-attachments/assets/9d6a4a8d-568a-4112-bd4f-5fbc01573472)
![Screenshot 2024-08-21 210058](https://github.com/user-attachments/assets/86da7bf3-c52a-442c-93ea-209ae9f25257)


- **10. To see indexes**
 
![Screenshot 2024-08-21 213713](https://github.com/user-attachments/assets/6854e204-243d-45aa-887f-49d91a66dfe7)


- **11. How composite indexes works**


![Screenshot 2024-08-21 213823](https://github.com/user-attachments/assets/b7457483-0894-4831-b29f-4af4c1397bf2)


## Snapshot of Creating VIEWS :


- **1. Create a GROSS_SALES view to call it again in next query**

![Screenshot 2024-08-21 190601](https://github.com/user-attachments/assets/15d616f6-7bb6-47b1-98b8-2dc81f119296)
![Screenshot 2024-08-21 190617](https://github.com/user-attachments/assets/4c014ad3-ed73-4787-a58a-4c99e1f0734b)


- **2. Create a SALES_PREINV_DISCOUNT view using GROSS_SALES view to call it again in next query**

![Screenshot 2024-08-21 223421](https://github.com/user-attachments/assets/ab56f29f-a972-4bce-be2f-c0c59c0be5af)
![Screenshot 2024-08-21 223507](https://github.com/user-attachments/assets/5025410d-65e5-4a8c-a1ac-21dfc7bfa659)


- **3. Create a SALES_POSTINV_DISCOUNT view to call it again in next query**


![Screenshot 2024-08-21 223030](https://github.com/user-attachments/assets/b2a8c197-e55f-44c2-bbd7-ff2dbf270d1f)
![Screenshot 2024-08-21 223314](https://github.com/user-attachments/assets/51c0d976-5644-408f-bb2a-fc2174ae49d7)


- **4. Create a NET_SALES view to call it again in next query**

![Screenshot 2024-08-21 222803](https://github.com/user-attachments/assets/6e861d5f-19b1-4dc3-a3a6-1b90b2f22ce2)
![Screenshot 2024-08-21 222831](https://github.com/user-attachments/assets/d804f5c3-f87c-42f0-a52d-02871f82658e)


## Snapshot of Creating PROCEDURES :


- **1. create a stored procedure that can give you the market, fiscal year and market badge is like 
-- if sold quantity is graeter than 5m then it is gold else silver**
  
![Screenshot 2024-08-21 190146](https://github.com/user-attachments/assets/6d62270a-962d-445f-af7b-0c35f1e39ef6)
![Screenshot 2024-08-21 190129](https://github.com/user-attachments/assets/64f311b8-6b84-4c41-8664-7c7a1f1f047c)


- **2. create a stored procedure to get forecast_accuracy for a perticular year, input will be fiscal year**

![Screenshot 2024-08-21 224143](https://github.com/user-attachments/assets/6146accd-e70a-4eb9-b1ae-a1c4612d78c4)
![Screenshot 2024-08-21 224546](https://github.com/user-attachments/assets/c7119eed-3d47-44a0-8bab-73ff6e698c76)


- **3. create a stored procedure to get get_yearly_gross_sales_for_customer for a perticular year, input will be customer ID**

![Screenshot 2024-08-21 224848](https://github.com/user-attachments/assets/9c5a472b-d012-471e-ad1d-a5b704a8d68a)
![Screenshot 2024-08-21 224936](https://github.com/user-attachments/assets/149c6b8c-28e2-4aed-bde6-51331df44ad0)


- **4. create a stored procedure to GET TOP_N_CUSTOMER by NET_SALES for a perticular year, input will be fiscal_year, top n, market**

![Screenshot 2024-08-21 225113](https://github.com/user-attachments/assets/3d53dc2a-ade1-4377-95f9-9aabd3a1b5f9)
![Screenshot 2024-08-21 225616](https://github.com/user-attachments/assets/ff5de8d4-8bff-434b-bd94-b816bbd70698)


- **5. create a stored procedure to GET TOP_N_MARKET by NET_SALES for a perticular year, input will be fiscal_year, top n**

![Screenshot 2024-08-21 225716](https://github.com/user-attachments/assets/1cc6e075-94d1-49b3-af64-a0ac59196e92)
![Screenshot 2024-08-21 225903](https://github.com/user-attachments/assets/dc663ad9-7d51-4083-bae1-a523b88a10d8)


- **6. create a stored procedure to GET TOP_N_PRODUCT_PER_DIVISION by SOLD_QUANTITY for a perticular year, input will be fiscal_year, top n**

![Screenshot 2024-08-21 230136](https://github.com/user-attachments/assets/33552acf-a803-465e-946d-1bb2e490dea1)
![Screenshot 2024-08-21 230159](https://github.com/user-attachments/assets/08092e8c-334d-4ac3-adbf-0e7e666a9239)


## Snapshot of creating TABLE using QUERY :


- **1. Create a physical table fact_act_est with a existing table or query**


![Screenshot 2024-08-21 195952](https://github.com/user-attachments/assets/5666f44c-25fa-4b46-9e8a-072f84d12c1f)
![Screenshot 2024-08-21 195936](https://github.com/user-attachments/assets/ba15c3f2-867b-414e-ac55-36e158c75747)
