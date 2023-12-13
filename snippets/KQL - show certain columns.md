---
tags:
  - snippet
  - KQL
---
- Use the `project` operator:
```kql
  StormEvents | project EventId, State, EventType
```
- Result columns are shown in the sequence stated in the query