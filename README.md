# 🛒 Retail Analysis Dashboard | Power BI Project

---

## 📌 Project Overview
This project analyzes **online retail sales data** to uncover insights about
revenue trends, top customers, and global sales distribution.
The dashboard helps business stakeholders understand monthly revenue patterns,
identify high-value customers, and track performance across countries.

---

## 🛠️ Tools & Technologies Used

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard building and data visualization |
| Power Query | Data cleaning and transformation |
| DAX | Calculated measures and revenue metrics |
| Excel (Online_Retail_Data_Set.xlsx) | Source dataset |

---

## 📊 Dataset Information

| Column | Description |
|---|---|
| InvoiceNo | Unique invoice number |
| StockCode | Product stock code |
| Description | Product description |
| Quantity | Number of units purchased |
| InvoiceDate | Date of transaction |
| UnitPrice | Price per unit |
| CustomerID | Unique customer identifier |
| Country | Country of the customer |
| Revenue | Total revenue (Quantity × UnitPrice) |

---

## 🔄 Project Workflow

### 1️⃣ Data Loading
- Loaded `Online_Retail_Data_Set.xlsx` into Power BI Desktop
- Previewed data structure, columns and data types

### 2️⃣ Data Cleaning (Power Query)
- Removed null values from CustomerID column
- Removed negative quantities (cancelled orders)
- Corrected data types for dates and numeric columns
- Filtered out United Kingdom from map visual
- Created **Month** column from InvoiceDate for trend analysis

### 3️⃣ DAX Measures Created
```
Revenue = Quantity * UnitPrice

Total Revenue = SUM(Revenue)

Total Quantity = SUM(Quantity)
```

### 4️⃣ Dashboard Building
Built a clean purple-themed **Retail Analysis Dashboard** with 4 key visuals

---

## 📊 Dashboard Overview

### 📈 Visuals Included

| Visual | Description |
|---|---|
| 📈 Revenue by Month | Line chart showing monthly revenue trend across the year |
| 📊 Quantity & Revenue by Country | Clustered bar chart comparing top 10 countries |
| 📊 Revenue by CustomerID | Bar chart showing top 10 customers by revenue |
| 🗺️ Total Units Sold by Country | World map showing global sales distribution |
<img width="1367" height="800" alt="Screenshot 2026-05-31 120453" src="https://github.com/user-attachments/assets/16a0544d-27df-4b98-9bff-2c23ed189aa5" />


---

## 💡 Key Business Insights

- 📈 **Revenue peaks in November** — likely driven by holiday season shopping
- 🌍 **Netherlands leads** in both quantity and revenue among international markets
- 👑 **Customer 14646** is the highest revenue generating customer
- 📉 **Revenue dips in April and August** — opportunity for targeted promotions
- 🗺️ **Europe dominates** global sales with strong presence across multiple countries
- 🔝 **Top 10 customers** contribute significantly to overall revenue — retention is critical

---
