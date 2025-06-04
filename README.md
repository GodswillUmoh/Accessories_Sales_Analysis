# Accessories_Sales_Analysis
This is a sales report for accessories products

---
## Contents

--
[Project Overview](#Project-Overview)  |  [Data Source](#Data-Source) | [Tools Used](#Tools-Used]) |  [Table Outlay](#Table-Outlay) | [Query Langaues (SQL)](#Query-Langaues-(SQL)) | [Visualization](#Visualization)

--

## Project Overview:
+ This project analyzes the sales of Accessories to uncover insights on sales distribution by various attributes such as Accessories, Bikes and Clothing, Using pivot tables, I explored metrics like total sales by Accessories and country, average income of buyers, gender distribution, and overall revenue. This analysis helps to understand the key factors driving sales in the dataset provided.


## Data Source: 
> www.kaggle.com/dataset

---

## Tools Used:
- Pivot Table / Charts
- PowerBI
- SQL

## Table Outlay: 
_First Three Columns_

| Date |	Customer ID	|Customer Age|	Age Group|	Customer Gender|	Country|	State	|Product Category	|Sub Category	|Product|	Frame Size|	Order Quantity|	Unit Cost	|Unit Price|	Cost|	Revenue|	Profit|
|-----|-----|-----|------|-----|-----|-----|------|-----|-----|-----|------|-----|-----|-----|------|------|
|26/11/2013|	11019|	19	|Youth (<25)|	M|	Canada|	British Columbia|	Accessories|	Bike Racks|	Hitch Rack| - 4-Bike|		8	|45	|120|	360	|950|	590|
|26/11/2015|	11019|	19|	Youth (<25)	|M	|Canada|	British Columbia|	Accessories|	Bike Racks|	Hitch Rack |- 4-Bike|		8|	45|	120	|360|	950	|590|

## Query Langaues (SQL):
> Some of the query languages to retrieve records are displayed here
```sql
SELECT * FROM accessories;
```
```sql
---Calculate Total Revenue by Country---
SELECT Country, SUM(Revenue) AS TotalRevenue
FROM accessories
GROUP BY Country
ORDER BY TotalRevenue DESC;
```

```sql
---Total sales Query sort by Model---
SELECT Sub Category, COUNT(Customer ID) AS TotalSales
FROM Accessories
GROUP BY Sub Category
ORDER BY TotalSales DESC;

```

```sql
---To Retrieve Minimum Price ---
SELECT Product Category, SUM(Price) AS TotalPrice
FROM Accessories
GROUP BY Product Category
ORDER BY TotalPrice ASC;
```
```sql
SELECT * FROM accessories;
```
---

## Visualization
### PowerBI Dashboard
[To view the Dashboard, Click Here](https://ibb.co/LzQbQYMW)


![Screenshot (401)](https://github.com/user-attachments/assets/3c015597-1a14-4ebc-b238-0f9970e7ccfa)








