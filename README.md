# SalesPerformanceAnalysisFor-a-RetailStore

### Objectives

 This project is aimed at analyzing the sales performance of a retail store. The data is explored to uncover key insights such as; 
 1. Top-selling products
 2. Regional performance
 3. Monthly sales trends

 ### Overview

The data analyzed for this report contains 6 distinct products;
- Hat
- Shoes
- Shirt
- Gloves
- Socks
- Jacket

These product are spread across the following regions;
- South
- East
- North
- West

### About Data

The data analyzed was provided by The Incubator Hub [Download Here](https://docs.google.com/spreadsheets/d/1wICM0no-Tro0hVhZwlUNi8u7bzkOnU-2kxRhH1T8GDA/edit?usp=sharing). The dataset contains sales transactions from the 4 different regions the store is located. The data originally contained 7 columns and 50001 rows, however, after cleaning the data we are left with 9922 rows and 11 columns.

| Column                  | Description                             | Data Type      |
| :---------------------- | :-------------------------------------- | :------------- |
| OrderID                 | Invoice of the sales made               | VARCHAR(30)    |
| CustomerID              | Customer that made the sales            | VARCHAR(30)    |
| Product                 | Product sold                            | VARCHAR(100)   |
| Region                  | Region at which sales were made         | VARCHAR(5)     |
| OrderDate               | The date on which the purchase was made | DATE           |
| Day                     | The day which the purchase was made     | VARCHAR(10)    |
| Month                   | The month which the purchase was made   | VARCHAR(10)    |
| Year                    | The year which the purchase was made    | INT            |
| quantity                | The amount of the product sold          | INT            |
| unit_price              | The price of each product               | INT            |
| Revenue                 | The amount paid by customer             | INT            |

### Tools Used 

- Google sheets for data cleaning, exploration and summarization.
- MS SQL Server for data querying.
- Tableau for data visualization.

### Key Questions

- Retrieve the total sales for each product category.
- Find the number of sales transactions in each region.
- Find the highest-selling product by total sales value.
- Calculate total revenue per product.
- Calculate monthly sales totals for the current year.
- Find the top 5 customers by total purchase amount.
- Calculate the percentage of total sales contributed by each region.
- Identify products with no sales in the last quarter.

### Data Cleaning and Preparation

- Identified and removed duplicates
- Checked for blank cells
- Ensured my data had clear headers
- Made the data consistent

### How New Columns were created

Order Day ............. ``` =TEXT(E2, "ddd") ```

Order Month ........... ``` =TEXT(E2, "mmm") ```

Order Year ............ ``` =TEXT(E2, "yyy") ```

Revenue ............... ``` =SUM(I2*J2) ```

### Exploratory Data Analysis

The data was explored to provide answers to the following questions;

- Avg sales per product

```  =AVERAGEIF(C2:C9922, "Hat", I2:I9922) ```

- Total revenue by region

 ``` =SUMIF(D2:D9922, "South", K2:K9922) ```

### Data Analysis

``` Select * From SalesData ```

See more [Here](https://github.com/Pelumi-Esther/SalesPerformanceAnalysisFor-a-RetailStore/blob/main/SQL_Queries)

### Data Visualization

![Dashboard 1](https://github.com/user-attachments/assets/e20b16bd-55f4-4e03-8902-e7c55ed85c3e)

### Insights

- South region sold the most quantity of products, while the West sold the least quantity of products, 24,298 and 11,400 respectively.
- Hat had the highest quantity sold, while Jacket had the least quantity sold.
- The South region made 927,820 in revenue making it the region with the highest revenue, while the West region made 300,345 in revenue making it the region with the lowest revenue.
- The product with the highest revenue is Shoes with 613,380 while Socks made the least revenue with 180,785.
- Most products were purchased on Sundays while Mondays experienced the lowest sales.

### Recommendation 

- Further investigation/research should be done to understand why the west has the least quantity of products sold and by extention the least revenue.
- Socks should be positioned within reach from the shoes section.
- Delivery services may be considered since customers may be busy to come to the store during weekdays.


 

  





 
