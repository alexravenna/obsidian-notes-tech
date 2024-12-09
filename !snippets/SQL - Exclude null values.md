- Use `IS NOT NULL`
  ```sql
  SELECT CustomerName, ContactName, Address  
FROM Customers  
WHERE Address IS NOT NULL;
```