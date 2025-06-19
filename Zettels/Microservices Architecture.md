Microservice architecture - a variant of the service-oriented architecture (SOA) structural style - arranges an application as a collection of loosely coupled services.

In a microservices architecture, services are fine-grained and the protocols are lightweight.

### Critiques
| Attributes                                                             | Critique                                                                                                                                                                                         |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| - Modularization by "business capability"<br>- Clear, stable interface | - Benefits are not unique to microservice archs, but a result of how well the modularization was done                                                                                            |
| - Fine granular                                                        | - Fine granularity can easily lead to performance problems<br>- New business requirements call for changes to many services<br>- Understanding the network of services can become very difficult |
| - Processing easily distributable over multiple machines               | - Advantages in scalability only achievable if app \|\|elizable and microservice overhead not large                                                                                              |