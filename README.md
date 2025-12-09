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

## 📏 DAX Measures
```DAX
Total Properties = COUNT(Fact_Properties[Property_ID])

Total Sold = CALCULATE(
    COUNT(Fact_Properties[Property_ID]),
    Fact_Properties[Status] = "Sold"
)

Total Revenue = SUM(Fact_Properties[Price])

Sold % = DIVIDE([Total Sold], [Total Properties])
