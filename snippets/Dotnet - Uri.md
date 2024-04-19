---
resources:
  - https://learn.microsoft.com/en-us/dotnet/api/system.urikind
  - https://learn.microsoft.com/en-us/dotnet/api/system.uri.-ctor
tags:
  - snippet
  - dotnet
  - uri
---

When creating a `Uri` with the [Uri(Uri, Uri) constructor](https://learn.microsoft.com/en-us/dotnet/api/system.uri.-ctor?view=net-8.0#system-uri-ctor(system-uri-system-uri), the first `Uri` has to be of the kind `UriKind.Absolute` and the second `Uri` has to be of the kind `UriKind.Relative`