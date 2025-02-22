---
created: 2024-02-23T13:33:47Z
updated: 2024-12-10T08:35:00Z
aliases:
  - EF Core
tags:
  - dotnet
  - open-source
  - orm
github: https://github.com/dotnet/efcore
documentation:
  - https://learn.microsoft.com/en-us/ef/core/
training:
  - https://learn.microsoft.com/en-us/training/modules/persist-data-ef-core/
  - https://www.entityframeworktutorial.net/
  - https://www.learnentityframeworkcore.com/
---
# Database Providers
- There are many databases that can be accessed through EF Core
- The providers created/maintained by the EF Core project (i.e. Microsoft) are:
	- [[SQL Server]]
	- [[SQLite]]
	- [[Azure Cosmos DB]]
	- An in-memory database
# Querying
- EF Core uses [[LINQ]] to query data from the database
- The representation translated from LINQ is cached
- This representation is translated to a database-specific query language by the database provider and then sent
- A LINQ query is only sent to a database when its results are consumed