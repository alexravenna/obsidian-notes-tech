---
aliases: 
resources:
  - https://learn.microsoft.com/en-us/azure/azure-monitor/app/configuration-with-applicationinsights-config
tags:
  - configuration
  - file
  - monitoring
---
- Created in project root folder
- Copied to `bin` folder upon compilation
# Telemetry Modules
- Each module collects specific type of data and uses the core API to send the data
# Telemetry Initializers
- Initializers set context properties sent along with every telemetry item
# Telemetry Processors
- Processors filter and modify each telemetry item before it's sent from the SDK to the portal