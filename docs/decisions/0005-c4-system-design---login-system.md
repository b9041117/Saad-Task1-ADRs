# C4 System Design - Login System

## Context and Problem Statement

## Status
Accepted

## Context
During the development of my C4 Diagrams I came across an issue regarding whether or not to include a Login system within the scope of the application. As sprawl began to creep in a re review of the fundemental requirements of the system was needed. Therefore a decision must be made whether to make the login system out of scope for the AFS system or remain in scope.

## Considered Options

* Keep the Login System within Scope
* Remove the Login system from the scope and make it an external system

## Decision Outcome

Chosen option: "Remove the Login system from the scope and make it an external system", because helps to stop sprawl of the system and keep it focused on the core functionality

## Pros and Cons of the Options

### Keep the Login System within Scope

This will keep the login system as a core feature of the AFS system

* Good, because It allows the login system to remain within the AFS application ecosystem
* Bad, because It is not explicitly within the requirements to have a log in system

### Remove the Login system from the scope and make it an external system

Remove the login system from the AFS application and treat it as an external system that can be utilised by the AFS System

* Good, because It helps to reduce software creep and cut down on development time
* Good, because It would help to focus on the core functionality of the system
* Bad, because Less features for the AFS System

## Links

* https://www.atlassian.com/microservices/microservices-architecture/software-sprawl
