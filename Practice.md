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