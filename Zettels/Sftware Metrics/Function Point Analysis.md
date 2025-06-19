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

For element it complexity is estimated, assigning it a number of function points and summing it all up to get the total.

### Sample System and Project Sizes
- **Very Small Systems** - 100 FP
	- Built by single person or small team within a few months
	- Cost ~100k CHF
- **Small Systems** - 1000 FP
	- Built by team of 5-10 staff within 1-2 years
	- Cost ~3m CHF
- **Typical major systems in large corporations** - 10000 FP
	- Built by large teams over 3-5 years, often extended over many years
	- Cost ~50m CHF
- Largest systems in existence - 100000 FP
	- Very few examples
	- Built by very large teams over many years in several major releases
	- Cost one billion or more CHF

### Caveats
- Doesn't measure but estimate software size and complexity
- There are many weaknesses when you look at a single example, which also lead to inconsistencies

Despite these weaknesses over a large number of samples, strongly statistically relevant results are found
- Avoid combining data from different sources
- When doing calculations, do them precisely not to accumulate errors, but be aware that the result has a relatively large error range

