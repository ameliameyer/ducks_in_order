# SQL: Query Grain and Joins

**Learning status:** Starter note — not assessed.

The *grain* of a table is what one row represents. Before joining, state the grain of both tables and the desired output.

## Example

A customer table has one row per customer. An order table has one row per order. Joining them creates one row per order for customers with orders.

```sql
SELECT C.CUSTOMERID, COALESCE(SUM(O.AMOUNT), 0) AS TOTAL_AMOUNT
FROM CUSTOMERS C
LEFT JOIN ORDERS O ON C.CUSTOMERID = O.CUSTOMERID
GROUP BY C.CUSTOMERID;
```

## Exercise

What happens to the sum of order amounts if you also join an order-items table with multiple items per order? How would you prevent duplication?
