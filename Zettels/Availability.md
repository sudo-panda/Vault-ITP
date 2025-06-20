---
tags:
  - Architecture_and_Architecture_Patterns
---
Time a business functionality is reachable and operational as a percentage of total time
Time unavailable includes both planned and unplanned outages

## Achieving High Availability
- 99%
	- Single low-end server
	- Prototype-quality software
	- Ad-hoc ops
- <99.5%
	- Single high-quality server
	- Stable software
	- Well managed ops
- <99.9%
	- Hot standby (second running server able to take over quicky)
	- Data replication
	- Highly stable software
	- Automated/quick failover
- <99.9%
	- Redundancy at every level
	- Ability to add/remove components while running
	- Sophisticated base services
	- Software written for distributed, fail-resistant environment
	- Highly automated ops
- Higher
	- Increasing fine-granular redundancy and failure detection at every level
	- Software designed to stop activity on one server and continue on another

