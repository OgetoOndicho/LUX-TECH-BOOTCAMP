# LUX-TECH-BOOTCAMP
## Introduction to SQL 101

 You are provided with a table called Sales, which contains the following columns:
- SaleID: A unique ID for each sale.
- ProductID: The ID of the product sold.
- CustomerID: The ID of the customer who made the purchase.
- SaleDate: The date the sale occurred.
- Amount: The amount of the sale.

Questions- Write SQL scripts that:

- Finds the total sales for each product.
```
SELECT ProductID, SUM(Amount) AS total sales;
  ```

- Calculates the total sales for each month.
```
SELECT 
    EXTRACT(YEAR FROM SaleDate) AS SaleYear, 
    EXTRACT(MONTH FROM SaleDate) AS SaleMonth, 
    SUM(Amount) AS TotalSales
FROM Sales
GROUP BY SaleYear, SaleMonth
ORDER BY SaleYear, SaleMonth;
```

- Identifies customers who made more than 5 purchases.
```
SELECT CustomerID, COUNT(SaleID) AS PurchaseCount
FROM Sales
GROUP BY CustomerID
HAVING COUNT(SaleID) > 5;
```

