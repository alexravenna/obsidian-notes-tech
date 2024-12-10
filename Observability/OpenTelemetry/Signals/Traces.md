---
created: 2024-05-28T09:31:52Z
updated: 2024-12-10T08:34:56Z
aliases:
  - Distributed Traces
resources:
  - https://opentelemetry.io/docs/concepts/signals/traces/
---
# Description
- A record of all units of work needed to handle an individual request
- Records the paths taken by requests through a multi-service architecture
- Consist of one or more [[Spans|spans]] in a [[Directed Acyclic Graph|DAG]]