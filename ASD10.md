# Design Patterns
## Class Design and Unified Process Terminology
* Typical information in a Design Class Diagram includes:
    * Classes, associations and attributes
    * Interfaces (with operations and constants)
## Applying Composite Pattern to UI Widgets
*  The Swing Component hierarchy is a Composite
    *  Leaf widgets (e.g.: Checkbox, Button, Label) specialize the component interface
## Facade Pattern
* Define a single point of contact to the subsystem - a facade object that wraps the subsystem. 

## Observer Pattern
* Generalization of the MVC pattern
    * Want to display data in more than one form at the same time and have all of the displays reflect any changes in that data
* Assumes the object containing the data is separate from the objects which display the data,
    * These display objects observe changes in that data
* Liabilities/Concerns
    * Possible cascading of notifications
    * Observers are not aware of each other and must be careful about triggering updates
    * Simple update interface requires observers to deduce changed item
## Designing for Low Representational Gap
* Normally we design for a low representational gap between real world and software
* Typically designed objects typically correspond to real world objects
* But (contra-indication):'
    * Don't design for low representational gap regarding actors
    * E.g.: we don't make a software class Clerk do all the work in the software system
* Exercise: why?
    * Actors do more than one specific class
    * It may be sensible to talk about one specific actor
    * Seperating it out into multiple classes
# Patterns
## Summary
* Principles (expressed in *patterns*) guide choices in where to assign responsibilities
* A *pattern* is a named
# Resources
* GRASP (General Responsibility Assignment Software Patterns)
    * Larman
* Gang of Four  