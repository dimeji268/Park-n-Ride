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
Data Cleaning and Exploratory Skills were deployed in cleaning up the Data and to normalized/Standardized for missing values.Also two additional relationships were created using the Knowledge of Joining base on Primary and Foreign Key relationship of the Tables.

## Data Transformation/Modelling:
Rows with missing values and wrong entry were identified. For example, in the Reseller and Customer Table, missing values were Normalized and Standardized in line with other entries in the respective Tables.

In the ResellerID Column,a row with value of [Not Applicable] was normalized to AW00000000 and other Columns and rows with [Not Applicable] were normalized to “Direct Order” to reflect that the Reseller is an **Online Merchant** with a Virtual Address.

Reseller_dirty          |     Reseller_clean
:-----------------------|-----------------------:
![](Reseller_dirty.png) | ![](Reseller_clean.png)


