# 🥤 Coca-Cola Sales Insights Dashboard (Power BI)

## 📊 Project Overview
This project presents an **interactive Power BI dashboard** analyzing Coca-Cola’s sales and profitability across regions, states, and beverage brands.  
It provides a comprehensive view of performance metrics such as **total sales, units sold, profit trends, and transaction distribution**, allowing stakeholders to make data-driven business decisions.  

---

## 🧾 Dataset Information
The dataset contains sales and operational data from Coca-Cola’s retail distribution network.

| Column Name | Description |
|--------------|-------------|
| Retailer | Retail partner (Amazon, Walmart, Target, etc.) |
| Retailer ID | Unique ID for each retailer |
| Invoice Date | Date of transaction |
| Region | U.S. region (Midwest, Northeast, South, Southeast, West) |
| State | State name |
| City | City name |
| Beverage Brand | Product name (Coca-Cola, Sprite, Fanta, etc.) |
| Price per Unit | Selling price per item |
| Units Sold | Quantity sold |
| Total Sales | Total revenue generated |
| Operating Profit | Profit after operating costs |
| Operating Margin | Profitability percentage |

---

## 🧮 Key KPIs and Visuals

| KPI / Visual | Description | Visual Type |
|---------------|--------------|--------------|
| **Total Units Sold by Beverage Brand** | Comparison of product performance by brand | Bar Chart |
| **Total Sales by Region** | Revenue breakdown by geographical region | Bar Chart |
| **% of Transactions by Region** | Proportion of sales transactions per region | Donut Chart |
| **Total Sales by State** | State-level performance view | Bar Chart |
| **Total Profit by Month** | Profitability trend over time | Line Chart |
| **Price per Product** | Current average price per unit | Card Visual |

---

## 🧰 Tools & Technologies

* Power BI Desktop – Data modeling & dashboard creation

* DAX (Data Analysis Expressions) – Calculations & measures

* Excel / CSV – Data source

* GitHub – Project documentation

## 🧃 Dynamic Brand Image Feature
A Beverage Brand URL column was created using DAX to dynamically display the brand image when selected in a slicer.
```DAX
Beverage Brand URL = 
SWITCH(
    'COCA COLA'[Beverage Brand],
    "Coca-Cola", "https://i.postimg.cc/7ht3D1sP/COKE.png",
    "Dasani water", "https://i.postimg.cc/9F8254c8/DASANI-WATER.jpg",
    "Diet Coke", "https://i.postimg.cc/bwRSx9P3/diet-coke-1.jpg",
    "Fanta", "https://i.postimg.cc/wxJv5QcX/Fanta.jpg",
    "Powerade", "https://i.postimg.cc/VNyZt1YN/Powerade.jpg",
    "Sprite", "https://i.postimg.cc/2yTgdt0G/Sprite.jpg",
    BLANK()
)
```



A Beverage Brand URL column was created using DAX to dynamically display the brand image when selected in a slicer.
## 📸 Dashboard Preview
 <img width="1665" height="857" alt="Image" src="https://github.com/user-attachments/assets/9e4d851a-9f8c-4f81-9a64-8f74c6ca3e7c" />

 
## Screen Recording
 https://github.com/AnalystKofi/COCA-COLA-ANALYSIS--POWER-BI/blob/main/coke%202025-10-25%2012-57-21.mp4

## 💡 Key Insights

* West Region achieved the highest sales and profit margins.

* Coca-Cola and Diet Coke are top-selling brands by units and revenue in both 2022 and 2023.

* Carlifonia  leads in number of transactions(total sales by state) in the year 2023, but in 2022 it was New york  .

* Monthly profit trends show consistent growth in peak seasons.

