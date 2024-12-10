---
created: 2024-04-19T04:09:04Z
updated: 2024-12-10T08:33:15Z
tags:
  - dotnet
  - snippet
  - uri
resources:
  - https://learn.microsoft.com/en-us/dotnet/api/system.uri.-ctor
  - https://learn.microsoft.com/en-us/dotnet/api/system.urikind
---

When creating a `Uri` with the [Uri(Uri, Uri) constructor](https://learn.microsoft.com/en-us/dotnet/api/system.uri.-ctor?view=net-8.0#system-uri-ctor(system-uri-system-uri), the first `Uri` has to be of the kind `UriKind.Absolute` and the second `Uri` has to be of the kind `UriKind.Relative`