---
created: 2024-01-03T11:59:29Z
updated: 2024-12-10T08:33:15Z
tags:
  - snippet
  - sort
  - sql
---
# Description
- Sort/order the result set
- Defaults to [[#ASC - Ascending]]

# ASC - Ascending
```sql
SELECT *
FROM Customers  
ORDER BY CustomerName ASC;
```

# DSC - Descending
```sql
SELECT *
FROM Customers  
ORDER BY CustomerName DSC;
```