---
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