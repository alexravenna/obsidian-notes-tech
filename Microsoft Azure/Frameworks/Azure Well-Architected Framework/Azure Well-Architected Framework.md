---
created: 2024-02-12T08:03:29Z
updated: 2024-12-10T08:34:58Z
aliases:
  - WAF
homepage:
  - https://learn.microsoft.com/en-us/azure/well-architected/
---
# Description
- Pillars:
	- [[Reliability]]
	- Security
	- Cost optimization
	- Operational excellence
	- Performance efficiency
# Workloads
- Workload: a collection of application resources, data and supporting infrastructure that function together towards a defined business goal
# [[Reliability]]
- Design principles:
	- Design for business requirements:
		- determine dependencies
		- understand platform commitments
	- Design for [[resilience]]:
		- distinguish components that are on the critical path (i.e. [[logging]] isn't critical)
		- identify potential failure points
		- self-preservation and [[self-healing]]
		- redundancy in layers
	- Design for recovery:
		- recovery plans
		- strategy for disaster recovery
	- Design for operations:
		- [[Shift-left|shift left]] in operations to anticipate failure conditions
			- build [[Observability|observable]] systems
			- simulate failures (e.g. [[chaos testing]])
			- automation (e.g. [[Infrastructure as Code]])
	- Keep it simple
		- avoid overengineering the architecture design, application code and operations:
			- keep the critical path lean
			- establish standards
			- use [[PaaS]] and [[SaaS]]
# [[Security]]
- Design principles:
	- Plan your security readiness
	- Design to protect confidentiality
	- Design to protect integrity
	- Design to protect availability
	- Sustain and evolve your security posture
# Cost Optimization
- Design principles:
	- Develop cost-management discipline
	- Design with a cost-efficiency mindset
	- Design for usage optimization
	- Design for rate optimization
	- Monitor and optimize over time
# Operational Excellence
- Related to [[DevOps]]
- Design principles:
	- Embrace DevOps culture
	- Establish development standards, e.g. [[agile]]
	- Evolve operations with observability
	- Deploy with confidence
	- Automate for efficiency
	- Adopt safe deployment practices
# Performance Efficiency
- Design principles:
	- Negotiate realistic performance targets
	- Design to meet capacity requirements
	- Achieve and sustain performance
	- Improve efficiency through optimization