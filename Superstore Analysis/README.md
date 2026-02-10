##   Introduction 
This project analyzes a sales dataset obtained from Kaggle, containing detailed transactional information for customers and products. 
The dataset includes customer demographics, order details, product categories, sales, discounts, and profit data.  

The objective of this project is to explore, visualize, and analyze the sales patterns to uncover insights such as:

1. Customer buying behavior across different segments and regions

2. Product performance by category and sub-category

3. Sales trends over time

4. Profitability analysis and impact of discounts

The analysis can help businesses optimize sales strategies, improve customer targeting and maximize profits.

## Business Problems
1. How can the company optimize its discount strategy to increase sales without compromising profitability?
2. 


## Data 

The data is obtained from [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) website.
| Column Name | Description |
|-------------|-------------|
| Row ID|Unique ID for each row.|
|Order ID | Unique Order ID for each Customer.|
|Order Date | Order Date of the product.|
|Ship Date | Shipping Date of the Product.|
|Ship Mode| Shipping Mode specified by the Customer.|
|Customer ID | Unique ID to identify each Customer.|
|Customer Name | Name of the Customer.|
|Segment| The segment where the Customer belongs.|
|Country | Country of residence of the Customer.|
|City | City of residence of of the Customer.|
|State| State of residence of the Customer.|
|Postal Code | Postal Code of every Customer.|
|Region | Region where the Customer belong.|
|Product ID |Unique ID of the Product.|
|Category | Category of the product ordered.|
|Sub-Category | Sub-Category of the product ordered.|
|Product Name | Name of the Product|
|Sales | Sales of the Product.|
|Quantity | Quantity of the Product.|
|Discount | Discount provided.|
|Profit | Profit/Loss incurred.|


## Tools
1. KNIME (Data Cleaning and Transformation)
2. Power BI (Data Visualization)


## KNIME - Data Preparation and Cleaning 


<img width="2298" height="608" alt="image" src="https://github.com/user-attachments/assets/f8d798bc-29ab-47ac-9ea4-2ba1a4355f7b" />

1. Change the Date column from string to date data type.
2. Change the postal code into string data type.
3.Rounded the values into 2 decimal points.
4. Remove duplicate and check any missing values.
5. Split the OrderID and ProductID for more clarity, avoid confusion and easier to read.
6. Remove any columns that are not important.
7. Renaming columns into appropriate names.
8. Set a rule engine to classift the discounts rate into 4 category.  
   1 -> 0 - 0.2  
   2 -> 0.2 - 0.4  
   3 -> 0.4 - 0.6  
   4 -> 0.6 - 0.8  



## Dashboard PowerBi
<img width="3014" height="1696" alt="image" src="https://github.com/user-attachments/assets/2b4af41d-f6fe-450a-89ed-534ee95e6b6f" />




## Conclusion



























