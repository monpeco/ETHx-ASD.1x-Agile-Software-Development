### Principles 

* Introduction to week 2 
* The enemy: Big Upfront Anything 
* Organizational principles 
* More organizational principles 
* Technical principles 
* A few method-specific principles

### Agile Principles

(Organizational)
1. Put the customer at the center
2. Accept change
3. Let the team self-organize
4. Maintain a sustainable pace
5. Produce minimal software:
  5.1 Produce minimal functionality
  5.2 Produce only the product requested
  5.3 Develop only code and test
(Technical)
6. Develop iteratively
  6.1 Produce frecuents working scenarios
  6.2 Freeze requirements during iterations
7. Treat test as key resource
  7.1 Do not start any new development until all test pass
  7.2 Test first
8. Express requirements through scenarios


### 1. Put the customer at the center

Beck: You will get [better] results with real customers. The are who you
are trying to please. No customer at all, or a "proxy" got a real 
customer, leads to waste as you develop features that aren't used, specify
tests that don't reflect the real acceptance criteria, and lose the chance
to build a real relationship between the people with the most diverse
perspective of the project.

XP: embedded customer
Scrum: product owner

Can customer involvment replace requirements?

### 2. Accept change

Agile manifesto: "Welcome" change

In standard software engineering, especially object-oriented:
extendibility

Poppendieck: While in theory OO development produces
code that is easy to change, in practice OO systems can be
as difficult to change as any other, especially when information
hiding is not deeply understood and effecively used.




### 3. Let the team self-organize

Traditional view: managers tell workers to do their job
Agile: managers listen to developers, explain possible actions,
provide suggestions for improvments

The leader is there to:

* Encourage process
* Help catch errors
* Remove impediments
* Provide support and hepl in difficult situations
* Make sure that skepticism does not ruin the team's spirit

Team chooses own commitments and has access to customers



### 4. Maintain a sustainable pace

- People perform best if they are not overstressed
- Developers should not work more than hours weeks
- If there is overtime or week-end work one week, ther should not be any in the next week
- XP avoids "crunch time" of traditional projects thanks to short releases cycles

To help achieve these goals
- Frequent code-merge
- Always maintain executables, test-covered, high-quality code
- Constant refactoring, helping keep fresh and alert minds
- Collaborative style
- Constant testing



### 5. Produce minimal software:
###  5.1 Produce minimal functionality

YAGNI (**Jeffries**): [this principle] reminds us always to work on the story we have, not something we thing we're going to need. Even if we know we're going to need it.

**Poppendieck**: Our sofware systems contain far more features than are ever going to be used. Extra features increase the complexity of the code, driving up costs nonlinearly. If even half of our code is unnecessary - a conservative estimate- the cost is not just double; it's perhaps ten times more expensive that it needs to be.

***The "lean" view***

7 wastes of software development

* Extra/unused features (Overproduction)
* Partially developed work not releases (Inventory)
* Intermediate/unused artifacts (Extra Processing)
* Seeking information (Motion)
* Escaped defects not caught by test/reviews
* Waiting (including customer waiting)
* Handoffs (Transportation)

### 5.2 Devvelop minimal software: product only

**Cunningham**:

You are always taught to do as much as you can. Always put checks in. Always look for exceptions. Always handle the most general case. Always give the user the best advice. Always print a meaningful error message. Always this. Always that. You have so many things in the background that you're supposed to do, there's no room left to think. I say, forget all that and ask yourself, **What's the simplest thing that could passibly work?**

### 5.3 Develop minimal software: code and test

Cockburn: You get not credit for any item that does not result in running tested code. Okay, you also get credit for **final deliverables** such as training materials and delivery documentation.

Poppendieck: The documents, diagrams, and models produced as part of a software development project are often consumables, aids used to produce the system, but not necessarily a part of the final product. **One a working system is delivered, the user may caer little about the intemediate consumables**. Lean principles suggest that every consumable is a candidate for scrutiny. The burden is on the artifact to prove not only that it adds value to the final product, but also that is the most efficient way of achieving that value.


---

### Technical principles

6. Develop iteratively
  6.1 Produce frecuents working scenarios

Horizontally layered clusters

  6.2 Freeze requirements during iterations
  
7. Treat test as key resource

  7.1 Do not start any new development until all test pass
  7.2 Test first
  
8. Express requirements through scenarios




### User Story

> A User Story is simply something a user wants

> Stories are more than just text written on an index card but for our purposes here, just think of user story as a bit of text saying something like: "Paginate the monthly sales report", "Change tax calculations on invoices"
> Many teams have learned the benefits of writting user stories in the form of "As a .. I ... so that ..."

### Standard form for user stories

"As a <user_or_role>
I want <business_functionality>
so that <business_justification>"

Example:

"As a customer,
I want to see a list of my recents orders,
so that I can track my purchases with a company"























