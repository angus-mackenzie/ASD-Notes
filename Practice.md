# Practice
This document has some question, answer pairs and was used to gain further insight into how this topic was tested within the university.
# Test 1 2017
*Section 1 - Project Management*</p>
**Question 1**</p>
1. How do you set out to manage risks at the start of the project? (4)
2. List the 3M's of risk management and explain what they entail (6)
<details>
<summary>1.1</summary>

1. Identify project specific risks
2. Analyze the risks
3. Rank them in a particular order
4. Plan for the monitoring, mitigation and management of these risks 
</details>
<details>
<summary>1.2</summary>

* Mitigation - avoiding or reducing the risk by changing requirements or transferring the risk (by buying insurance, etc), or assume the risk and put in measures to control it
* Monitoring - what factors can we track that will enable us to determine if the risk is becoming more or less likely
* Management - what contingency plans do we have that will enable us to determine if the risk is becoming more or less likely.
</details>

**Question 2**</p>
1. Consider the following principles of Extreme Programming (XP) and briefly describe each principle (0.5 each)
    * Incremental Planning
    * Small Releases
    * Simple Design
    * Test-first Development
    * Refactoring
    * Pair Programming
    * Collective Ownership
    * Continuous Integration
    * Sustainable Pace
    * On-site customer
2. Describe test-driven development (4)
3. List some of the benefits of pair programming (3)

<details>
<summary>2.1</summary>

* Incremental Planning - requirements are recorded on story cards and the stories to be included in a release are determined by the time available and their relative priority. The developers break these stories into development 'Tasks' 
* Small Releases - the minimal useful set of functionality that provides business value is developed first. Releases of the system are frequent and incrementally add functionality to the previous release.
* Simple Design - enough design is carried out to meet the current requirements and no more.
* Test-first Development - an automated unit test framework is used to write tests for a new piece of functionality before that functionality itself is implemented.
* Refactoring - all developers are expected to refactor the code continuously as soon as possible code improvements are found. This keeps the code simple and maintainable.
Pair Programming: Developers work in pairs, checking each other’s work and providing the support to always do a good job.
* Collective Ownership - the pairs of developers work on all areas of the system, so no islands of expertise develop and all the developers take responsibility for all of the code: anyone can change anything.
* Continuous Integration - as soon as the work on a task is complete, it is integrated into the whole system. After any such integration, all the unit tests in the system must pass.
* Sustainable Pace - large amounts of overtime are not acceptable as the net effect is often to reduce code quality & medium term productivity
* On-site Customer - a representative of the end-user of the system (the customer) should be available full time for the use of the XP team. In an extreme programming process, the customer is a member of the development team and is responsible for bringing system requirements to the team for implementation.

</details>

<details>
<summary>2.2</summary>

* TDD can be described as 
    * TDD = TFD + Refactoring
* TDD turns traditional development around
    * Instead of writing functional code first and then your testing code an afterthought
    * You first write your test code before your functional code
* Also you do so in very small steps
    * One test and a small bit of code at a time
* With TDD a developer refuses to write a new function unless there is a test that fails because that function isn't present
    * Refuse to add even a single line of code until a test exists for it
* Once the test is in place do the work required to ensure that the test suite now passes
* Once your code works, refactor it to ensure that it remains of high quality
</details>

<details>
<summary>2.3</summary>

* Productivity is similar to that of two people working independently
* Common ownership of code
* Collective (team) responsibility for the system
* Spreads knowledge across the team
* Reduces risk if someone leaves
* Motivates refactoring as the whole team will benefit from it
</details>

*Section 2 - Architecture*</p>
**Question 3**</p>
1. Briefly describe the pipe and filter architecture and draw a diagram to illustrate it (6)
2. How can the pipe and filter architecture be generalized, what is it then called? (2)
3. We discussed several architecture patterns in the duration of this course. What is the key aim of these patterns? Define any new terms that you introduce during your explanation. (4)


<details>
<summary>3.1</summary>
A system is decomposed into a set of functional transformations that consume inputs and produce outputs. Data flows from one function to another (the pipeline) and is transformed as it passes through the sequence

![Pipe And Filter](img/pipeandfilter3.png)

</details>

<details>
<summary>3.2</summary>
It can be generalized to have branching pipes connecting filters. It is then called the Data Flow Architecture
</details>

<details>
<summary>3.3</summary>

The key aim of architectural patterns is to minimize coupling while maximising cohesion.
* Cohesion is the degree to which communication takes place within the module 
* Coupling is the degree to which communication takes place between modules

You could also explain this in terms of the *separation of concerns and localization of impact*.
</details>

**Question 4**</p>
Many personal computer applications are event processing systems
1. Why are they called *event processing systems*? (1)
2. What is the key characteristic of *event processing systems* that impacts the architecture (2)
3. Please describe a high-level view of data processing systems (3)

<details>
<summary>4.1</summary>
They respond to events in the environment of the system
</details>

<details>
<summary>4.2</summary>
Their key characteristic is that event timing is unpredictable so the architecture has to be organised to handle this
</details>

<details>
<summary>4.3</summary>
Data processing systems are data-driven and operate in batch mode and generally have an input-process-output structure. Records are inputted to the system, information is processed and outputs are generated
</details>

# Test 1 2018
*Section 1 - Project Management*</p>
**Question 1**</p>
1. You are a project manager (PM). An activity on the critical path is behind schedule. You hve no additional resource available. What do you do? (3)
2. You are the PM and have successfully determined your scope. In addition to your project plan, you have several supporting plans. One of them being a risk management plan. Name another appropriate supporting plan and the purpose of it? (3)

<details>
<summary>1.1</summary>

Two major options:
* Move the project deadline to accommodate the delay
* Reduce the scope of the project

Both of these have to be discussed with the client
</details>

<details>
<summary>2.2</summary>

Human Resource plan.
* Name key individuals and organisations: describe roles and responsibilities
* Describe the number and type of people needed

Communication and Management plan
* Necessary for keeping requisite people informed about the project.
* Clarify how they will receive this information
    * Frequency
    * Medium

Marketing plan
* Go to market strategy
    * Target market, releasing content freely or as paid DLC, promotion, etc

</details>

**Question 2**</p>
1. One of the few artefacts required in Scrum is the *Burndown Chart*. What is it and what does it provide? (3)
2. What is test driven development? Highlight how it differs from more traditional software development methods. (5)
3. Name a traditional software development method (1)

<details>
<summary>2.1</summary>

A burndown chart tracks the progress of a sprint. It is a graphical plot of work left to do in a sprint against time. It can be used to identify the rate that work is being completed - which is known as velocity. It can give indications that work is too slow, or that things are quicker than expected
</details>

<details>
<summary>2.2</summary>
Test Driven Development (TDD) can be described as test first development + refactoring. TDD turns traditional development around and instead of writing functional code first and then testing your code, you first write your test code before your functional code. In addition, the development occurs in very small steps: one test and a small bit of code at a time. Once the code passes the test it is refactored to ensure it remains of high quality.

The radical point is that new code is only written when an automated test fails.
</details>

<details>
<summary>2.3</summary>
Waterfall method
</details>

*Section 2 - Architecture*</p>
**Question 3**</p>
1. What is meant by software architecture? (2)
2. Indicate whether the following statements are True or False
    1. In agile development, architectures should be developed incrementally (1)
    2. When designing complex applications, a single architectural model is mostly used (1)
3. Briefly describe pipe and filter and draw a diagram to illustrate it (7)

<details>
<summary>3.1</summary>
Multiple answers, but here are three:

The software architecture of a program or computing system is the structure
or structures of the system, which comprise software components, the externally visible
properties of those components, and the relationships among them.

Or IEEE: The fundamental concepts or properties of a system in its environment
embodied in its elements, relationships, and in the principles of its design and evolution.

Or outline: software architecture ≡ “the set of principal design decisions about the
system”. It is about the BIG picture; the large scale: motivations, constraints,
organization, patterns, responsibilities, connections of a system (or a system of systems)
</details>

<details>
<summary>3.2.1</summary>
False
</details>

<details>
<summary>3.2.2</summary>
False
</details>

<details>
<summary>3.3</summary>
A system is decomposed into a set of functional transformations that consume inputs and
produce outputs. Data flows from one function to another (the pipeline) and is
transformed as it passes through the sequence.

![Pipe](img/pipeandfilter3.png)
</details>

**Question 4**</p>
1. Which kind of UML diagram is most commonly used for logical layered architectures? (1)
2. Name two layered reference architectures use in networking (2)
3. Which programming language constructs are used to implement the concept of type? (2)
4. Explain what is meant by *high cohesion*
5. What is a very commonly used run-time organization pattern for distributed systems, particularly over the internet?
6. Briefly explain the concept of *low representational gap* when designing classes and objects

<details>
<summary>4.1</summary>
Package Diagram
</details>

<details>
<summary>4.2</summary>
OSI & TCP/IP
</details>

<details>
<summary>4.3</summary>
Abstract Classes & Interface
</details>

<details>
<summary>4.4</summary>
Cohesion is a measure of how strongly related and focused the responsibilities of an
element are. A class with low cohesion does many unrelated activities or does too much
work. A class with high cohesion has a relatively low number of methods with highly
related functionality and doesn’t do much work.
</details>

<details>
<summary>4.5</summary>
Client Server
</details>

<details>
<summary>4.6</summary>
Classes/objects should closely correspond to real world objects
</details>