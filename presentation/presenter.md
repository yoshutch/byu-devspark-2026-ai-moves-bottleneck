# Presenter Notes
1. Load Shapez game before presentation starts
2. Open screen capture video
3. Start demo code `go run .`

## 02 — AI Wrote the Code

- Start with the small demo codebase: Advisement appointment API
- Show the video of Codex adding a new feature

## 03 — Is It Ready?

- Ask the audience to diagnose the change before showing your own checklist.
- Write their responses on the whiteboard or group them verbally under problem, correctness, security, and delivery/operation.

## 04 — We've Seen This Before

- Switch to Shapez
- This is a bit of a contrived example, but may not be far from the truth in some situations
- Quickly walk through 
	- the goal of Shapez: trying to build X amount of certain shape
	- the steps to create the shape
- Show the throughput (should be about 1/s)
- Add more painters
- Show how it speeds that part up, but what else do we see?

## 05 — The DevSecOps Software Lifecycle

- Now, let's tie manufacturing into software!
- This is a DevSecOps view of the Software Development Lifecycle
- Ask: "What else goes into developing a working piece of software?"
- Ask the audience which stage usually takes the longest in their work.
- Ask which stage would become the bottleneck if development suddenly became ten times faster.

## 06 - So Many Lines of Code!
- Ask: "How can we improve the lifecycle?"
- "Often some people think the answer is to use AI to make more code faster!"

## 07 - The Silver Bullet?
- Frederick P. Brooks, Jr. wrote a paper in 1986 entitled "No Silver Bullet", full quote:
> There is no single development, in either technology or management technique, which by itself promises even one order-of-magnitude improvement within a decade in productivity, in reliability, in simplicity.

- Some research findings here are a bit dated and AI models have improved a lot since then.
- Still this is only supposed to highlight that when AI is used to primarily improve only one portion of the development lifecycle, the gains are not what we expect.

- "Let's take a step back and ask ourselves a more fundamental question"

## 08 - What Is the Goal?
- Write down their ideas

## 09 — The Goal: Improve the Flow

- Introduce *The Goal* as a story about a manufacturing plant, but the lessons apply to any system with work flowing through it.
- Productive = anything that moves towards The Goal
- Keeping every station busy is not the same as delivering more valuable outcomes.
- Jump back to Shapez
	- Show the throughput (should be about 1/s still)
	- Show the bottleneck (at the cutters) = large pile of materials is inventory
	- "We increased operating expense by increasing the number of painter machines"
	- How does this factory equate to software development?
- In most companies the goal is to **make money**
- What is BYU's goal? Anyone have a guess or have it memorized?

## 10 — BYU's Goal

- Clarify that this is the goal for this talk—not maximizing lines of code, story points, or software throughput for its own sake.
- Ask: “What does your software make possible for students and faculty?”
- Share an example from BYU systems study abroad:
	- I used to work on a web application that facilitated the process to apply for international study abroad programs.
  	The features we added to that system had an impact towards students' progression, specifically the "Strengthen the student experience" strategic objective.

## 11 — Plan, Code, & Build

- Let's jump back to DevSecOps software lifecycle!
- Ask: “How often do we discover the real business rule after development has started?”
- Ask: "How many of you have asked if what you're working on has any real value to the University? To its goal?" - sometimes the less things we build, the more value we add
- Connect this slide to the Shapez developer station: if coding accelerates, architecture, CI capacity, and the feedback loop may become the constraint.

## 12 — Test, Release, & Deploy

- Ask: “How many of you wait for review, UAT, or security approval before rollout? How long do you wait?”
- Distinguish generating tests from establishing confidence. AI can suggest edge cases and draft tests, but people still decide whether the evidence represents the real risk.
- Share the hard-coded database credential story as the concrete reminder that code can work and still be unsafe.
	- I was asked to review the code of an AI generated piece of software. This was from a team that didn't normally write code. They reached out to see what the next step was to hosting and running this code on BYU infrastructure. This was intended to be run on the browser for hundreds, possibly thousands of individuals concurrently. I took a look and quickly found that the AI hard-coded database credentials in the HTML and JavaScript.
- Ask: “What would we need to know before allowing a change into production?”

## 13 — Operate, Monitor, & Feedback

- Remind the audience that software is not finished when it is deployed.
- If we're not careful; alert noise, incident response, support work, and maintaining generated complexity all consume capacity ~ can be viewed as an increase in operating expense, regardless of how fast it was developed and released.
- Ask: “What evidence would tell us that this feature actually helped students or faculty?”

## 14 — Find the Constraint

- What are some ways we can find the constraints or bottlenecks?
- Ask the audience where work waits in their systems: pull-request review, security findings, UAT, CI runners, release approvals, or operational response.
- You can use methodologies like DDD, TDD, Team Topologies, Agile etc. Things we've learned for years that are all trying to solve aspects of accomplishing the goal.
  - These can be used to address different symptoms of bottlenecks, so understand these patterns and match the pattern that fits your constraint
- Use the question: “If code generation becomes ten times faster, where does the extra work wait?”

## 15 — Improve the System

- Return to Shapez and ask the audience to identify the current constraint.
- Demonstrate the three moves:
	1. Remove unnecessary work before the constraint = remove extra stars.
	2. Filter defective inputs before they consume bottleneck capacity = remove random squares.
	3. Increase flow through the constraint = fix the cutter station.
	- Now you can see there's a more steady flow going into other parts of the system, we can see the throughput increase
      - Throughput should be close to 2/s
      - Inventory should be flowing constantly, less stagnant piles before machines
      - Yes operating expense increased, but so did our value
- Close with: “Find the constraint. Improve the system around it. Use AI where it actually helps.”
- End with the mission question: “What would help our software move students and faculty toward learning, excellence, and their full potential?”

## 16 - End
- The biggest takeaways I want you to leave with are:
	- Software development is more than just coding, to be "productive" you must incorporate all the different aspects of software development lifecycle
	- Keep in mind the bigger picture: how does your work contribute to BYU's goal?
