---
resources:
  - https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview
  - https://learn.microsoft.com/en-us/azure/azure-monitor/app/opentelemetry-overview?tabs=aspnetcore
tags:
  - azure
  - telemetry
  - logging
---
# Description
- A feature of [[Azure Monitor]]
- Enables [[Application Performance Management]]
- Sends telemetry from a web application to the [[Azure]] portal
- Telemetry types/"pillars":
	- Distributed tracing
	- Metrics
	- Logs
- There are automatic and manual methods for enabling an app to send telemetry
- Data model:
	- Telemetry types automatically collected:
		- Requests - server requests
		- Exceptions
		- Dependencies - calls to external components
	- Types for custom telemetry (not automatically collected):
		- Traces - diagnostic logs
		- Events - user actions and other events
		- Metrics - performance measurements
- Integration possibilities:
	- Application Insights ASP.NET SDK
		- Configured by [[ApplicationInsights.config]]
- #caveat [[Redis]] dependencies must be manually configured, they aren't detected automatically
# Sampling
- Application Insights features three sampling methods:
	- Adaptive sampling (default)
		- telemetry volume is automatically adjusted
		- only available for [[ASP.NET]]/[[ASP.NET Core]] server-side telemetry and [[Azure Functions]]
	- Fixed-rate sampling
		- the rate of sampling is configured in the application
		- clients and servers synchronize their sampling
	- Ingestion sampling
		- is configured in the Azure Portal
		- the rate can be configured without redeploying
		- is mutually exclusive with adaptive and fixed-rate sampling
		- doesn't reduce telemetry sent, but can be useful to reduce Application Insights usage/costs
- Sampling can be configured in [[ApplicationInsights.config]]
# Optimizing
- Described here: [DevOps - Optimize Telemetry with Application Insights | Microsoft Learn](https://learn.microsoft.com/en-us/archive/msdn-magazine/2017/may/devops-optimize-telemetry-with-application-insights)