---
created: 2023-11-23T10:28:51Z
updated: 2025-04-11T16:23:18+02:00
aliases:
  - OTel
tags:
  - cncf-incubating
  - framework
  - observability
  - open-source
  - telemetry
  - vendor-neutral
resources:
  - https://opentelemetry.io/
  - https://opentelemetry.io/docs/
  - "[[OpenTelemetry Simplifying Hybrid Cloud Monitoring]]"
---
# Description
- [[Observability]] framework and toolkit
- Creates and manages telemetry data: [[Traces|traces]], [[Metrics|metrics]] and [[Logs|logs]]
	- Any data that is not a trace or metric is a log
- [[vendor-neutral|Vendor]]- and tool-agnostic
- A merger of OpenTracing and OpenCensus
- Can be instrumented through:
	- code - with [[API]]s and [[SDK]]s
	- zero-code
- Components:
	- [[OpenTelemetry Protocol]]
- Customized versions of components are called "distributions"