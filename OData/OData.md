---
aliases:
  - Open Data Protocol
tags:
  - oasis
  - protocol
homepage:
  - https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=odata
  - https://www.odata.org/
documentation:
  - https://learn.microsoft.com/en-us/odata/
  - https://www.odata.org/documentation/
training:
  - https://www.odata.org/getting-started/advanced-tutorial/
  - https://www.odata.org/getting-started/basic-tutorial/
  - https://www.odata.org/getting-started/understand-odata-in-6-steps/
---
# Description
- An [[abstraction layer]] upon a [[REST|RESTful]] [[API]]
- OData metadata: [[machine-readable]] description of an API's data model
- The endpoint `/odata/$metadata` retrieves the service metadata
- Service metadata is described with [[CSDL]]
- Routing:
	- Supports:
		- parentheses-style keys: `~/Shapes(1)`
		- key-as-segment: `~/Shapes/1`
# Functions and Actions
- Actions:
	- operations that maybe have [[side effects]] upon invocation
	- invoked with [[POST]] [[HTTP request]]s
- Functions:
	- operations that must return data and must have no side effects
	- invoked with [[GET]] HTTP requests
- Both can be:
	- bound:
		- applied to a specific entity type, primitive type, complex type or collection
		- after one of the above: `GET ~/odata/Books/mostRecent()`
	- unbound:
		- invoked on the whole service
		- after the route prefix: `GET ~/odata/ReturnAllForKidsBooks`