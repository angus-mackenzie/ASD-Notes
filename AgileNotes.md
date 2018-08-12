#### Refactoring when Developing Software
* Try to add a new function
    * (oops) realize this would be much easier if the code were structured differently
* Refactor for a while 
    * The code is better structured
* Add the new function
    * get the new function working
        * it is coded in a way thats awkward to understand
        * so refactor
#### Examples of Refactoring
* Re-organization of a class hierarchy to remove duplicate code
* Tidying up an renaming attributes and methods to mkae them easier to understand
* The replacement of inline code with calls to methods that have been included in a program librarysnio

Initial Classes - Video Rental

![Example](img/refactoringex1.png)

Refactored Classses Video Rental

![Example](img/refactoringex2.png)

#### Why Refactor
##### Improves the Design of Software
* Deal with Software rot, decay and loss of structure
* Refactoring is like tidying up the code
    * Regular refactoring helps code retain its shape
    * You refactor code that works but is not ideally structured
* An important aspect of improving design is to eliminate duplicate code
    * Ensure the code says everything once and only once
    * More code <=> harder to modify correctly <=> mode code to understand
    * Change this bit of code here, but the system doesn't do what is expected becuase you didn't change that bit over there that does much the same thing in a slightly different context.
* Changes are easier to make becaus ethe code is well-structured and clear
##### Makes Software Easier to Understand
* Improve the understandability and readability of the software
    * Reduces the need for documentation
    * Good programmers write code understandable by human beings
* After code is written it has to be maintained
    * Someone will try to read the code and make changes
    * It matters if it takes a programmer a week to make a change that would have taken an hour if she had understood your code
* When you are trying to get the program to work, you are not thinking about that future developer
    * It takes a change in rhythm to make changes that make code easier to understand
    * Refactoring leads to higher levels of understanding that would otherwise be missed during development
##### Helps find bugs
* By clarifying the strucutre of the program you clarify certain assumptions you've made
    * To the point at which even you can't avoid spotting bugs
* Kent Beck often says about himself:
> I'm not a great programmer; I'm just a good programmer with great habits
* Refactoring helps me to be much more effective at wiritng robust code
##### Helps you program faster
* Good design is essential for rapid software development
* Changes take longer as you try to understand the ystem and find the duplicate code
* New feature need more coding as you patch over a patch that patches a patch on the original code base
* Refactoring helps you develop softwar more rapidly, because it stops the design of the system from decaying
* It can even improve a design
#### Refactoring Categories
1. Composing methods
    * The refactorings serve restructurings at the method levle
2. Moving features between objects
    * These refactorings support the moving of methods and fields between classes
3. Organizing data
    * These refactorings restructure the data organisation
4. Simplifying conditional expressions
    * These refactorings simplify conditional expressions
5. Making method calls simpler
    * These refactorings simplify method calls
6. Dealing with generalization 
    * These refactorings help to organise inheritance hierarchies
#### Refactoring to Patterns
* Refactoring to Patterns is the marriage of refactoring with patterns
    * Patterns $\equiv$ classic solution to recuring design problems
* Use patterns to improve an existing design
    * Better than using patterns early in a new design
* This is compatible with XP's desire to avoid too much upfront design
### Conclusion
* The traditional view is that refactoring is a waste of resources
#### Collaboration with Users
* Agile development relies on close cooperation and collaboration between all team members and stakeholders.
    * Keep requirements and documentation lightweight
    * Acknowledge that change is a normal and acceptable reality in software development
    * Required to clarify requirements just-in-time
    * Keep all team members on the same page throughout the development
* You can't do away with a big spec up-front and not have close collaboration
#### Agile method applicability 
* Product development where a software company is developing (medium-sized) product for sale
* Custom system development within an organisation, where there is a clear commitment from the customer to become involved in the development process and where there are not a lot of external rules and regulations that affect the software
#### Problems with agile methods
* It can be different to keep the interest oc customers who are involved in the process
* Team members may be unsuited to the intense involvement that characterizes agile methods
* Prioritising changes can be difficult where there are multiple stakeholders
* Maintaining simplicity requires extra work
* Contracts may be a problem as with other approaches to iterative development
* Because of their focus on small, tightly-integrated teams, there are problems in scaling agile methods to large systems
#### Agile methods and software maintenance
* Most organisations spend more on maintaining existing software than they do on new software development
    * So agile methods have to support maintenance as well as original development
* Two key issues
    * Are systems that are developed using an agile approach maintainable, given the emphasis in the development process of minimizing formal documentation?
    * Can agile methods be used effectively for evolving a system in response to customer change requests?
* Problems may arise if original development team cannot be maintained
#### Plan-driven specification and development
* A plan-driven approach to software engineering is based around separate development stages with the outputs to be produced at each of these stages planned in advance
* Not necessarily waterfall model, plan-driven, incremental development is possible
* Iteration occurs within activities

![Plan Driven](img/specanddev.png)

#### Agile specification and development
* Specification, design, impementation and testing are inter-leaved
* Outputs from the development process are decided through a process of negotiation during the software development process

![Specficiation and Dev](img/specanddev2.png)

#### Architecture Change and Refactoring
* Changes that require architecture refactoring is very expensive
* It is hard to do
* It has consequences for the code and implies code refactoring
#### Summary - Points to consider
##### Principles of Agile Methods
1. Active user involvement is imperative
2. The team must be empowered to make decisions
3. Requirements evolve but the timescale is fixed
4. Capture requirements at a high level, lightweight and visual
5. Develop small, incremental releases and iterate
6. FOcus on frequent delivery of product
7. Complete each feature before moving on to the next
8. Apply 80/20 rule
9. Testing is integrated throughout the project lifecycle - test early and often
10. A collaborative & cooperative approach betwen all steakholders is essential
##### Active User Involvement
* Requirements are clearly communicated and understood at the outset
* Requirements are prioritized appropriately, based on the needs of the user and market
* Requirements can be clarified daily with the project team, not from lengthy documents that arent read or are misunderstoood
* Emerging requirements can be factored into the development schedule with the impact and trade-off decisions understood
* The right product is delivered
* As iterations are delivered, check they meet user expectations
* The product is more intuitive and easy to use
* The user is seen to be interested in the development
* The user/business sees the commitment of the team
* Developers are accountable, share progress openly every day
* There is complete transparency as there is nothing to hide
* The user shares responsibility for issues arrising; it is not a customer-supplier relationship but a joint team effort
* Timely decisions can be made about features, priorities, issues, and when the product is ready
* Responsiblity is shared; teh team is repsonsible together for the delivery of the product
* When the going gets tough, the whole team - business and technical - work together!
##### Fixed Timescale
* No-one knows what the right solution is at the outset
    * Its practically impossible to build the right solution initially
* Traditional project fight change, with change control processes
    * Minimise and resist change wherever possible
* Agile development embraces and expects change
    * The only thing that is certain in life is change
    * Requirements are allowed to evolve, but the timescale is fixed
        * To include a neq requiremnt, or to change a requirement, the user must remove a comparable amount of wokr
    * Assumes there are enough non-mandatory features included in the original timeframes.
##### Agile Requirements are Barely Sufficient
* Contrast this to the traditional situation
    * User still has new and cahnged requirements
        * Expects the new and existing features to be delivered in the original timeframes
* Teams that don't control changes can end up with scope creep
    * One of the most common reasons for projects to fail
* Agile teams accept change and even expect it
##### Agile Development Cycle
###### Frequent Delivery 
* Agile development is about frequent delivery of products
    * Gone are 12 month projects
    * a 3-6 month project is strategic
* Consider web
    * Products are released early with basic features
    * In the web 2.0 its perpetual beta
        * derive some benefits early
        * get feedback
        * look at metrics -> find what works/doesn't
        * before building "everything"
###### Regular Release Cycle
* Allows you to learn more effectively
* Estimates might be good or bad but they should be consistent
    * Estimate features at a granularity of less than 1 day and track your performance
    * You'll begin to udnerstand your delivery rate
    * You'll be surprised at how predictable you cab be
* Managing expectations is about predictability
    * If people know what to expect, they're gnerally happy
    * If they don't theyre not happy
* Focus on frequent delivery of product
* Even more importantly, focus on consistent delivery
##### eXtreme Programming (XP)
1. Whole Team: remove barrier between customer and the rest of the dev team
2. Metaphor: Common analogy for the system
3. Planning Game: planing specifies the next step
    * As the project progresses get a better and better picture of what will be accomplihed
    * Client expresses goals through user stories - overall behaviours of the software
    * Development takes storeis and estimates costs
    * Client prioritises stories
4. Simple design - as simple as the current level of functionality allows. No extraneous complexity allowed
    * When the code becomes too unwieldy its time for refactoring 
    * Design only extend to the next iterations new features
5. Small Releases: XP development teams release tested, working code, very frequently
    * Each iteration - 2 weeks - the client gets new code
    * Client evaluates it and dictates the next delivery
6. Consumer Test - The customer develops acceptance tests to see if software meets user stories
    * Tests are automated and used frequently by the developers
7. Pair Programming
8. Test Driven Development
9. Design Improvement - refactoring code whenever deficiencies are noticed = improving the design of the existing code
10. Collective code ownership: immaterial who wrote the code; anyone can modify it at any time
    * Whoever notices a problem, fixes it
11. Continuous Integration: At all times the system compiles, runs and passes all tests
12. Sustainable Pace: Same amount of work and effort in every iteration
    * Overtime leads to burnout, mistakes and more burnouts
13. Code standard - adopt some coding standard that is consistently adhered to
##### TDD
* Programming technique ensuring that code is thoroughly unit tested if a test fails then progress has been made: you know what to fix
    * Clear measure of suxxess when the test no longer fails
* TDD increases confidence that the system meets the requirements
* Side effect of TDD is you achieve 100% coverage test
    * Every single line of code is tested
    * Not guaranteed with traditional testing
* Does not replace traditional testing: just effective unit testing
* Side effective of TDD: the resulting tests are working examples for invoking the code -> provides a working spec for the code
