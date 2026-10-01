Online Retail Dataset II audit

#Data cleaning steps
I used pandas in Python to clean the dataset and to test it for customer revenue.

I used isnull() to identify missing and null values in the dataset. 

The 'Description' column contained 2928 null values and the 'Customer ID' column contained 107,927 null values.

I then dropped all rows with null values to perform accurate aggregations with the data.

Next, I dropped all orders with a quantity less than 0, or in other words, invalid, thus dropping all cancelled and invalid orders so the dataset is ready to work with.

#Analysis
I create a revenue column by multiplying 'Price' and 'Quantity' columns.

I group the customers by total revenue and sort descending to find the top customers in terms of revenue.

Then I identify the cumulative sum of the revenue of the top 10 customers to discover how significant a small portion of customers impacts the revenue
