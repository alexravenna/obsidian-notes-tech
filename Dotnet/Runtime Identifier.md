---
created: 2024-05-21T08:36:49Z
updated: 2024-12-10T08:34:59Z
aliases:
  - RID
documentation:
  - https://learn.microsoft.com/en-us/dotnet/core/rid-catalog
---
- With .NET 8, a smaller RID graph was introduced
	- version-specific and [[distro]]-specific RIDs were removed in favor of using "portable" RIDs, e.g.:
		- `alpine-x64` -> `linux-musl-x64`
		- `win10-x64` -> `win-x64`
- A tool for visualizing RID graphs: https://github.com/0xced/RidGraph
- A list of all RIDs: [sdk/src/Layout/redist/PortableRuntimeIdentifierGraph.json at main · dotnet/sdk (github.com)](https://github.com/dotnet/sdk/blob/main/src/Layout/redist/PortableRuntimeIdentifierGraph.json)