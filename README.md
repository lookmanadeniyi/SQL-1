# SQL-works
##Write a query to return the 10 earliest orders in the orders table. Include the id, occurred_at, and total_amt_usd.
SELECT id,occurred_at,total_amt_usd
FROM orders
LIMIT 10;


##Write a query to return the top 5 orders in terms of the largest total_amt_usd. Include the id, account_id, and total_amt_usd.
SELECT id,occurred_at,total_amt_usd
FROM orders
ORDER BY total_amt_usd DESC
LIMIT 5;

Write a query to return the lowest 20 orders in terms of the smallest total_amt_usd. Include the id, account_id, and total_amt_usd.
SELECT id, account_id, total_amt_usd
FROM orders
ORDER BY total_amt_usd
LIMIT 20;
