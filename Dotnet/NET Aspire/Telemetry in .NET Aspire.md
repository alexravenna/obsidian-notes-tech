---
created: 2024-10-18T06:29:41Z
updated: 2024-12-10T08:35:00Z
documentation:
  - https://learn.microsoft.com/en-us/dotnet/aspire/fundamentals/telemetry
training:
  - https://learn.microsoft.com/en-us/training/modules/use-telemetry-dotnet-aspire/
---
# Description
- Is configured in the [[ServiceDefaults]] [[project]]:
	- `ConfigureOpenTelemetry()`
	- `AddOpenTelemetryExporters()`
	- `AddBuiltInMeters()`
- Common export destinations:
	- [[Aspire dashboard]]
	- [[Application Performance Management|APM]] tools like [[Prometheus]] or [[Grafana]]
	- [[Application Insights]]