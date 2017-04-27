
<!-- .slide: data-background="#555" id="the-beginning" -->
## Exploratory Testing <!-- .element: style="color:#eee" -->

By Group 6 <!-- .element: style="color:#aaa" -->

`06·26·46·56·66` <!-- .element: style="color:#579;font-size: 0.5em" -->
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

## Agenda
* [Theory &amp; Definition](#section-theory-and-definition) <!-- .element: class="fragment" data-fragment-index="1" -->
* [Question &amp; Answer](#section-q-and-a) <!-- .element: class="fragment" data-fragment-index="2" -->
* [Example](#section-example) <!-- .element: class="fragment" data-fragment-index="3" -->
* [Summary](#section-summary) <!-- .element: class="fragment" data-fragment-index="4" -->
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
<!-- .slide: data-background="#09c" id="section-theory-and-definition" -->
## Theory &amp; Definition  <!-- .element: style="color:#eee" -->

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
<!-- Following pages abstracted from slides provided in class. Remove them if they are useless. -->
## Basic Description

| Item         |  Description          |
|:------------:|:----------------------|
| Tag line     | Simultaneous learning, planning, and testing |
| Objective    | Simultaneously learn about the product and about the test strategies to reveal the product and its defects |
| Testers      | Explorers |
| Coverage     | Hard to access |

////////////////////////////////////////

##### (Continued)

| Item         |  Description          |
|:------------:|:----------------------|
| Potential problems | Everything unforseen by planned testing techniques |
| Activities   | Learn, plan, and test at the same time |
| Evaluation   | Varies |
| Complexity   | Varies |
| Harshness    | Varies |
| SUT readiness | Medium to late: use cases must work |

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

## Representative cases
* Skilled exploratory testing of the full product
* Rapid testing & emergency testing (including thrown-over-the-wall test-it-today)
* Troubleshooting / follow-up testing of defects.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

## Strengths
* Customer-focused, risk-focused
* Responsive to changing circumstances
* Finds bugs that are otherwise missed

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

## Blind spots
* The less we know, the more we risk missing.
* Limited by each tester's weaknesses (can mitigate this with careful management)
* This is skilled work, juniors are not very good at it.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
<!-- The following slides are collected from Internet. Some part are repeated with contents above. -->
### What is Exploratory Testing?
> a style of software testing emphasizing the personal freedom and responsibility 
 of the individual tester to continually optimize the value of her work by treating
 test-related learning, test design, test execution, and test result interpretation 
 as mutually supportive activities running in parallel throughout the project.
 <br />-- Cem Kaner
////////////////////////////////////////
#### Exploratory testing is simultaneous learning, test design, and test execution.
> the testing that design and execution are performed at the same time, opposite to scripted testing

- no definition in advance
- "improvised", "impromptu"
- no plan to follow preciously
- *scripted testing*: not fully opposite to it, since the scripted testing 
  still contains interesting details that are uncovered

Note:
* the quote is a *Plainest* explanation, with some uncompleted compare with *scripted testing* and *"ad hoc" testing*
* the scripted testing doesn't mean complete coverage of testing details (leaves blanks for exploratory actions),
  whereas the exploratory testing doesn't means no preparation as instruction at all.
* *"ad hoc"*: test the testing that performed completely without previous 
  planning and filly according to the interesting of tester.
////////////////////////////////////////
#### Decomposing the term
the exploratory testing consists of both "exploratory" and "testing"
  - *exploratory*: emphasize on the freedom and personality of action (testing) executor.
    + often performed by individual
    + simultaneously learning from the situation and planning for next action, then perform the action instantly
  - *testing*: perform specific task with the subject testing unit and compare the result with expectation

Note:
* this section try to explain the definition of ET from its literal terms
* *exploratory* is not limited to the testing field, but also the design, development, etc.
////////////////////////////////////////

#### Other perspectives
* Exploratory testing is not a testing technique. It's a way of thinking about testing.

Note:
* Example: after bug regression, a tester may verify the fix of bug then *explore* the fixed software to search for side effects.


>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Why to perform exploratory testing?
#### Objective
   Simultaneously learn about the product and about the test strategies 
   to reveal the product and its defects
   * it is not random, but purposed
////////////////////////////////////////

#### Detailed Goal I: To gain quick understanding of application
* Understand how an application works, what its interface
  looks like, and what functionality it implements.

* Such a goal is often adopted by testers new to a project or those who want
  to identify test entry points, identify specific testing challenges, 
  and write test plans. 
* This is also the goal used by experienced testers 
  as they explore an application to understand the depth of its testing needs 
  and to find new unexplored functionality.

////////////////////////////////////////
#### Detailed Goal II: To force the software to exhibit its capabilities
* The idea is to make the software work hard and to ask it hard questions 
  that put it through its paces. This may or may not find bugs, 
  but it will certainly provide evidence that the software performs the function 
  for which it was designed and that it satisfies its requirements.

* Some other test approaches may constraint the testers to perform certain actions,
  whereas the exploratory testing can be used to verify functionality without 
  preconceived restrictions.

////////////////////////////////////////
#### Detailed Goal III: To find bugs
* Exploring the edges of the application and hitting potential soft spots 
  is a specialty of exploratory testing. The goal is purposeful, 
  rather than aimless, exploration to identify untested 
  and historically buggy functionality.

* Exploratory testers should not 
  simply stumble across bugs, they should zero in on them with purpose and intent.

Note:
That is, the test executors should bearing in mind that goal of this action is to 
find bugs instead of experience the features.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### How to perform exploratory testing?
#### Basic workflow of Exploratory Testing

  * learning: collect &amp; abstract related information
  * design: ignite the sparks of testing 
  * execution: doing the test and collect the result
  * interpretation: 

////////////////////////////////////////
#### Learning
Learning: collect &amp; abstract information related to testing subject
  - learn from anything that can guide us in what to test, how to test, or how to recognize a problem
  - possible source of the learning process including existing project documentation (requirement, design spec, manual, etc), 

////////////////////////////////////////
#### Design


////////////////////////////////////////
#### Execution


////////////////////////////////////////
#### Interpretation

Separation of the testing preparation and 
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Assessment
* More detailed explanation of dimensions of Exploratory Testing.
* Covers the following topics: coverage
////////////////////////////////////////
#### Assessment: the coverage
* In a word: Varies and hard to assess
* For testers with less expertise...
  * Think about coverage mostly in terms of what they can see.
  * Cover the product indiscriminately.
  * Avoid questions about the completeness of their testing.
  * Can’t reason about how much testing is enough.
////////////////////////////////////////
* For better testers...
  * Think about coverage in many dimensions.
  * Maximize diversity of tests while focusing on areas of risk.
  * Invite questions about the completeness of their testing.
  * Lead discussions on what testing is needed.

////////////////////////////////////////
#### 

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Pros &amp; Cons

////////////////////////////////////////

#### Strength

* Customer-focused, risk-focused
* Responsive to changing circumstances
* Finds bugs that are otherwise missed
* 

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Application of Exploratory Testing

This section consists some involvement and integration of exploratory testing to the whole testing process.

///////////////////////////////////////
#### For agile teams
* Exploratory testing is especially suited to modern web application development 
using agile methods. Development cycles are short, leaving little time 
for formal script writing and maintenance. Features often evolve quickly, 
so minimizing dependent artifacts (like pre-prepared test cases) is a desirable attribute. 

////////////////////////////////////////

* If the test case has a good chance of becoming irrelevant, why write it in the first place? 

* Are you not setting yourself up for spending more time maintaining test cases than actually doing testing?
////////////////////////////////////////
#### Coexistence with planned scripted testing
* Having formal scripts can provide a structure to frame exploration,
  and exploratory methods can add an element of variation to scripts 
  that can amplify their effectiveness.
* An approach to combine them is to start with formal scripts and 
  use exploratory techniques to inject variation into them. Thus the formal scripts become extensible.
/////////////////////////////////////////
* The added element of exploratory testing to traditional scenario testing widens 
  the scope of the script to inject variation, investigation, and optional user paths.
* Sometimes also referenced as "paired exploratory testing"

Note:
The "BBST18-Paired-Exploratory-Testing.pdf" contains some other material about *paired exploratory testing*.
////////////////////////////////////////
#### 
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
<!-- .slide: data-background="#09c" id="section-q-and-a" -->
## Question &amp; Answer  <!-- .element: style="color:#eee" -->

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Theoretical concerns

#### Effective: 
////////////////////////////////////////
#### As opposite of scripted testing, no script is allowed/required.
* For some tests that are too complex to be kept in tester's mind, writing informal note before execution is preferred.
* There is no inherent conflict between ET and documentation.
* Automatic logging tools can solve part of the problem.
////////////////////////////////////////
#### How can a team without testing expert using exploratory testing?
* Since ET requires test design skill in some measure, ET management must constrain the testing problem to fit the level and type of test design skill possessed by the tester.
Note:
This is incomplete, more points are required.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

### Application concerns

////////////////////////////////////////
#### The software is so complex that a viable path for testing is hard to find.

* The tourist metaphor: exploratory testing is like to travel in a large city, an organized tour is required
* Some viable tours: 

  The Guidebook Tour, The Money Tour, The Landmark Tour, The Intellectual Tour, The FedEx Tour, The Garbage Collector’s Tour,
  The Bad-Neighborhood Tour, The Museum Tour, The Back Alley Tour, The All-Nighter Tour, The Supermodel Tour, The Couch Potato Tour,
  The Obsessive-Compulsive Tour...

Note:
This topic can be expanded into a whole representation use with careful consideration.
Detailed material are listed at [tour.md](./tour.md)
/////////////////////////////////////////
#### Track the result: how to track the result of the testing?

////////////////////////////////////////
#### Support tools: any toolkit support the ET?
* the existing tooling constraints the thinking of exploring
* some CASE tools contains sort of support for manage the ET process
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
<!-- .slide: data-background="#09c" id="section-example" -->
## Example  <!-- .element: style="color:#eee" -->

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

## Experience the exploratory testing from specific cases

* CASE I: 

* CASE II:

* CASE III:

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Case I: 
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Case II: 
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
### Case III:  

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

<!-- .slide: data-background="#09c" id="section-summary" -->
## Summary  <!-- .element: style="color:#eee" -->

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

### References
* Exploratory Software Testing: Tips, tricks, tours and techniques to guide test design.
  [ref](https://msdn.microsoft.com/en-us/library/jj620911(v=vs.120).aspx)

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

<!-- .slide: data-background="#555" id="the-end" -->
## Thanks <!-- .element: style="color:#eee" -->
the end <!-- .element: style="color:#aaa" -->