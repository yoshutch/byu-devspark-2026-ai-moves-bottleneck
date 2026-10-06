# AI Didn’t Make Development Faster - it Moved the Bottleneck
> AI can write your code faster, but was writing code the slow part of the software development lifecycle? Does AI improve collaboration with users, speed up quality assurance, decrease deployment time, increase system comprehension, or reduce the friction of operating and monitoring software?
> 
> AI didn't make software development faster, it only moved the bottleneck.

## Working thesis
AI can accelerate individual activities, but development only becomes faster when the entire system is improved to facilitate BYU's mission: assisting individuals in their quest towards perfection and Eternal Life through learning, commitment to excellence, and the full realization of their potential.
## Outline

### Intro
- "Safe harbor" statement - this is my opinions, not official direction of OIT
- I want to clarify that although I am skeptical of AI for code generation (might be some bias in this presentation), I want to be clear AI can still help make us more effective
### AI Generated Code Example
- start with a demo code base
- present a new feature that's needed
- plug that feature into Codex
- ask audience if it's ready
- write on whiteboard their responses
### Factory Example
- Show a Shapez workflow example that has a few small bottlenecks but works
- Label certain portions as different parts of the software development lifecycle or DevSecOps cycle
- Increase the speed of the developer part and show the accumulation of "inventory"
### Software Development Lifecycle
- Show SDLC diagram
- Show how an increase in one step doesn't make the whole cycle faster
- What else goes into developing a working piece of software?
	- What takes you the longest on a task?
	- What hidden (or visible) checklist items are in a feature request?
- What part is the most important?
### Improve the Lifecycle
- Show screenshot of chief executives bragging about how many lines of code they made
- Often the go-to answer in the software industry is to use AI code generation to "improve" the flow
### AI Isn't the Silver Bullet
- Fred Brooks quote: 
	> “there is no single development, in either technology or management technique, which by itself promises even one order of magnitude tenfold improvement within a decade in productivity, in reliability, in simplicity.”
- Studies that show AI in development doesn't always increase code throughput
- Studies that show AI generated code on average increases bugs
- AI doesn't introduce new problems it amplifies already existing problems
### The Goal
- What is the Goal?
	- is it to be as efficient as possible?
	- to keep everyone busy?
	- to maximize the number of story points or tasks you accomplish each week/sprint?
- Introduce the book
- The goal in a typical company is usually: "To make money"
- What is BYU's goal?
	- Mission, AIMS, and Becoming BYU
- Anything helping that goal is "productive"
	- Example of how software at BYU helps BYU's mission
		- Student Ecclesiastical Endorsement System, International Study Abroad program, Student Voting, etc.
		- What are ways your software connects to BYU's mission/goal?
- How can software support that goal?
- 3 metrics
	- **Throughput:** mission-aligned outcomes enabled for students and faculty.
	- **Inventory:** work in progress, unreviewed code, unresolved findings, deployment queues, and accumulated technical debt.
	- **Operating expense:** the people, tools, and time required to move work through the system and keep it running.
- Identify the bottleneck
	- Make sure it's doing most valuable work
	- Eliminate unnecessary work that must pass through it
	- Add quality controls before the bottleneck
	- Increase the throughput of the bottleneck
### DevSecOps
#### Understand & Build
- Can be a bottleneck when the problem, user, success criteria, business rules, architecture, CI capacity, or feedback loop are unclear or slow.
- Improve flow with mission-aligned outcomes, clear acceptance criteria, shared domain language, TDD, and fast CI feedback.
- AI can expose ambiguity, challenge assumptions, prototype quickly, and accelerate small changes.
- Security questions: What requirements and abuse cases should influence the design? Are dependencies, secrets, permissions, and generated artifacts handled securely?
#### Verify & Deliver
- Can be a bottleneck when pull requests, manual tests, UAT, security review, approvals, or releases form a queue.
- Improve flow with small pull requests, explicit review ownership, automated checks, small batches, progressive delivery, feature flags, and easy rollback.
- AI can suggest edge cases and draft tests, but people still establish confidence and own the release decision.
- Security questions: Have we verified the highest-risk behaviors? Are production configuration and rollback paths safe?
#### Operate & Learn
- Can be a bottleneck when alert noise, incidents, support work, or user feedback are difficult to understand and act on.
- Improve flow with useful telemetry, runbooks, incident ownership, outcome metrics, and explicit follow-up work.
- AI can summarize operational evidence and feedback, but people decide whether the work advanced the mission.
- Security questions: Do logs or responses expose sensitive data? Can we detect misuse, and do we trust the feedback?

### Find the Constraint
- Look for evidence of the constraint rather than relying on the most visible complaint:
	- aging queues and long waits
	- rework and recurring defects
	- scarce capacity such as reviewers, CI runners, or release windows
	- slow feedback about whether the change helped users
- consumed people, tooling, and support capacity
- Measure the flow from idea to validated outcome.
- Improve the suspected constraint and check whether valuable throughput increases.
- Match the intervention to the constraint:
	- Understanding: clear requirements, domain language, and prototypes
	- Feedback and review: TDD, CI, small changes, and explicit ownership
	- Release and operations: automation, progressive delivery, observability, and runbooks
	- Learning: user feedback, outcome metrics, and continuous improvement

### Improve the System
- Remove unnecessary work before the bottleneck.
- Filter defects earlier.
- Increase flow through the constraint before upgrading everything else.
- Use AI for bounded prototypes, information synthesis, assumption-checking, drafts, and edge-case exploration.
- Keep humans responsible for mission, architecture, security, judgment, and acceptance.
- Review the Shapez factory and close with: Find the constraint. Improve the system around it. Use AI where it actually helps.
