# 📊 Power BI Dashboard – Real Estate Analytics
![REAL_ESTATE](https://github.com/user-attachments/assets/19cfc50f-735a-4541-9497-65487c19320f)

---

## 📁 Project Overview
This Power BI project provides an interactive analytics dashboard for real estate data.  
It helps users understand property distribution, owner performance, agent activity, location-wise patterns, and key business KPIs.

The dashboard includes cards, slicers, visual charts, and drill-down features for better decision-making.

---

## 🎯 Objectives
- To clean and transform raw real-estate dataset  
- To build meaningful relationships between tables  
- To create insightful KPIs and interactive visuals  
- To enable dynamic filtering using slicers  
- To generate a dashboard useful for management and reporting  

---

## 🗂 Dataset Information
| Field | Description |
|-------|-------------|
| Property_ID | Unique ID of each property |
| Owner_Name | Property owner details |
| Agent_ID | Assigned real estate agent |
| Location | State → City → Area hierarchy |
| Property_Type | Residential / Commercial |
| Price | Property selling price |
| Status | Available / Sold |
| Date | Registration / Listing Date |

*(Dataset cleaned & transformed using Power Query.)*

---

# 📊Dashboard

---

<img width="1320" height="747" alt="Real_Estate_Dashboard_1" src="https://github.com/user-attachments/assets/6937e20f-f340-4280-851b-79ac2e235169" />

---

<img width="1316" height="728" alt="Real_Estate_Dashboard_2" src="https://github.com/user-attachments/assets/2379d380-120f-4cce-9df7-e3cb9b9af2a5" />

---

<img width="1317" height="738" alt="Real_Estate_Dashboard_3" src="https://github.com/user-attachments/assets/48cb6afa-cd94-4609-b820-34ad6b84d978" />

---

<img width="1312" height="737" alt="Real_Estate_Dashboard_4" src="https://github.com/user-attachments/assets/5c15ead2-6f02-4b50-b5f3-c7f023b752af" />

---

<img width="1339" height="755" alt="Real_Estate_Dashboard_5" src="https://github.com/user-attachments/assets/22d20ec3-e85d-4167-aeee-89bc31b74157" />

---

<img width="1320" height="737" alt="Real_Estate_Dashboard_6" src="https://github.com/user-attachments/assets/c4eaf734-160d-48eb-81e3-b1567db76f8a" />

---

<img width="1325" height="736" alt="Real_Estate_Dashboard_7" src="https://github.com/user-attachments/assets/f684f9f9-67eb-472b-bc39-98d9df8f13c2" />

---

<img width="1318" height="742" alt="Real_Estate_Dashboard_8" src="https://github.com/user-attachments/assets/b7a6043a-0ec7-461d-99b3-2c1ef3570e9b" />

---

<img width="1315" height="735" alt="Real_Estate_Dashboard_9" src="https://github.com/user-attachments/assets/ecdfcee9-91bb-4816-9125-eabf74dcb793" />

---

<img width="1308" height="740" alt="Real_Estate_Dashboard_10" src="https://github.com/user-attachments/assets/0eed8edd-ec04-40e0-932d-51a46bf4880d" />

---

<img width="1316" height="742" alt="Real_Estate_Dashboard_11" src="https://github.com/user-attachments/assets/00b1525c-3817-407e-be9a-8c179a4179e9" />

---

<img width="1338" height="752" alt="Real_Estate_Dashboard_12" src="https://github.com/user-attachments/assets/8a82f145-a37c-4b19-9280-636e370b504c" />


---

## 🔧 Tools & Technologies Used
- **Power BI Desktop**
- **Power Query**
- **DAX (Data Analysis Expressions)**
- **Excel (data handling)**

---

## 🧹 Data Cleaning (Power Query Steps)
- Removed duplicates  
- Handling blanks/null values  
- Standardized text formats  
- Split columns (Location hierarchy)  
- Added conditional columns  
- Changed data types  
- Merged & appended queries  
- Created a Date Table  

---

## 🔗 Data Modeling
- Star Schema implemented  
- Fact Table: `Fact_Properties`  
- Dimension Tables:  
  - `Dim_Owner`  
  - `Dim_Agent`  
  - `Dim_Location`  
  - `Dim_Date`  
- Relationships: One-to-Many with active joins  
- Cross-filter: Single direction  

---


