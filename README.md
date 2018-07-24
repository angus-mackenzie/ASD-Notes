# CSC3003S Notes
# Lectures
## Lecture 1
### Advanced Software Development
JonJon Clark - clrjon005@myuct.ac.za
**Topics**
* Requirements Gathering
* Software Design
* Documentation
* Coding
* Testing
* Bug Fixing
### The Process of Software Engineering
**Definition**
* The establishment and use of effective engineering principles in order to obtain software that is reliable and works efficiently on real machines.
* The application of a sytematic, disciplined, quanitifiable approach to the development, operation, and maintenance of software.
### Topics
1. Review O-O & UML
2. Project Management
3. Software Development Methodologies
4. Agile Software Development
5. Software Development with SCRUM
6. Case Study: SCRUM in Game Development
7. UML, Patterns and Architecture
8. Software Architecture
9. Design Patterns
10. Open Source
11. Validation/Verification
### Guest Lectures Thursdays
### What is version/source control?
• Version control systems are a category of software tools that
help a software team manage changes to source code over
time.
• keeps track of every modification to the code in a special kind
of database
• If a mistake is made, developers can turn back the clock and
compare earlier versions of the code to help fix the mistake
while minimizing disruption to all team members
### source Control
Managing a codebase with lots of simultaneous contributors
|Distributed|Centralized|
|---|---|
|Mercurial (hg),git| CVS, Subversion|
|Work in local repository, sync changes later | Repository exists on a client server, work on clients|
### Web-based hosting service for version control using Git
* Bitbucket
* Github
* [Gitlab](gitlabcs.uct.ac.za)
## Lecture 2
### Advance Software Design: Project Management
* Concerned with activities involved in ensuring software is delivered on time and on schedule and in accordance with the requirements of the organisations developing and procuring the software.
* Project management is needed because software development is always subject to the **budget and schedule constraints** that are set by the organisation.
* Read [Bennet Chapter 22](/docs/BennetChapter22.pdf)
* Systems Development is a complex activity that requires careful project management
* Inter-dependencies between the artefacts of softwaree development
    * production has to be planned, monitored and co-ordinated
    * So that software development is efficient, effective and on time.
    * E.g.: when would you start build the Chess AI?
* A software development project may involve many developers, some with specialized skills who will be required at different times.
* Activites must follow a particular sequence.
    * For example,  testing a system can only begin when at last some elements have been constructed.
    * Test scripts and test harness may be prepared earlier in the project
### No Silver Bullet
There is no technique that fixes the inherent complexity of software design and development.
### Project Management Tools
* Basecamp
* Freedcamp
* TeamGantt
* Asana
* Overleaf
### Scope of a Project
* The functions and features that are to be delivered to end-users
* The data that are input and output
* The content that is presented to users as a consequence of using the software
* The performance, constraints, interfaces and reliability that bound the system
### Defining SCope
* Scope is defined using one of two techniques
    * A narrative description of software scope is developed after communication with stakeholders
    * A set of use-cases is developed. A use-case is a scenario-based description of the user's interaction with the software from the user's point of view.
* Performance considerations encompass processing and response time requirements.
* Constraints identify limits placed on the software by external hardware, available memory, or other existing systems.
### Determining Feasibility
* Given the scope, determine the resources required.
    * Cost
* Make sure you have an answer to the question:
    * Do we have the resources we need to build this software?
* Resources are:
    * People
    * hardware and software tools
    * reusable components.
### Project Planning Goals - Aka scope
* Goals are derived from the needs and expectations of stakeholders:
    * Project sponsor
    * customer for deliverables
    * Users of the project outputs
    * project manager and project team
* Find true needs that create real benefits
    * Prioritize them
* Create measurable goals
    * S - Specific, significant, stretching
    * M - Measurable, meaningful, motivational
    * A - Agreed upon, attainable, achievable, acceptable, action-oriented
    * R - Realistic, relevant, reasonable, rewarding, results-oriented
    * T - time-boxed, time-based, time-bound-timely, tangible, trackable.
### Project Planning Deliverables
* Deliverables are a list of items that have to be delivered to meet the goals
    * Verifiable and specific
    * Can be report, equipment acquisition or Executable code module etc
    * Has a stakeholder who needs it
* Say when it has to be delivered
* Give quality standards
    * document is according to specified format
### Project Planning Schedule
* The effort required (in terms of time)
* The people required (and other resources)
* Update deliverables with this & work schedule out
* If the schedule is unrealistic you can justify some of the following:
    * Renegotiate deadline - delay
    * Additional resources - more expensive
    * reduce scope - fewer deliverables (only thing that makes sense for capstone - carefully determine your scope)
### Project Planning Supporting Plans
Human Resource Plan
* Name key individuals and orgs: describe rols and responsibilities
* Describe the number and type of people needed
    * Start dates etc

Communication and Management Plan
* Who needs to be kept informed about the project
* How they will receive the information?
    * Weekly review meeting
    * progress reports
    * revised schedule
  
Risk Management Plan
* Identify as many risks as possible
* Be prepared if something bad happens

Marketing Plan
* Important to get funding

### The Range of Management Activities
**P**eople
* Managers, Project Managers, Team Leaders, Software Team, Customers, End-Users
**P**roduct 
* Scope and decomposition
**P**rocess
* SDLC: initiation -> Analysis -> Design -> Construct -> Test -> Implement 
* UP: Inception -> Elaboration -> Construction -> Transition -> Production
**P**roject
* Size estimation, scheduling, risk management, tracking

### People
#### Roles and Responsibilities
It seems obvious that a team needs people with different skills
* Range of duties in a small project
    * Project management: Strategist, Leader, Politician, Project Facilitator, Administrator
    * Systems analysis: Stakeholder needs, Interaction Designer, Cost estimator
* User interface designer, user stories
* Architect: Application overview, performance
    * Middleware —software layer between the operating system and the applications on a distributed computer network
* Specialists as required: database, games engine, mobile development, …
* Documentation: Amanuensis

##### Essential Roles in Small Software development teams
1. Course developer - prep and coordination of training.
2. Database designer - essential to the process, mainly due to the specific nature of its knowledge
3. Implementer - programs sub-systems and components that support
4. Integrator (lead programmer) - responsible for maintaining the implementer' awareness of the project context, for identifying the tasks to be undertaken and for appointing th eperson responsible for each one. Also responsible for the initial definition of the critical dates of the project and for developing a plan for the integration of the sub-systems, to allow the project manager to inform th eclient when each feature is expected to be available.
5. Process Engineer - mainly concerned with the management of the dev process, its adaptation to org context and monitoring its implementation, in order to identify and implement process improvements.
6. Project Manager - Assume a global overview of the project through a detailed interaction with the internal and external participants. Must create the conditions for the project to achieve success, by ensuring timeliness and fulfilment of all commitments. Requires: basic knowledge in management; knowledge about the client’s business domain; project management methodologies and negotiation skills.
7. Project reviewer -  This role cannot be considered critical, however, due toresponsibilities related to the verification and approval of several artefacts produced by other participants, and possible conflict of interests, this person cannot have another role within the project
8. Software Architect -  Responsible for setting the technological foundation onwhich the project implementation should be based. The software architect is responsible for managing the technical risks.
9. Systems Administrator -  Focused on ensuring the provision of the infrastructure needs (e.g., PCs for developers, servers, etc.)
10. Systems Analyst - Scope management. Identify and document the requirements (functional or non-functional). Understand the client'sbusiness domain and to perceive the real motivations and relevance of the requirements.
11. System tester - Entrusted with very different tasks, like review of documentation and testing behaviour. 
12. Test Manager - Responsibility is to ensure the product quality by devising a plan for internal quality audits and implementation. Cannot have other roles, particularly with those roles related to the design and construction.
13. UI designer - The scope of this role in a project varies according to the nature of the artefacts to be developed.
#### Choosing People
* Information from candidates about their background and experience
    * Best evidence to judge suitability
#### Managing with different Personality Types
* Backgrounds and personality styles of team members
* Management styles of customers and developers
* Realize tha other people are not like you
#### Management and Team Success
* Most software engineering is a group activity
    * Non-trivial software projects cannot be done by one person
    * People motivated by success of the group and their own personal goals
* Individual success depends on:
    * Ability and interest to work hard
### Estimation and Metrics
#### Milestones and Deliverables
