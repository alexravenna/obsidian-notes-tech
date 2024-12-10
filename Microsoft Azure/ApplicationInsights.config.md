---
created: 2023-11-13T10:59:49Z
updated: 2024-12-10T08:34:58Z
aliases: []
tags:
  - configuration
  - file
  - monitoring
resources:
  - https://learn.microsoft.com/en-us/azure/azure-monitor/app/configuration-with-applicationinsights-config
---
- Created in project root folder
- Copied to `bin` folder upon compilation
# Telemetry Modules
- Each module collects specific type of data and uses the core API to send the data
# Telemetry Initializers
- Initializers set context properties sent along with every telemetry item
# Telemetry Processors
- Processors filter and modify each telemetry item before it's sent from the SDK to the portal