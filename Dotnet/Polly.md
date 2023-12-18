---
tags:
  - dotnet
  - library
  - resilience
  - NETFoundation
documentation:
  - https://www.pollydocs.org/index.html
homepage:
  - https://www.thepollyproject.org/
---
# About
- A [[.NET]] library for implementing resilience strategies

# Resilience Strategies
## Reactive

### Retry
- Use automatic retries to get around sporadic, self-correcting faults
### Circuit Breaker
- Executions are blocked for a period when the number of faults exceeds a threshold
### Fallback
- Use an alternative action or return value if a fault occurs
### Hedging
- Execute parallel actions if the system is slow and wait for the fastest one
## Proactive
### Timeout
- Configure a certain time period to wait after which it's unlikely the call will be successful. This limits the amount of time that the caller will have to wait.
### Rate Limiter
- Control the load on the system by limiting the rate of executions

