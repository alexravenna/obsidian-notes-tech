---
documentation:
  - https://learn.microsoft.com/en-us/ef/core/saving/cascade-delete
---
# Description
- Cascade delete allows data connected through [[primary key]]-[[foreign key]] relationships to be deleted
	- when the primary key entity (parent/principal) is deleted -> also delete foreign key entities (child/dependent)
	- when the relationship navigation is severed, i.e. the foreign key in the child entity is deleted -> the child entity itself would be deleted