# Summary 
This is a summary of the content of ASD, I recommend reading through the other notes on this repository alongside this.

# Introduction
## Software Engineering (SE)
> establishment and use of effective engineering principles to create software that is reliable and works efficiently on real machines
> Application of a systematic, disciplined, quantifiable approach to the creation, operation and maintenance of software

### Elements of SE
* Requirement gathering
* Design
* Documentation
* Coding
* Testing
* Bug fixing

### Process of SE
* Definition
* Development
* Support

# Project Management
## Planning
* Project Scope
    * Defining scope
        * Narrative: narrative description of software based on what stakeholders say
        * Use cases: stories describing user interaction with software, from user POV
    * Determine feasibility
        * Given the scope, determine the resources required
    * Project Planning Goals
        * AKA Scope
        * Create measurable goals
            * S - Specific
            * M - Measurable
            * A - Agreed upon
            * R - Realistic
            * T - Time boxed
    * Deliverables - list of items to be delivered to meet goals
    * Schedule
        * Effort required (in terms of time)
        * If schedule is unrealistic you can do the following:
            * Renegotiate deadline
            * Additional resources
            * reduce scope
    * Supporting Plans
        * HR Plan
            * Name key individuals and organisations: describe roles and responsibilities 
        * Communication & Management Plan
            * Who needs to be informed about the project
            * How will they receive the information
                * Weekly review meeting
                * Progress reports
                * Revised schedule
        * Risk Management Plan
            * Identify as many risks as possible
            * Be prepared if something bad happens
        * Marketing Plan

* Management Activities
    * People
        * Managers, PM, Team Leads, Customers, End-users
    * Product
        * Scope/Decomposition
    * Process
        * SDLC
            * Initiation -> Analysis -> Design -> Construct -> Test -> Implement
        * UP
            * Inception -> Elaboration -> Construction -> Transition -> Production
    * Project
        * Size estimation, scheduling, risk management, tracking

> The 4 P's

* People
    * Roles and Responsibilities
        * Project Management
        * Systems Analysis
        * User Interface Designer
        * Architect
            * Middleware
        * Specialists
        * Documentation
    * Essential Roles
        1. Course Developer
        2. Database Designer
        3. Implementer
        4. Integrator
        5. Process Engineer
        6. Project Manager
        7. Project Reviewer
        8. Software Architect
        9. Systems Administrator
        10. Systems Analyst
        11. System Tester
        12. Test Manager
        13. UI Designer
    * Management and Team Success
        * Software Engineering is a group activity
        * Individual success depends:
            * Ability and interest to work hard etc
        * Team success depends on:
            * Ability to communicate and express ideas in the team
            * Group interaction is a key determinant of group performance
        * Management Skills

* Estimation and Metrics
    * Milestones and Deliverables
        * Activity - Task that takes time
            * Duration
            * Due date
            * Precursor
        * Milestone
            * Completion of an activity
            * Recognizable end-product of a task
            * Requires a formal output
        * Deliverable
            * A project result that is delivered to a customer
        * Milestone vs deliverable
            * Deliverable is a measurable and tangible outcome of the project. They are developed by project team members in alignment with the goals of the project
            * Milestones on the other hand are checkpoints throughout the life of the project. They identify when one or multiple groups of activities have been completed thus implying that a notable point has been reached in the project
    * Software Metric Characteristics
        * Process Metrics
            * Some aspect of the development process
        * Product Metrics
            * Some aspect of the software product
        * Result Metrics
            * Measure outcomes
        * Predictor Metrics
            * quantify estimates for project resource requirements
    * Are they worth anything?
        * Yes
        * Useful for prediction
        * Size metrics used for resource requirements
    * Why do we use them?
        * To plan and manage software development projects
## Scheduling
* Split the work in a project into separate tasks
* Network Analysis
    * Label tasks in order and indicate dependencies
    * Fill in earliest start, earliest finish
    * Fill in latest start, latest finish
    * Fill in total float
    * Fill in free float
* Gantt Charts
## Risks
* 3M's
    * Mitigation
    * Monitoring
    * Management
* Risk Matrix
    * Probability
    * Impact
* Boehm's Top Ten Risks
    1. Personnel shortfalls
    2. Unrealistic schedules and budgets
    3. Developing the wrong functions
    4. Developing the wrong user interfaces
    5. Gold-plating
    6. Continuing stream of requirements changes
    7. Shortfalls in externally-performed tasks
    8. Shortfalls in externally-furnished components
    9. Real-time performance shortfalls
    10. Straining computer science capabilities

## Planning vs Management
* Planning
    * Pre/Post
    * Network analysis, resourcing
* Management
    * During
    * Controlling resources and timescales
# PM Methods
## Triangle

![Triangle](img/softwaretriangle.png)

## YAGNI - You Ain't Gonna Need It
* Build only what you need now
## Software Entropy
* Entropys is a measure of disorder in a physical system
* Software based entropy is the measure of code complexity
    * Tends to increase over time
## Yak Shaving
## Traditional SE MEthods
### Waterfall
* Analysis
* Requirement Specification
* Design
* Implementation
* Testing and Integration
* Operation and Maintenance

These all happen linearly
## Modern Alternatives
* More lightweight
* Iterative
* Agile Software Development
* Rapid Application Development
* Extreme Programming
* Scrum
# Agile Development
Agile is a set of values and principles
## Principles of Agile Methods
| Principle            | Description                                                     |
| --- | --- |
| Customer Involvement | Customers should be closely involved throughout the development process. Their role is to provide and prioritize new system requirements and to evaluate the iterations of the system |
| Incremental Delivery | The software is developed in increments with the customer specifying the requirements to be included in each increment.                                                               |
| People not process   | The skills of the development team should be recognized and exploited. Team members should be left to develop their own ways of working without prescriptive processes.               |
| Embrace Change       | Expect the system requirements to change and so design the system to accommodate these changes                                                                                        |
| Maintain Simplicity  | Focus on simplicity in both the software being developed and in the development process. Wherever possible, actively work to eliminate complexity from the system.                    |

## Pareto's Law
* Typically 70% of your results come from 20% of your efforts