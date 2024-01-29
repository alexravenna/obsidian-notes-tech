---
aliases:
  - DDD
---
# Modelling
- Build a model from domain knowledge
- Collaborative modeling:
	- Domain expert works with developer
	- "knowledge crunching" to get the essential knowledge out of the domain
		- Methods:
			- [[Event Storming]]
			- [[Domain Storytelling]]
	- Direct communication necessary and with a common language
	- Find out the "unknown knowns" - knowledge from domain experts that they think is obvious
	- Results in a [[Ubiquitous language|ubiquitous language]] for each domain
# Building Blocks/Vocabulary
- Entities
	- Implemented as classes
- Value objects
	- Properties of entities
- Domain events
	- Show that something has happened in the system
- [[Bounded Context]]
	- Context mapping
		- Determining the relationships between the different contexts
- Domain service
# Architecture
- Four layers:
	- User Interface
		- Receives input and user commands and presents information
	- Application (a.k.a. Service Layer)
		- Describes and coordinates application processes
	- Domain
		- Business domain logic
	- Infrastructure
		- Persistence and/or communication with other systems
- System should be built around a domain model
# Anti-patterns
- Anemic domain model
	- Model looks like it has methods from the domain, but actually doesn't
		- Often caused by using setters too much instead of 