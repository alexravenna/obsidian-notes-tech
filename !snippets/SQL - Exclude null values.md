---
created: 2024-04-19T04:18:34Z
updated: 2024-12-10T08:33:15Z
---
- Use `IS NOT NULL`
  ```sql
  SELECT CustomerName, ContactName, Address  
FROM Customers  
WHERE Address IS NOT NULL;
```