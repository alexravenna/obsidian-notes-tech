---
created: 2024-02-05T11:52:58Z
updated: 2024-12-10T08:33:20Z
tags:
  - aws
  - lambda
  - serverless
---
- AWS attempts to analyze when our functions are called to forecast/pre-allocate usage
- SnapStart for optimizing cold starts
	- A snapshot is created during the first execution and saved in order to be "restored" and used in subsequent executions
	- #caveat The length of the cold start should be reduced, but the billing duration may be increased
	- Has certain limitations (no [[ARM Architecture|ARM]])
- Provisioned Concurrency:
	- AWS keeps the lambda function alive (for more money)
- Reserved Concurrency
	- A max of 1000 lambda functions can be created per account
	- In order to make sure that priority lambdas are always executable, you can reserve instances for them
- Layers
	- Offer the ability to set up a base set of functionality upon which all (or just a set of) lambda functions shall run, e.g.
		- external dependencies
		- common services, e.g. creating a database connection
	- Help minimize the size of function build artifacts 