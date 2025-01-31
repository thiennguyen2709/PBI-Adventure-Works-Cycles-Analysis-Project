# Power BI - Adventure Works Cycles Analysis Project
### **I. Project Assumption**
AdventureWorks database supports standard online transaction processing scenarios for a fictitious bicycle manufacturer - Adventure Works Cycles. Scenarios include Manufacturing, Sales, Purchasing, Product Management, Contact Management, and Human Resources. As a data analyst, I need to explore, visualize data and based on it to find out insight and give recommendation for my Purchase Manager by using:
- Data set: adventureworks2019.Purchasing
- Data table: Including 3 data tables:
  + Orders (Fact table): Recording information related to Sales order
  + People (Dim table): Saving Salesperson and region information respectively
  + Returns (Dim table): Recording information related to Return sales order
- Tool: Power BI
### **II. Project Objectives**
Finding out insight of data set and give answers for 3 key questions:
1. How is the business performance of company?
2. Where are the potential markets?
3. Which products can be strategic?
### **III. Data Modeling and Visualization**
To standardize data, I create an additional table called "Dim_date" and based on data of each table, I used Star Schema to execute data modeling

![image](https://github.com/user-attachments/assets/df20de9b-1c24-4b09-9d34-dae0fd9a40f0)

Then, I visualize data via 3 dashboards which will solve 3 question as mentioned above respectively:

_**Dashhboard 01: Business Performance Overview**_

This dashboard provides detailed and visual insights related to business performance of company

![image](https://github.com/user-attachments/assets/9591f988-0237-4e77-8349-44f3ac4599ee)

_**Dashhboard 02: Market Analyst**_

This dashboard provides business information of company in each market or country

![image](https://github.com/user-attachments/assets/26d8a868-1547-44ea-8ebd-3eb5219f2b58)

_**Dashhboard 03: Product Analyst**_

This dashboard provides detailed business statistics of products such as profit margin, average ordered quantity growth rate year over year,...

![image](https://github.com/user-attachments/assets/07b8fef8-9b71-4e8e-8b04-c7d74a119ceb)

### **IV. Insight and Recommendation**
![image](https://github.com/user-attachments/assets/f693a2cc-e78f-4691-bd1e-665eb6ca1281)

### **V. Used technical skills**
_**1. Data Processing & Transformation**_
- Power Query (ETL - Extract, Transform, Load) such as removing duplicates and errors, converting column formats, creating new calculated columns, ...
- DAX (Data Analysis Expressions) such as creating dynamic calculations such as total sales, profit, and profit margin, building key measures, ...

_**2. Data Analysis**_
- Key Metrics & KPIs such as Revenue, profit, and sales volume by category & country, Customer segments generating the highest revenue, ...
- Trend Analysis such as Sales & Profit over time using time-series analysis, Year-over-Year (YoY) Growth Analysis, ...
- Profitability Analysis such as Identifying products with the highest profit margins, Comparing profit margins across markets & product categories, ...

_**3. Data Visualization**_
Power BI Dashboard such as Bar & Line Charts, Matrix Table, Slicers & Filters, ...

