---
tags:
  - Architecture_and_Architecture_Patterns
---

| Benefits                                                                             | Challenges for Devs                                                              | Impact on Operations                                                                |
| ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| High [[Availability\|availability]]                                                  | Understanding respective concepts                                                | Handle 10+ connected services for what used to be a single server                   |
| Scalability: Add or remove redundant components to adapt to volume                   | Designing application for distributed processing, failure detection and recovery | Implement automated deployment, configuration, monitoring, failure detection, . . . |
| Gradual upgrades:<br>Add a changed component, ensure it works well and then roll out | Tuning performance to overcome overhead of distributed architecture              |                                                                                     |
### Function Call vs API Call
| Function Call                                                 | HTTP API Call                                                                                                                                                                                                                                             |
| ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Passing data in memory<br><br>Executing the business function | Putting data in network packet<br><br>Identifying network address of service<br><br>Sending data through network<br><br>Identifying which service to execute, unpacking data<br><br>Executing the business function<br><br>Same path back through network |

### Alternatives for High Scalability and High Availability
- Scalability
	- Use a larger server
	- Tune software for low resource needs and scalability
- High Availability
	- Use hardware and software designed for high availability and high availability
	- Very expensive equipment, but may pay off in lower software complexity
