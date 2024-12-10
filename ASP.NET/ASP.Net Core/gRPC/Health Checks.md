---
created: 2024-08-21T13:49:33Z
updated: 2024-12-10T08:35:01Z
documentation:
  - https://learn.microsoft.com/en-us/aspnet/core/grpc/health-checks
---
```csharp
using GrpcServiceHC.Services;
using Microsoft.Extensions.Diagnostics.HealthChecks;

var builder = WebApplication.CreateBuilder(args);

builder.Services.AddGrpc();
builder.Services.AddGrpcHealthChecks()
                .AddCheck("Sample", () => HealthCheckResult.Healthy());

var app = builder.Build();

app.MapGrpcService<GreeterService>();
app.MapGrpcHealthChecksService();

// Code removed for brevity.
```