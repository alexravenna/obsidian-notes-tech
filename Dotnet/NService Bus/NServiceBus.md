---
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