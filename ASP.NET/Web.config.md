---
tags:
  - ASPNET
  - IIS
  - XML
  - file
resources:
  - https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/transform-webconfig
  - https://azuliadesigns.com/c-sharp-tutorials/ultimate-guide-webconfig-file/
documentation:
  - https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/web-config
---
- [[XML]] file for configuring [[ASP.NET]] web applications
- Can be "transformed" with an additional XML file to apply to other environments
	- Typically "Debug" and "Release" in ASP.NET projects, i.e. `Web.Release.config`
- The root tag is `<configuration>`