<!-- the consecutive `/` and `*` are used to separate slides horizontally and vertically -->
<!-- remove all of them if the final presentation is implemented on some other platform -->

<!-- .slide: data-background="#555" id="the-beginning" -->
## Exploratory Testing <!-- .element: style="color:#eee" -->


`Jack Q` <!-- .element: style="color:#579;font-size: 0.5em" -->
****************************************

## Agenda
* [Theory &amp; Definition](#section-theory-and-definition) <!-- .element: class="fragment" data-fragment-index="1" -->
* [Question &amp; Answer](#section-q-and-a) <!-- .element: class="fragment" data-fragment-index="2" -->
* [Example](#section-example) <!-- .element: class="fragment" data-fragment-index="3" -->
* [Summary](#section-summary) <!-- .element: class="fragment" data-fragment-index="4" -->
****************************************
<!-- .slide: data-background="#09c" id="section-theory-and-definition" -->
## Theory &amp; Definition  <!-- .element: style="color:#eee" -->

****************************************
<!-- Following pages abstracted from slides provided in class. Remove them if they are useless. -->
## Basic Description

| Item         |  Description          |
|:------------:|:----------------------|
| Tag line     | Simultaneous learning, planning, and testing |
| Objective    | Simultaneously learn about the product and about the test strategies to reveal the product and its defects |
| Testers      | Explorers |
| Coverage     | Hard to access |

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

##### (Continued)

| Item         |  Description          |
|:------------:|:----------------------|
| Potential problems | Everything unforseen by planned testing techniques |
| Activities   | Learn, plan, and test at the same time |
| Evaluation   | Varies |
| Complexity   | Varies |
| Harshness    | Varies |
| SUT readiness | Medium to late: use cases must work |

****************************************

## Representative cases
* Skilled exploratory testing of the full product
* Rapid testing & emergency testing (including thrown-over-the-wall test-it-today)
* Troubleshooting / follow-up testing of defects.

****************************************

## Strengths
* Customer-focused, risk-focused
* Responsive to changing circumstances
* Finds bugs that are otherwise missed

****************************************

## Blind spots
* The less we know, the more we risk missing.
* Limited by each tester's weaknesses (can mitigate this with careful management)
* This is skilled work, juniors are not very good at it.

****************************************
<!-- The following slides are collected from Internet. Some part are repeated with contents above. -->
### What is Exploratory Testing?
> a style of software testing emphasizing the personal freedom and responsibility 
 of the individual tester to continually optimize the value of her work by treating
 test-related learning, test design, test execution, and test result interpretation 
 as mutually supportive activities running in parallel throughout the project.
 <br />-- Cem Kaner
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
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
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### Decomposing the term
the exploratory testing consists of both "exploratory" and "testing"
  - *exploratory*: emphasize on the freedom and personality of action (testing) executor.
    + often performed by individual
    + simultaneously learning from the situation and planning for next action, then perform the action instantly
  - *testing*: perform specific task with the subject testing unit and compare the result with expectation

Note:
* this section try to explain the definition of ET from its literal terms
* *exploratory* is not limited to the testing field, but also the design, development, etc.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

#### Other perspectives
* Exploratory testing is not a testing technique. It's a way of thinking about testing.
* Exploratory testing is not an equivalence to *quick testing*
* Exploratory testing is not only functional testing
* Exploratory testing can involve complex tests which required significant preparation
Note:
* Example: after bug regression, a tester may verify the fix of bug then *explore* the fixed software to search for side effects.


****************************************
### Why to perform exploratory testing?
#### Objective
   Simultaneously learn about the product and about the test strategies 
   to reveal the product and its defects
   * it is not random, but purposed
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

#### Detailed Goal I: To gain quick understanding of application
* Understand how an application works, what its interface
  looks like, and what functionality it implements.

* Such a goal is often adopted by testers new to a project or those who want
  to identify test entry points, identify specific testing challenges, 
  and write test plans. 
* This is also the goal used by experienced testers 
  as they explore an application to understand the depth of its testing needs 
  and to find new unexplored functionality.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### Detailed Goal II: To force the software to exhibit its capabilities
* The idea is to make the software work hard and to ask it hard questions 
  that put it through its paces. This may or may not find bugs, 
  but it will certainly provide evidence that the software performs the function 
  for which it was designed and that it satisfies its requirements.

* Some other test approaches may constraint the testers to perform certain actions,
  whereas the exploratory testing can be used to verify functionality without 
  preconceived restrictions.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
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

****************************************
### How to perform exploratory testing?
#### Basic workflow of Exploratory Testing

  * learning: collect &amp; abstract related information
  * design: ignite the sparks of testing 
  * execution: perform the test and collect the result
  * interpretation: learn from the test

Note:
More material can be found from [A tutorial in exploratory testing](./reference/A-Tutorial-in-Exploratory-Testing.pdf)
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### I. Learning
Learning: collect &amp; abstract information related to testing subject
  - learn from anything that can guide us in what to test, how to test, or how to recognize a problem
  - possible source of the learning process including existing project documentation (requirement, design spec, manual, etc), 

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### II. Design
design: ignite the sparks of testing 

* Designing is not scripting. The representation of a plan is not the plan.
* Explorers’ designs can be reusable.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
design activities by scenario
* design test based on a story that is motivating and credible
* The story involves a complex use of the program or a complex environment or a complex set of data.
* The test results are easy to evaluate.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### III. Execution
execution: perform the test and collect the result

##### Execution activities

* Configure the product under test
* Branch / backtrack: Let yourself be productively distracted from one course of action in order to p produce an unanticipated new idea
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
* Alternate among different activities or perspectives to create or relieve productive tension
* Vary activities and foci of attention
* Create and debug an automated series of tests
* Run and monitor the execution of an automated series of tests
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

##### Result Collection
* use automated tools to assist
* paired testing may be helpful

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### IV. Interpretation
interpretation: learn from the test
* Oracle: determine whether program passed the test
* Oracles are heuristic: they are incomplete and they are fallible.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
some heuristics of test interpretation
* **Product**: consistent with behavior of comparable functions or functional patterns within the product.
* **Comparable Products**: consistent with behavior of similar functions in comparable products.
* **A Model’s Predictions**: consistent with expectations derived from a model.
* **History**: consistent with past behavior.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
* **Our Image**: consistent with an image that the organization wants to project.
* **Claims**: consistent with documentation or ads.
* **Specifications or Regulations**: consistent with claims that must be met.
* **User’s Expectations**: consistent with what we think users want.
* **Purpose**: consistent with apparent purpose.

Note:
* Oracle: [https://en.wikipedia.org/wiki/Oracle_(software_testing)]()
****************************************
### Assessment
* More detailed explanation of dimensions of Exploratory Testing.
* Covers the following topics: coverage
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### Assessment: the coverage
* In a word: Varies and hard to assess
* For testers with less expertise...
  * Think about coverage mostly in terms of what they can see.
  * Cover the product indiscriminately.
  * Avoid questions about the completeness of their testing.
  * Can’t reason about how much testing is enough.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
* For better testers...
  * Think about coverage in many dimensions.
  * Maximize diversity of tests while focusing on areas of risk.
  * Invite questions about the completeness of their testing.
  * Lead discussions on what testing is needed.

****************************************
### Pros &amp; Cons
* Someone believes this is sort of radical
* Someone believes this is efficient and responsive
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

#### Strength
<!--presented in course slides-->
* Customer-focused, risk-focused
* Responsive to changing circumstances
* Finds bugs that are otherwise missed
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
<!--more-->
* Exploratory testing is useful for discovering new information
* Improves the skills of the tester through simultaneous learning
  since the tester can learn about the behavior and the failure
   of the system under test.
* It increases the defect detection efficiency in terms
  of defect count, defect severity levels and number of
  false defect reports.
* Pre-defined test cases are not required in
  exploratory testing which hence leads to reduced
  documentation.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

#### Blind Spots
* The less we know, the more we risk missing.
* Limited by each tester's weaknesses (can mitigate this with careful management)
* This is skilled work, juniors are not very good at it.

****************************************
### Application of Exploratory Testing

This section consists some involvement and integration of exploratory testing to the whole testing process.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### For agile teams
* Exploratory testing is especially suited to modern web application development 
using agile methods. Development cycles are short, leaving little time 
for formal script writing and maintenance. Features often evolve quickly, 
so minimizing dependent artifacts (like pre-prepared test cases) is a desirable attribute. 

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

* If the test case has a good chance of becoming irrelevant, why write it in the first place? 

* Are you not setting yourself up for spending more time maintaining test cases than actually doing testing?
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### Coexistence with planned scripted testing
* Having formal scripts can provide a structure to frame exploration,
  and exploratory methods can add an element of variation to scripts 
  that can amplify their effectiveness.
* An approach to combine them is to start with formal scripts and 
  use exploratory techniques to inject variation into them. Thus the formal scripts become extensible.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
* The added element of exploratory testing to traditional scenario testing widens 
  the scope of the script to inject variation, investigation, and optional user paths.
* Sometimes also referenced as "paired exploratory testing"

Note:
The ["BBST18-Paired-Exploratory-Testing.pdf"](./reference/BBST18-Paired-Exploratory-Testing.pdf) contains some other material about *paired exploratory testing*.
****************************************
<!-- .slide: data-background="#09c" id="section-q-and-a" -->
## Question &amp; Answer  <!-- .element: style="color:#eee" -->

****************************************
### Theoretical concerns

#### Effective: 
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### As opposite of scripted testing, no script is allowed/required.
* For some tests that are too complex to be kept in tester's mind, writing informal note before execution is preferred.
* There is no inherent conflict between ET and documentation.
* Automatic logging tools can solve part of the problem.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### How can a team without testing expert using exploratory testing?
* Since ET requires test design skill in some measure, ET management must constrain
 the testing problem to fit the level and type of test design skill possessed by the tester.

Note:
This is incomplete, more points are required.
****************************************

### Application concerns

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### The software is so complex that a viable path for testing is hard to find.

* The tourist metaphor: exploratory testing is like to travel in a large city, an organized tour is required
* Some viable tours: 

  The Guidebook Tour, The Money Tour, The Landmark Tour, The Intellectual Tour, The FedEx Tour, The Garbage Collector’s Tour,
  The Bad-Neighborhood Tour, The Museum Tour, The Back Alley Tour, The All-Nighter Tour, The Supermodel Tour, The Couch Potato Tour,
  The Obsessive-Compulsive Tour...

Note:
This topic can be expanded into a whole representation use with careful consideration.
Detailed material are listed at [tour.md](./tour.md)
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### Track the result: how to track the result of the testing?
* Session based testing
* Workflow breakdowns
* Dashboards

Note:

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
#### Support tools: any toolkit support the ET?
* the existing tooling constraints the thinking of exploring
* some CASE tools contains sort of support for manage the ET process


****************************************
<!-- .slide: data-background="#09c" id="section-example" -->
## Example  <!-- .element: style="color:#eee" -->

****************************************

## Experience the exploratory testing from specific cases

* Case Elaboration


<!-- .slide: data-background="#09c" id="section-summary" -->
## Summary  <!-- .element: style="color:#eee" -->
****************************************

### Summary of Exploratory Testing
* It is simultaneous learning, planning, and testing
* It requires some skills to perform
* It suits well with other testing techniques

Note:
Add more summary items accordingly
****************************************

### References
* Exploratory Software Testing: Tips, tricks, tours and techniques to guide test design.
  [link](https://msdn.microsoft.com/en-us/library/jj620911.aspx)
* BBST17: Exploratory testing: [PDF](./reference/BBST17-Exploratory-testing.pdf)
* BBST18: Paired Exploratory testing: [PDF](./reference/BBST18-Paired-Exploratory-Testing.pdf)
* The Nature of Exploratory Testing: [PDF](./reference/The-Nature-of-Exploratory-Testing.pdf)
* A Tutorial in Exploratory Testing: [PDF](./reference/A-Tutorial-in-Exploratory-Testing.pdf)
* Exploratory Testing: An Overview [PDF](./reference/Exploratory-Testing-An-Overview.pdf)
****************************************

### Other material
(currently not used in pervious contents)
* Exploratory Testing: A Multiple Case Study [PDF](./reference/Exploratory-Testing-A-Multiple-Case-Study.pdf)
* How is Exploratory Testing Used:A State-of-the-Practice Survey [PDF](./reference/How-is-Exploratory-Testing-Used-A-State-of-the-Practice-Survey.pdf)
* 3 Simple Tricks to Make Exploratory Testing More Efficient [link](http://reqtest.com/testing-blog/3-simple-tricks-to-make-exploratory-testing-more-efficient/)
****************************************

<!-- .slide: data-background="#555" id="the-end" -->
## Thanks <!-- .element: style="color:#eee" -->

the end <!-- .element: style="color:#aaa" -->

By Jack Q <!-- .element: style="color:#666; font-size: 0.5em" -->