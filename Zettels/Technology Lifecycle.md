---
tags:
  - Technology_Lifecycle
---
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
		- **Long duration** with nothing to show (big bang) or lil true benefit until the end erode momentum on business and subsequently IT side (step-wise)
		- **High complexity**
		- Lack of detailed business logic understanding
		- Need to invest into two systems
		- Project abortions often leave company in a worse situation than before the project
- Replace with package
	- projects have different sizes, depending on the amount of functionality covered
	- project success rate is high, even though there are a number of high-profile failures, in particular in cases where the supplier could not deliver functionality the customer considered important
	- satisfaction after migration varies a lot, with reported weaknesses including
		- functionalities do not support the business as well as the former solution
		- high efforts for surrounding systems which close gaps of the package or integrate with it
		- ability to obtain new functionalities low
		- package suffering from legacy issues too
- Replatform
	- projects are narrowly defined to address technical obsolence
	- moving the application onto a different tech platform leaving functionality, architecture and tech debt as is
	- static code translators are used if possible, ehich have a bad reputation of generating hard to maintain code
	- <mark style="background: #88FF88DD;">success rate high</mark>
	- <mark style="background: #FF5582DD;">lil benefit to business</mark>
- Refactor
	- Gradually addressing legacy issues in an app, leaving app in place, and changing or rewriting parts over time
	- With it being an ongoing activity with small steps it
		- <mark style="background: #88FF88DD;">has low risk</mark>
		- <mark style="background: #88FF88DD;">no radical changes in app</mark>
		- <mark style="background: #FFB86CA6;">cannot be evaluated well (not binary success or failure)</mark>
		- fits well into maintenance activities for the app
- Software mimicry
	- Use AI and large number of observations

## Selecting Apps for Renewal
### Analyze the legacy situation
Understand for each attribute
- Does the application have it
- How big is it
- How large are risks if unresolved
- How much business value could be unlocked if resolved
### Select an app and approach w/ a positive business case or large risk avoidance
- Identify legacy applications that include large business risks
- Identify legacy applications where resolving issues unlocks large business value
- Focus on most attractive renewal opportunities, and put all others into either "do not touch" or "refactor" mode
- Select an approach that addresses the actual issues and unlocks business value or risk avoidance
### Examples
- Application running on obsolete technical platform, with little other legacy issues: REPLATFORM
- Application with strong business functionality, but architectural issues and technical debt preventing it to be extended further, such as for
	- merging acquired business into the application
	- leveraging the application in other geographies
	- implementing new business offerings
	LARGE REFACTORING INITIATIVE (focus: business needs)
- Application with outdated functionality, which is non-differentiating: REPLACE w/ PACKAGE
