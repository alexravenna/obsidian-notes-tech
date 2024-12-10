---
created: 2023-12-18T13:57:06Z
updated: 2024-12-10T08:34:59Z
tags:
  - queue
  - service-bus
documentation:
  - https://docs.particular.net/transports/learning/
---
- The Learning Transport simulates a queue by storing all message actions in the local file system
- It uses a `.learningtransport` as the storage location in the folder hierarchy and *should* create one if not present
- The storage location can also be manually configured:
```csharp
var transport = endpointConfiguration.UseTransport<LearningTransport>(); transport.StorageDirectory("PathToStoreTransportFiles");
```
- #caveat The manually configured storage location should not be committed to [[VCS]], but the default `.learningtransport` directory may be necessary for something like [[integration tests]], whereby committing the empty directory (with a [[gitkeep|.gitkeep]] file) will be necessary