# Task 1 Customers with top transactions :top:

The first step to begin with your analysis is to convert your data into a table and name them. To do this, first, go to the **Sales_fact** sheet in your workbook. Select all the data, go to the **Format** tab and click on **Convert to table**. Name the table as Sales_fact.

Do the same for **Category_dim** and **Geography_dim** sheets.

## ❓Question 1 
Calculate the sales for each transaction.

For this create a new column at the end named **Sales** where Sales = Quantity * Price.

_Enter the sales value for transaction ID “31245032” of product ID “10000338”._: ₹ 300

**Note: -** You have to filter two columns that is Trasaction_id and Product_id for values 31245032 and 10000338 respectively.

| Date       | Transaction_id | Customer_id | Product_id | Store_id |	Quantity | Price (INR) | Sales |
|------------|----------------|-------------|------------|----------|----------|-------------|-------|
| 2020/11/30 |    31245032    |  712345322  |  10000338  |  36002   |   3.00   |   100.00    | 	300  |

## ❓Question 2
Calculate the total sales for each Customer_id - Transaction_id combination.

For this create a new worksheet and name it **Sales_by_Customer_Transaction**.

Copy the Transaction_id and Customer_id columns simultaneously, and paste them into the new sheet.

Select this data and go to the **Data** tab and click on **Data clean-up >> Remove duplicates**. This way you get a unique combination of Transaction_id and Customer_id.

Create a new column **Total Sales**. 

Here, creating a _Table_ will be of great help. In cell C2 use the Function **=SUMIFS(sum_range, criteria_range1, criterion1, [criteria_range2, criterion2, ...])**.

_=SUMIFS(Sales_fact[Sales], Sales_fact[Transaction_id], A2, Sales_fact[Customer_id], B2)_

Here you can see the table name Sales_fact with its column name. This is called structured reference. This is very helpful for entering the range of values in a table from different or the same sheet.

_What is the customer_id for the highest sales?_: 712345388

# Task 2 Product sales from 18th till 15th December

