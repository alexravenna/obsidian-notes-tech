---
tags:
  - ASPNET
  - file
  - IIS
  - XML
documentation:
  - https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/web-config
resources:
  - https://azuliadesigns.com/c-sharp-tutorials/ultimate-guide-webconfig-file/
  - https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/transform-webconfig
---
- [[XML]] file for configuring [[ASP.NET]] web applications
- Can be "transformed" with an additional XML file to apply to other environments
	- Typically "Debug" and "Release" in ASP.NET projects, i.e. `Web.Release.config`
- The root tag is `<configuration>`