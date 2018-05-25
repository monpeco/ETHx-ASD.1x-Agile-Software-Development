### Introduction to week 4
1. Meetings
2. Development
3. Release
4. Testing and quality
5. Management and others

### 1. Meetings

**Daily meeting**
* Held every morning
* **Goal**: set the day's work, in the broader context of the project
* Time-limited, usually 15 minutes (stand-up meeting)
* Involves all team members, with special role for "committed"
* Focus:
  - Defining commitments
  - Uncovering impediments
* Resolution will take place outside of meetings

Planning Meetings, Review Meetings

**Daily Meeting: The 3 questions**
The daily meeting requires every team memer to answer 3 questions:
* What did you do yesterday?
* What will you do today?
* Are there any impediments in your way?

**Planning Meeting**
* At beginning of every sprint
* **Goal**: define work from sprint
* Outcome: Spring Backlog, with time estimate for every task
* 8-hour time limit
  - 1st half, Product Owner + Team: prioritize Product Backlog
  - 2nd half, Team only: plan for Sprint, producing Sprint Backlog

**Retrospective Meeting**
* At end of every sprint
* All team members reflect on past Sprint
* Make continuous process improvements
* Two main questions:
  - What went well?
  - What could be improved?
* 3-hour time limit

**Review Meeting**
* At end of every sprint
* Review work:
  - Completed
  - Not completed
* Present and demo completed work to stakeholders
* Incomplete work cannot be demostrated
* 4-hour time limit

**Reflective Improvement** (Crystal)
* Developers must take breaks from regular development to look for ways to improve the process
* Iterations help with this by providing feedback on whether or not the current process is working

**What we have seen:**
* Agile development is characterized by a set of well-defined meetings
* Most important is the Daily Meeting
* In Scrum: Planning and Review Meetings
* Require adaptations for distributed teams



### 2. Development

**Pair Programming**
Two programmers sitting at one machine, thinking out loud.

**Goals**
* Make thinking process explicit
* Keep each other on task
* Brainstorm refinements to systems
* Clarify ideas
* Take initiative when other stuck, lowering frustration
* Hold each other accountable to team practices

**Single Code Base** (XP)

Maintain a single code base: avoid branching, even if permitted by configuration management system


**Shared Code** (XP)
Agile methos reject code ownership in favor of code whose responsibility is shared by entire team

Rationale:
* Most non-trivial features extend across many layers in the application
* Code ownership creates unnecessary dependencies between team members and delays
* What counts is implemented features, not personal responsibility
* Avoid blame game
* Avoid specialization
* Minimize risk (team members leaving)

**Leave optimization till last** (XP)
* Wait until you have finished a story and run your test before you try to optimize your work
* Only then can you analyze what exactly it is that needs optimizing
* Do not make work for yourself by trying to anticipate problems before they exist

**Simple Design** (XP)
* Produce the simplest design that works
* Refactor as needed


**Incremental Design** (XP)
Developers work in small steps, validating each before moving to the next 

* Start by creating the simplest design that could possibly work
* Incrementally add to it as the needs of the software evolve
* Continuously improve design by reflecting on its strengths and weaknesses


**System Metaphor** (XP)
A metaphor is meant to be agreed upon by all members of a project as a means of simply explaining the purpose of the project and thus guide the structure of the architecture

**Refactoring** (XP)
Disciplined technique for restructuring an existing body of code, altering its internal structure without changing its external behavior

Examples refactoring techniques:
* Encapsulate attibute (field) into function
* Replace conditional with dynamic binding
* Extract routine (method)
* Rename routine or attribute
* Move routine or attribute to another class
* Pull up, Pull down

Used in agile methods as a substitute for upfront design




