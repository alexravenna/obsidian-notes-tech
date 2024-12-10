---
created: 2023-11-17T13:16:18Z
updated: 2024-12-10T08:34:54Z
tags:
  - file
  - XML
resources:
  - https://learn.microsoft.com/en-us/visualstudio/msbuild/common-msbuild-project-items
---
- [[XML]] file that describes an [[MSBuild]] project
- `.csproj` for [[Csharp|C#]] projects, `.fproj`
# Private references
- Means that the reference should be copied to the output folder
- Corresponds to the `Copy Local` property in [[Visual Studio]]
- Snippet:
```xml
<Reference>
	<Private>True</Private
```
