---
created: 2023-12-18T13:40:18Z
updated: 2024-12-10T08:34:59Z
aliases:
  - NSB
tags:
  - bus
  - pub-sub
  - service-bus
homepage:
  - https://particular.net/nservicebus
github: https://github.com/Particular/NServiceBus
documentation:
  - https://docs.particular.net/nservicebus/
---
# Description

# Outbox
- Docs: [Outbox • NServiceBus • Particular Docs](https://docs.particular.net/nservicebus/outbox/)
- A feature to enable distributed transactions and avoid [[zombie records]] and [[ghost messages]]
- Simulates an [[atomic]] [[transaction]]
- Message handlers don't have to be [[idempotent]] because the outbox ensures consistency
- Basically, incoming messages are kept in an outbox before acknowledgement of their receipt is sent
- #caveat Requires persistent storage
# Sagas
- A message-driven state machine
	- Basically a collection of message handlers with a persisted shared state
- Useful when a process relies on more than one message
- Often called "policies": implementing [[class|classes]] are suffixed with `Policy`
- Saga data is often implemented as a nested class inside the saga definition
# Recoverability
- Docs: [Recoverability • NServiceBus • Particular Docs](https://docs.particular.net/nservicebus/recoverability/)
- Two types of automatic retries offered:
	- immediate (default: 5)
	- delayed (default: after 10 seconds, after 20 seconds, after 30 seconds)
- These defaults lead to a maximum possible amount of retries of 24
- Automatic [[rate limiting]] can be configured for multiple consecutive failing messages at an endpoint
	- affects the entire endpoint, not just one message type processed by the endpoint
- When messages reach the maximum number of allowed retries, the failing message is moved to the [[error queue]]
- Unrecoverable exceptions can be defined
	- Default: only `MessageDeserializationException`