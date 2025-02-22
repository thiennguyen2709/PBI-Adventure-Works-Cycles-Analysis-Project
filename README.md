# 📊 Power BI - Global Superstore Sales Project  
Author: Nguyen Duc Thien  
Date: 2024-11-11  
Tools Used: Power BI 

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)   
3. [📊 Key Insights & Visualizations](#-key-insights--visualizations)

---

## 📌 Background & Overview  

### Objective:
### 📖 What is this project about? 
 
AdventureWorks database supports standard online transaction processing scenarios for a fictitious bicycle manufacturer - Adventure Works Cycles. Scenarios include Manufacturing, Sales, Purchasing, Product Management, Contact Management, and Human Resources. In a manufacturing company, purchasing is one of the most important processes that require high-quality and on-time delivery so Purchase Manager always wants to control it real-time and continuously.

###  ❓Business Questions:  
1. How is the purchasing performance of company?
2. How is order fulfillment of Vendors?
3. How is product quality of Vendors?

### 🎯Project Outcome:  
✅ Purchasing performance and trends: Purchase order quantity and value increased significantly, especially in 2013 and 2014
✅ Fulfillment control: The fulfillment rates have significantly improved since 2013
✅ Product quality control: The defect rates have significantly decreased in 2013 and 2014

---

## 📂 Dataset Description & Data Structure

### 📊 Data Source, Data Structure & Relationships  

#### 1️⃣ Tables Used:
- Data source: GoogleBigQuery\adventureworks2019.Purchasing
- Number of data tables: 5 tables

#### 2️⃣ Table Schema & Data Snapshot  

Table 1: ProductVendor
- Size: 11 columns and 460 rows
- Description: Saving vendor ID and product ID respectively  

![image](https://github.com/user-attachments/assets/3baadc48-e1f5-44b6-ba42-eddb84f15812)
![image](https://github.com/user-attachments/assets/bdad185e-1893-422f-b057-8258ad976e24)

Table 2: PurchaseOrderDetail
- Size: 11 columns and 8845 rows
- Description: Recording detailed information related to Purchase order   

![image](https://github.com/user-attachments/assets/f0680abb-e39c-4631-b60c-26ff8700b57c)
![image](https://github.com/user-attachments/assets/7966cf4f-3aa5-44a9-af23-8e34b217c50d)

Table 3: PurchaseOrderHeader
- Size: 13 columns and 4012 rows
- Description: Recording information related to Purchase order

![image](https://github.com/user-attachments/assets/be9aa25e-480b-42dc-9452-9f2c866b0314)
![image](https://github.com/user-attachments/assets/1cc682d9-7fa1-4e54-98f8-85c075f6220e)

Table 4: ShipMethod
- Size: 6 columns and 5 rows
- Description: Categorize shipping methods

![image](https://github.com/user-attachments/assets/9d82c80b-741c-45a7-92f0-1f9ac4ed1c2b)

Table 5: Vendor
- Size: 8 columns and 104 rows
- Description: Saving vendor information

![image](https://github.com/user-attachments/assets/11d4a11c-3d4d-41be-9b69-dfb99499764b)

#### 3️⃣ Data Relationships:  
To standardize data, I create an additional tables called "Dim_date", "Dim_StatusName" and based on data of each table, I use Snowflake Schema to execute data modeling

![image](https://github.com/user-attachments/assets/60c1f09b-52c3-465c-8ec5-e9707c255521)

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashhboard 01: Procurement Overview

![image](https://github.com/user-attachments/assets/8e7cceb7-fcfb-40a3-b173-1746cb972ddb)

📌 Insight:
- Purchase order quantity and value increased significantly, especially in 2013 and 2014.
- The average purchase order quantity is approximately 600,000 units.
- The average purchase value is around $16,000,000.
-> This indicates that sales and production have also grown rapidly.

✅ Recommendation:
- Monitor procurement trends to anticipate future demand and ensure supply chain stability.
- Optimize inventory management to avoid overstocking or shortages during high-growth periods.
- Negotiate better contracts with suppliers to accommodate increased purchase volumes and secure cost reductions.

#### 2️⃣ Dashhboard 02: Order Fulfillment of Vendors

![image](https://github.com/user-attachments/assets/0b1849cb-2376-4404-a733-83f14b24d915)

📌 Insight:
- Fulfillment rates have significantly improved since 2013, indicating that vendors are more capable of meeting supply demands.
- Some vendors (e.g., SUPERSALES INC.) receive a high number of orders but maintain a low fulfillment rate, which can negatively impact production efficiency and supply chain stability.

✅ Recommendation:
- Diversify supplier base: Instead of relying on vendors with low fulfillment rates, find and onboard additional suppliers with higher reliability.
- Implement vendor performance tracking: Regularly assess supplier fulfillment rates and adjust procurement strategies accordingly.
- Negotiate service-level agreements (SLAs) to ensure better compliance with delivery commitments.

#### 3️⃣ Dashhboard 03: Product Quality of Vendors

![image](https://github.com/user-attachments/assets/1a4dcdec-cd4e-45e5-b7c1-2ecc281e279f)

📌 Insight:
Despite the rapid increase in purchase order quantity, defect rates have significantly decreased in 2013 and 2014. This suggests that vendor product quality has improved, and procurement processes (vendor screening, filtering, and evaluation) are more effective.

✅ Recommendation:
- Strengthen partnerships with high-performing vendors who consistently deliver high-quality products.
- Reduce dependency on low-performing vendors with high defect rates while investigating the root causes of quality issues.
- Implement stricter quality control measures before finalizing purchase orders to maintain consistent product standards.
