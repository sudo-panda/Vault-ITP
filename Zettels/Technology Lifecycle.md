### Emulation

### Security considerations

### Key Takeaways
- Every technology is subject to a lifecycle from inception to decline and obsolescence
- In IT, total duration ranges from 60+ years (IBM Mainframe) to 40+ years for highly successful technologies to less than 20 years for less successful ones
- Emulation can add a significant number of years to the use of an obsolete technology
- Obsolescence is generally a weak reason to quickly replace systems relying on it, but often used as an argument
- Making good technology decisions in light of lifecycle considerations is very challenging

### Attributes of Aging software 
- Functional obsolescence
	- Apps may become functionally obsolete if a business changes dramatically or a company discontinues a business or service
	- Challenging are cases where an application is functionally obsolete in parts, leaving a large code base with much unused functionality, which cannot be retired as some other functionality is still needed.
- Technical debt
	- Nor bad practice but result of many sensible decisions
	- The more technical debt an app has the more likely it will accumulate more
	- Business-critical systems: avoid risk - avoid major code changes - add tech debt
- Architectural obsolescence
	- Evolution in business and tech makes chosen arch obsolete
- Technical obsolescence
	- New apps are generally developed using tech then considered mature
	- My the time the app is mature the underlying tech is already in decline
	- Apps tend to have longer lifecycles than many techs

## Legacy Software
- Functionally fit-for-purpose
- Has a some combination of:
	- Tech debt
	- Technical obsolescence
	- Architectural obsolescence
	- Partial functional obsolescence

### Approaches to address legacy software 
- Do not touch
- Rewrite
	- Typically large scale programs with a high rate of failure
	- Experienced challenges
		- **Long duration** with nothing to show (big bang) or lil true benefit until the end erode momentum on business and subsequently IT side
		- **High complexity**
		- Lack of detailed business logic understanding
		- Need to invest into two systems
		- Project abortions often leave company in a worse situation than before the project
- Replace with package
- Replatform
- Refactor
- Software mimicry

