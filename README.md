# Power BI - Adventure Works Cycles Analysis Project
### **I. Project Assumption**
AdventureWorks database supports standard online transaction processing scenarios for a fictitious bicycle manufacturer - Adventure Works Cycles. Scenarios include Manufacturing, Sales, Purchasing, Product Management, Contact Management, and Human Resources. In a manufacturing company, purchasing is one of the most important processes that require high-quality and on-time delivery so Purchase Manager always wants to control it real-time and continuously. As a data analyst, I need to explore, create operation dashboard and based on it to present insight and give recommendation to my Purchase Manager by using:
- Data set: GoogleBigQuery\adventureworks2019.Purchasing
- Data table:
  + PurchaseOrderDetail (Fact table): Recording detailed information related to Purchase order
  + PurchaseOrderHeader (Fact table): Recording information related to Purchase order
  + ProductVendor (Dim table): Saving vendor ID and product ID respectively
  + ShipMethod (Dim table): Categorize shipping methods
  + Vendor (Dim table): Saving vendor information
- Tool: Power BI
### **II. Project Objectives**
Exploring and visualizing data via operation dashboard to answer 3 key questions:
1. How is the purchasing performance of company?
2. How is order fulfillment of Vendors?
3. How is product quality of vendors?
### **III. Data Modeling and Visualization**
To standardize data, I create an additional tables called "Dim_date", "Dim_StatusName" and based on data of each table, I use Snowflake Schema to execute data modeling

![image](https://github.com/user-attachments/assets/6f79c16c-8676-41d6-879f-ab8a92fa57c5)

Then, I visualize data via 3 dashboards which will solve 3 questions as mentioned above respectively:

_**Dashhboard 01: Procurement Overview**_

This dashboard provides general information related to purchasing performance of company

![image](https://github.com/user-attachments/assets/fb6d93e4-25fd-48f7-9d82-02a70cc08097)

_**Dashhboard 02: Order Fulfillment of Vendors**_

This dashboard focuses on purchase-order fulfilling performance of Vendors

![image](https://github.com/user-attachments/assets/90a084fb-16c5-448b-a368-09de416714ce)

_**Dashhboard 03: Product Quality of Vendors**_

This dashboard shows detailed information of purchased product quality such as Rejected quantity, Defect rate,...

![image](https://github.com/user-attachments/assets/840cfc03-3e45-4df6-8fe7-5d7b2fb4ac97)

### **IV. Insight and Recommendation**

![image](https://github.com/user-attachments/assets/cf13cbdb-ad92-43e9-bdfd-1cd60b51126e)

### **V. Used technical skills**
_**1. Data Extraction & Transformation (ETL)**_
- Data Source Connection: Connected to the AdventureWorks2019 database
- Power Query Editor: Cleaned and transformed raw data before loading it into the model.
- Merging & Appending Queries: Combined multiple tables from the Purchasing schema to create a comprehensive dataset.

_**2. Data Visualization & Dashboard Design**_
- KPI Cards: Displayed key indicators like Total Orders, Total Spend, Defect Rate, and Fulfillment Rate.
- Bar & Line Charts: Visualized trends and comparisons across different years.
