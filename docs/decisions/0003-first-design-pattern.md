# First Design Pattern

## Context and Problem Statement

## Status
Accepted

## Context
After choosing to use a Microservices architectural style for the AFS System there were some issues that required the aid of some design patterns to solve. These included how to ensure each service can communicate with the rest of the system and how to ensure that services are alerted to outside changes/processes.

## Considered Options

* Event Drive Design Pattern
* Command Query Responsibility Segregation (CQRS)
* Service Registry

## Decision Outcome

Chosen option: "Event Drive Design Pattern", because it allows for the microservices to remain decoupled, while also enabling them to act on real time changes to the system

## Pros and Cons of the Options

### Event Drive Design Pattern

Uses events to communicate and activate between different decoupled services

* Good, because Works well with Microservices Architectural Style
* Good, because Increase Scalabilty as more event consumes can be added to the system horizontally
* Good, because Makes the Microservices even more loosely coupled and less dependent on each other
* Bad, because Increases complexity
* Bad, because Increases difficulty in monitoring, debugging and troubleshooting

### Command Query Responsibility Segregation

Seperates the read and write queries for each database

* Good, because Seperation of the read and write increases the speed of both
* Good, because Have two seperate database for Read and write operations
* Bad, because Complex implementation
* Bad, because Increases in database can increase the failure rate

### Service Registry

Each microservice registers themselves with the service registry acts and it allows services that require one another to query the register to find it's location

* Good, because Simple Implementation
* Bad, because It couples every service to the register

## Links

* https://aws.amazon.com/event-driven-architecture/#:~:text=An%20event%2Ddriven%20architecture%20uses,on%20an%20e%2Dcommerce%20website.
