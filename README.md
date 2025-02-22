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

👉🏻 Insert a screenshot of table schema 

Table 2: PurchaseOrderDetail
- Size: 11 columns and 8845 rows
- Description: Recording detailed information related to Purchase order   

👉🏻 Insert a screenshot of table schema 

Table 3: PurchaseOrderHeader
- Size: 13 columns and 4012 rows
- Description: Recording information related to Purchase order

👉🏻 Insert a screenshot of table schema 

Table 4: ShipMethod
- Size: 6 columns and 5 rows
- Description: Categorize shipping methods

👉🏻 Insert a screenshot of table schema

Table 5: Vendor
- Size: 8 columns and 104 rows
- Description: Saving vendor information

👉🏻 Insert a screenshot of table schema


#### 3️⃣ Data Relationships:  
To standardize data, I create an additional tables called "Dim_date", "Dim_StatusName" and based on data of each table, I use Snowflake Schema to execute data modeling

👉🏻 Include a screenshot of Data Modeling to visualize relationships.  

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashhboard 01: Procurement Overview

👉🏻 Insert Power BI dashboard screenshots here  

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

👉🏻 Insert Power BI dashboard screenshots here

📌 Insight:
- Fulfillment rates have significantly improved since 2013, indicating that vendors are more capable of meeting supply demands.
- Some vendors (e.g., SUPERSALES INC.) receive a high number of orders but maintain a low fulfillment rate, which can negatively impact production efficiency and supply chain stability.

✅ Recommendation:
- Diversify supplier base: Instead of relying on vendors with low fulfillment rates, find and onboard additional suppliers with higher reliability.
- Implement vendor performance tracking: Regularly assess supplier fulfillment rates and adjust procurement strategies accordingly.
- Negotiate service-level agreements (SLAs) to ensure better compliance with delivery commitments.

#### 3️⃣ Dashhboard 03: Product Quality of Vendors

👉🏻 Insert Power BI dashboard screenshots here  

📌 Insight:
Despite the rapid increase in purchase order quantity, defect rates have significantly decreased in 2013 and 2014. This suggests that vendor product quality has improved, and procurement processes (vendor screening, filtering, and evaluation) are more effective.

✅ Recommendation:
- Strengthen partnerships with high-performing vendors who consistently deliver high-quality products.
- Reduce dependency on low-performing vendors with high defect rates while investigating the root causes of quality issues.
- Implement stricter quality control measures before finalizing purchase orders to maintain consistent product standards.