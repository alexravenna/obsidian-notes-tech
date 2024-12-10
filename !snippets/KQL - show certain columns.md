---
created: 2023-12-10T12:41:11Z
updated: 2024-12-10T08:33:15Z
tags:
  - KQL
  - snippet
---
- Use the `project` operator:
```kql
  StormEvents | project EventId, State, EventType
```
- Result columns are shown in the sequence stated in the query