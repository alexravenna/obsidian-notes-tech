---
tags:
  - t-sql
  - data-type
  - integer
  - binary
documentation:
  - https://learn.microsoft.com/en-us/sql/t-sql/data-types/bit-transact-sql
---
- An [[integer]] data type
- Used for storing boolean values: `"TRUE"` => 1 and `"FALSE"` => 0
- Possible values:
	- 1
	- 0
	- NULL
- [[SQL Server]] optimizes storage of bit columns: every group of up to 8 columns is stored as 1 [[byte]]