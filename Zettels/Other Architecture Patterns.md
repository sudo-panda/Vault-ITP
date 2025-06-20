---
tags:
  - Architecture_and_Architecture_Patterns
---
- Service Mesh
	- Infrastructure layer handling service-to-service comms and corresponding config
	- Part of cloud native arch
- Backend for frontend
	- Services providing Frontend-specific APIs, e.g. lil data for mobile device use or rich analytics data for feature-rich front-ends
	- Enables more efficient/ faster front ends
- Micro-frontends
	- Applying microservices concepts to front-ends
	- More independent development
- Serverless & Function as a Service
	- Enabling to run a time-restricted function without explicitly allocating a server, reacting to events
	- Saving on cloud infrastructure for rarely running functions
- Event sourcing
	- Storing all data as events, never deleting data and providing "projections" of the actual state of data
- Command Query Responsibility Separation (CQRS)
	- Add-on to Event Sourcing, letting different components handle change/commands and queries providing projections
- Distributed ledger Technology/Blockchain
	- Using event-sourcing, implementing automatic replication and distributed consensus with untrusted parties
- Hexagonal/Ports & Adapter Arch
	- Separating core business logic from external concerns
	- Makes external concerns independent from core business logic
- Data Mesh
	- Breaking down data into data products managed by different teams with federated governance
	- Concept of domain-driven design/microservices applied to data
- Space-based Arch
	- Aims for high scalability through in-memory data grids and distributed processing
	- Impact:?
- Reactive/stream processing
	- Real-time processing of events or data streams
	- Real-time processing
- Actor model
	- Natural concurrency model, where a component receives data or an event, processes it and passes the result to other actors
	- Strong fit with microservices, event-sourcing and reactive.stream proessing
### Event sourcing & Command Query Responsibility Separation
- Full audit trail, never deleting events
- Timeshift functionality
- Different data representations for different uses
- Requires good caching in projectors to offer good performance
- Extremely robust data storage
- Very good support for rollback
- Potentially simplifies data privacy compliance or complicates it
### Distributed Ledger Technology/Blockchain
- Fundamentally a distributed event-sourcing architecture with automatic replication and distributed consensus algorithms
- Can be tuned for different needs, eg. for very high throughput transaction processing or many replicas
- Consensus algorithms can be designed to use voting rather than trust, enabling transactions between untrusted parties

## Use of AI Capabilities in Apps
- Novel UIs
- New sensory capabilities/extraction of data from unstructured input
- AI capabilities
- AI generated funcitonality
- New output generation capabilities

## Business requirements and Archs
|                           | Business requirements                                                                                                                                                                                                                                                                                                                                                                       | Architecture Patterns                                                                                                                                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Multi-tenant capabilities | - Allowing multiple separate to be served from a single system<br>- Prerequisite for many SaaS-offerings<br>- Implementation flows may leak data to 3rd parties<br>- Retrofitting capability very difficult                                                                                                                                                                                 | - Keep tenant-related data separate in separate databases                                                                                                                                                             |
| Time-dependent data       | - Enabling data to be kept separate by period and to be applied by period<br>- Enabling different versions of data over time to e maintained, regenerated, and compared<br>- Lack of capability may limit what can be changed when, require complex procedural workarounds, or lead to processing errors; it may also make audits much more difficult<br>- Retrofitting extremely difficult | - Never overwrite existing data, but add changes to the data, allowing to regenerate every earlier state of the data<br>- Such archs are known as "event-sourcing" archs as they store all data changes as events<br> |
| Multi-language support    | - Allowing system to be used with different languages<br>- Requires dictionaries of texts for all inputs and outputs and flexible formatting<br>- Retrofitting possible                                                                                                                                                                                                                     | - Translate every input and output through language specific tables<br>- Make formatting adapt to the text being displayed or printed                                                                                 |
