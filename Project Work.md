# Task 1 Customers with top transactions :top:

The first step to begin with your analysis is to convert your data into a table and name them. To do this, first, go to the **Sales_fact** sheet in your workbook. Select all the data, go to the **Format** tab and click on **Convert to table**. Name the table as Sales_fact.

Do the same for **Category_dim** and **Geography_dim** sheets.

## ❓Question 1 
Calculate the sales for each transaction.

For this create a new column at the end named **Sales** where Sales = Quantity * Price.

_Enter the sales value for transaction ID “31245032” of product ID “10000338”._: ₹ 300

You have to filter two columns that is Trasaction_id and Product_id for values 31245032 and 10000338 respectively.

| Date       | Transaction_id | Customer_id | Product_id | Store_id |	Quantity | Price (INR) | Sales |
|------------|----------------|-------------|------------|----------|----------|-------------|-------|
| 2020/11/30 |    31245032    |  712345322  |  10000338  |  36002   |   3.00   |   100.00    | 	300  |

