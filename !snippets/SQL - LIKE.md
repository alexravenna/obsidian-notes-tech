---
created: 2024-01-03T12:02:04Z
updated: 2024-12-10T08:33:15Z
tags:
  - search
  - snippet
  - sql
---
# Description
- Search for a specified pattern in a column
- [[SQL Wildcards]] can be used
- Without wildcards only exact matches are returned
# Example with wildcard
```sql
SELECT *
FROM Customers  
WHERE CustomerName LIKE 'a%';
```