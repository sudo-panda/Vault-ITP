- As application size increases the Person Months required increwases super linearly
- As system size increases the the productivity falls in a log fashion
## Function Point Analysis
- **Usage**: FPA can be used to estimate:
	- Efforts: how many person months does one require to develop a software system?
	- Costs: how much are the total development costs?
	- Schedule: when will it be done?
	- Deliveries: all of the above for individual deliveries
- **Benefits**: FPA offers
	- Technology independence: regardless of language, development method, or hardware platform used, the number of function points for a system remains constant
	- Variability: FPA can be employed for all kinds of software
	- Completeness: FPA measures all activities, not only coding
	- . . . and it allows for statistical analysis

### Calculation
Decomposition system into five functional classes:
1. External inputs (EI), e.g., values passed from a user input mask
2. External outputs (EO), e.g., a report
3. Internal logical files (ILF), i.e., system states
4. Inquires (EQ), e.g., a query to a database
5. External interface files (EIF), e.g., a database

For element it complexity is estimated, assigning it a number of function points and summing it all up to get the total

