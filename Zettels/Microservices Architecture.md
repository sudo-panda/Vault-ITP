---
tags:
  - Architecture_and_Architecture_Patterns
---
Microservice architecture - a variant of the service-oriented architecture (SOA) structural style - arranges an application as a collection of loosely coupled services.

In a microservices architecture, services are fine-grained and the protocols are lightweight.

### Critiques
| Attributes                                                             | Critique                                                                                                                                                                                         |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| - Modularization by "business capability"<br>- Clear, stable interface | - Benefits are not unique to microservice archs, but a result of how well the modularization was done                                                                                            |
| - Fine granular                                                        | - Fine granularity can easily lead to performance problems<br>- New business requirements call for changes to many services<br>- Understanding the network of services can become very difficult |
| - Processing easily distributable over multiple machines               | - Advantages in scalability only achievable if app \|\|elizable and microservice overhead not large                                                                                              |
### Versioning Problem
|                                   | Monolithic                                                           | Shared library/local service                                                | Micro-service in cloud            |
| --------------------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------- |
| Upgrading 3rd party funcitonality | Rebuild app with new lib version re-test and redeploy on all systems | Redeploy the new lib version on all systems<br>- Test ??                    | (done by supplier)<br>- Test ???? |
| Control over upgrade              | Full Control                                                         | Must be coordinated with all users on the same machine to have full control | No control                        |
#### Version Conflicts Solution: Illusion of single machine:
- Single physical machine - No illusion, versioning problem big
- Virtual Machines - Easy versioning, too resource intensive
- Containers - Easy versioning, not too resource intensive
- Env Managers(Conda only) - lil versioning problems but not resource intensive

Amason Prime Video: Was Microservices $\mapsto$ Now Monolith