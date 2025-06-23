---
tags:
  - Architecture_and_Architecture_Patterns
---
Software architecture is about making fundamental structural choices that are costly to change once implemented. Two laws:
1. Everything is a trade-off
2. "Why is more important than how"

Different Archs for different design aspects
- Application Arch
- Infrastructure Arch
- Software Layer Arch
- Data Arch . . .

## [[Purpose, Pitfalls, Good Practice of SW Arch Docs]]

## Modularization
- The degree to which a system's components may be separated and recombined, often with the benefit of flexibility and variety in use.
- breaking a system into varying degrees of **interdependence** and **independence** across
- In software design, typical modularization objectives are:
	- Enable independent design, implementation, and test of individual modules by different teams
	- Increase flexibility/agility by new requirements only impacting one or few modules
- A good modularization minimizes dependencies between modules, and provides narrow, stable interfaces
- Designing it requires a profound understanding of business functionality and dependencies and great foresight about potential future requirements
- A shift in business needs can turn a good modularization into a bad one

