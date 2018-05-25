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


### Releases

**Only one pair integrates code at a time** (XP)
* Collective code ownership
* Development proceeds in parallel

But: to avoid conficts, only one pair is permitted to integrate its changes at any given time

**Continuous Integration** (XP)
* The combination of frequent releases with relentless testing
* Keep system fully integrated at all times

Rather than weekly or daily builds, build system several times per day.

Benefits:
* Integration is easier because little has changed
* Team learns more quickly
* Unexpected inteactions rooted out early: conflicts are found while team can still change approach
* Problematic code more likely to be fixed because more eyes see it sooner
* Duplication easier to eliminate because visible sooner

**Release early and often**
* Follows from rejection of "Big Upfront Design"
* Avoid long architectural phases
* Refactor

**Small Releases** (XP)
XP teams practice small releases in two important ways:
* Release running, tested software, delivering business value chosen by the Customer, every iteration. The Customer can use ths software for any purpose, whether evaluation or even release to end users.
* Release to end users frequently as well. Web projects release as often as daily, in house projects monthly or more frequently. Even shrink-wrapped products are shipped as often as quarterly.

**Incremental Deployment** (XP, Scrum)
* Deploy functionality gradually
* "Big Bang" deployment is risky

**Daily Deployment** (XP)
* Goes back to Microsoft's Daily Build
"Chine Shop rules": you break it, you fix it

Difficult to reconcile with other XP principles

**Ten-minutes Build** (XP)
Make sure that the build can be completed, through an automatic script, in ten minutes or less, to allow frequent integration. Includes:
* Compile source code
* Run tests
* Configure registry settings
* Initialize database schemas
* Set up web servers
* Launch processes
* Build installers
* Deploy

Make sure the build provides a clear indication of success of failure.

If it has to take more than ten minutes, split the project into subprojects, and replace end-to-ennd funcational tests by unit tests.



**Weekly Cycle** (XP)

Plan work a week at a time. Have meeting at the beginning of every week:
1. Review progress, including how actual progress for the previous week matched expected progress.
2. Have customers pick a week's worth of stories to implemment this week.
3. Break the stories into tasks.

Start week by writing automated test that will run when the stories are completed. Spend rest completing stories and getting test to pass. The goal es to have deployable software at the end of the week.

The nice thing about a week is that everyone is focused on having the test run on Friday. If you get to Wednesday and it is clear that all thte tests won't be running, you still have time to choose the most valuable stories and complete them.

**Quarterly Cycle**
Recommendation: reviews of high level systems structure, goals and priorities on a quarterly basis, matching the financial reporting practices of many companies.

Also an opportunity to reflect on the team practice and state of mind, and discuss any major changes in practice and tools.

Period chosen as large enough not to intefere with current concerns, and short enough to allow frequent questioning of practices and updates of long-term goals.



### Testing

**Coding Standards** (XP)

Project members all code to the same conventions

**All code must have unit tests** (XP)
Core idea of XP: 
* Do not write code without associated unit tests
* Code that does not pass tests is waste.
* Do not proceed to next step, e.g.
  - Next user story
  - Next release

untill all tests pass

**Test-First Development** (XP)
* Write tests **before** code
* The test replaces the specification

**Test-Driven Development** (XP)
Standard cycle:
* Add a test
* Run all test and see if the new one fails
* Write some code
* Run the automated tests and see them succeed
* Refactor code

Expected benefits:
* Catch bugs early
* Write more tests
* Drive the design of the program
* Replace specifications by tests
* Use debugger less
* More modular code
* Better coverage
* Improve overall productivity

The basic idea is sound..
.. but not the replacement fo specifications by test.

Major benefit: keep an up-to-date collection of regresion tests

Requirement that all tests pass can be unrealistic (tests degrade, a non-passing test can be a problem with the test and not with the software).

Basic TDD idea can be applied with specifications! See Contract-Driven Development

**When a bug found, create test before fixing it** (XP)

A bug is not an error in logic, it is a test you forgot to write.


**Root-Cause Analysis** (XP, Scrum)
When finding a defect, do not just fix it but analyze cause and make sure to correct that cause, not just the symptom

**Run acceptance test often and publish results** (XP)
* Acceptance tests are black box systems tests. Each acceptance test represents some expected result from the system
* Automate them so then can be run often
* Publish acceptance test score is to the team



### Management

**Scrum of Scrums** (Scrum)
* Each day after daily scrum
* Cluster of teams discuss areas of overlap and integration
* A designated person fro each team attends
* Agenda as Daily Scrum, plus the following four questions:
  - What has your team done since we last met?
  - What will your team do before we meet again?
  - Is anything slowing your team down?
  - Are you about to put something in another team's way?

**Whole Team** (XP, Scrum)
All contribuitors sit together as members of one team:
* Includes a business representative who provides requirements, sets priorities and steers the project.
* Includes programmers
* May include testers
* May include analysts, helping to define requirements
* Often includes a coach
* May include a manager

None of this roles is the exclusive property of just one individual. The best teams have no specialist, only a general contributor with special skills.

**Planning Poker** (Scrum)
* Present individual stories for estimation
* Discuss
* Deck has successive numbers (quasi-fibonacci)
* Each participant choose estimate from his deck
* Keep estimates private until everyone has chosen a card
* Reveal estimates
* Repeat until consensus

(Variant of Wideband Delphi technique)

**Open workspace** (XP, Crystal)
Workspace:
* Organized aroung pairing stations
* With whiteboard space
* Locating people according to conversations they should overhear
* With room for personal effects
* With a place for private conversations

Expected benefits: improve communication, resolve problems quickly with the benefits of face-to-face interaction (as opposed to e.g. email)

**Osmotic Communication** (Crystal)
* Team is together in a room and listen to each other
* Information to flow around it
* Developer must break concentration
* Information must quickly throughout the team
* Questions answered rapidly
* All team updated on what is happening
* Reduce need for email and other non-direct communication
* Facilitate taking over of others' tasks

**Informative workspace** (XP, Scrum)
Facilitate communication through well-organized workspace:
* Story borad with user story cards movable from "not started" to "in progress" to "done" column
* Release charts
* Iteration burndown charts
* Automated indicators showing the status of the latest unit-testing run
* Meeting room with visible charts, whiteboards and flipcharts

**Technical Enviroment** (Crystal)
* Access to automated tests, configuration management, frequent integration, code repository.

**Team continuity** (XP)
* Keep the team together and stable
* Do not reassign people to other teams or theat them as mere resources.

**Shrinking Teams** (XP)
* As team grows in capability, keep its workload constant but gradually reduce its size
* This frees people to form more teams
* When the team has to few members, merge it with another too-small team

**Customer allways available** (XP)
All project phases require communication with customer, preferably face to face. Assign one or more customers to the development team who:
* Help write user stories to allow time estimates and assign priority
* Help make sure most of the desired fuctionality is covered by stories
* During planning meeting, negotiate selection of user stories for release
* Negotiate release timing
* Make decisions that affect their business goals
* Try systems early to provide feedback

This may seem like a lot of the customer's time, but the customer's time is saved initially by not requiring a detailed requirements specificacions and later by not delivering a uncooperative system.

**Slack** (XP)
In any plan, include some minor task that can be dropped if you get behind.

Goals:
* Establish trust in the team's ability to deliver
* Reduce waste

