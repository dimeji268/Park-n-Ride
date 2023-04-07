# Park-n-Ride Analysis

## Introduction:
**Park ‘n’ Ride** is an assumed  Store that sells Bike and Accessories through Resellers, across Europe, North America and Pacifics. It also allows direct Online purchase by Customers directly from the Store. The Reseller Business types ranges from  Warehousing, Value Added, Direct Sales and Speciality Bike Shop.

![](Introduction_image.jpg)

## Problem Statement:
Over time, the Store decides to review its business model of using Reseller vis a vis direct online Order by Customers, as well as its Profitability over a Four (4) Years  Financial cycle. This information will help them to rejig their business model in order to enhance their profitability.It will also afford them an holistic view across the entire Region of Operations.

## DataSet:
The assumed Raw DataSet is the Excel Sales file of  AdentureWorks 2019 provided by Oyinbooke.It contains Seven (7) Tables,namely:
1. Sales Order Data
2. Sales Territory Data
3. Sales Data
4. Reseller Data
5. Date Data
6. Product Data
7. Customer Data

## Skills Demonstrated:
Data Cleaning and Exploratory Skills were deployed to identify Rows and Columns that require cleaning,normalizing/Standardizing.Also two additional relationships were created using the Knowledge of Joining base on Primary and Foreign Key relationship that exist in the Tables.

## Data Transformation/Modelling:
Rows with missing values and wrong entry were identified. For example, In the Reseller Table,ResellerID Column has a row with value of [Not Applicable].This was normalized to AW00000000.Other Columns and Rows with [Not Applicable] were normalized to “Direct Sales” to reflect that the Reseller is an **Online Merchant** with a Virtual Address.

Reseller_dirty          |     Reseller_clean
:-----------------------|-----------------------:
![](Reseller_dirty.png) | ![](Reseller_clean.png)

Also in the Customer Table, CustomerID Column has a row with value of [Not Applicable].This was normalized to AW00010000. Other Columns and Rows with [Not Applicable] were normalized to “Direct Sales” to reflect that the **Online Customer** i.e the Customer order or make the purchase Online with a Virtual Address.

Customerer_dirty          |     Customer_clean
:-----------------------|-----------------------:
![](Customer_dirty.png) | ![](Customer_clean.png)

Thereafter two  new Relationships were created on the Sales table.First by joining the Sales Table with the Customer Table using the CustomerIDKey Column.Secondly the Sales table was joined with the Date Table using the DateKey Column.The two joins were executed using the  Primary /Foreign Key relationship that exist on the respective Tables. Unwanted Columns were removed and the Clean Dataset(7 Tables) were loaded into PowerBI for analysis.

Model_before            |     Model_after
:-----------------------|-----------------------:
![](Model_before.png)   | ![](Model_after.png)

## Analysis and Visualization:

The Analysis was done in Four(4)  broad Headers and relevant insight were generated accordingly.The Headers are :

## 1. Customers :

![](Customers_image.jpg)

It analyses the Customer's Spending pattern,the Demography as well as the Yearly Order Trend. Eight (8) Insights were generated namely:
-  Number of Customers
-  Number of Order
-  Highest Spender
-  Lowest Spender
-  Customers spending by Country-Region
-  Number of Customer Order by Fiscal Year
-  Number of Customer Order by Fiscal Quarter
-  Customers spending by State Province Top(5)

![](Customer_dashboard.png)

## 2. Products:

![](Products_image.jpg)

It Analyses the Product range in terms of Price,Category and Sub Category. Five (5) Insights were created namely:
- Number of Products
- Cheapest Product
- Expensive Products
- Sales by Product Category
- Sales by Product Sub Category

![](Products_dashboard.png)

## 3.  Reseller:

![](Reseller_image1.jpg)

It Analyse the performance of the Resellers in their region of Operations and individual contribution to the Business for the Period under review.
Five (5) Insights were created namely:
- Number of Resellers
- Reseller Sales by Business Types
- Top(5) Reseller by Sales
- Top(5) Reseller Sales by State-Province
- Reseller Sales by Country-Region

![](Reseller_dashboard.png)

## 4. Management:

![](Management_image.jpg)

It gives an Insight to the Management on the overall outlook of the Business in terms of Profitability.Six (6) Insights were created namely:
- Profit
- Profit by Group
- Profit by Channel
- Profit by Country
- Income by Cost by Fiscal Year
- Profit by Fiscal Year

![](Management_dashboard.png)

## Report

The full Report of the Analysis is a Click away :point_right: (https://app.powerbi.com/view?r=eyJrIjoiNjM3YmZiOTMtNGJkNC00MzJjLWI2YjgtOTk1ZDllMWE3MWFiIiwidCI6IjJlYWMyZjE5LTE1MWUtNGQzOC05NGUzLTlkYzg0YjYxNGJkNyIsImMiOjZ9)

## Conclusion/Recommendation:

For the Period under review, **Park ‘n’ Ride** generated a whopping $13M in Profit with 96% of it coming through Internet Channel while 4% was through Resellers.
FY2020 was the Year with the Highest Income($51M) and Highest Profit($5.8M) which can be attributed to highest Volume of Order processed while FY2018 was the Least($23) and Profit($3).United States with over $4M generated the highest Profit while Canada with Slightly over $1M, generated the least.

The highest Selling Products by Category is Bike($95M) specifically Road Bikes Sub Category($44M).The Cheapest Product on the Shelf is $2.29 while the most Expensive is $35,800.From the Analysis,Customers tend to prefer Direct Online Purchase as this count for $29M of the Total Sale.The abysmal performance of the Resellers in terms of Sales in their area of Operations need further Analysis in order to undetsand the underlining reasons.

## Recommendation:
The recommendation is Park ‘n’ Ride should enhance the Online Order Process and take a comprehensive review of the over 700 Reseller on their books to understand their challenges in contributing to the bottom line of the business.Furthermore Customers that Ordered Online should be assigned a unique CustomerID and necessary information obtained rather then the  “Not Applicable” entries adopted in recording their Purchases.


