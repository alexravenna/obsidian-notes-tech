---
created: 2024-04-15T07:09:21Z
updated: 2024-12-10T13:15:53Z
tags:
  - binary
  - data-type
  - integer
  - t-sql
documentation:
  - https://learn.microsoft.com/en-us/sql/t-sql/data-types/bit-transact-sql
---
# Description
- An [[integer]] data type
- Used for storing [[boolean]] values: `"TRUE"` => 1 and `"FALSE"` => 0
- Possible values:
	- 1
	- 0
	- NULL
- [[SQL Server]] optimizes storage of bit columns: every group of up to 8 columns is stored as 1 [[byte]]