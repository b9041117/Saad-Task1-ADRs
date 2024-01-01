# Architectural Style

## Context and Problem Statement

## Status
Accepted

## Context
The AFS system contains lots of functionality from functional and non functional requirements that are not always related to one another. In addition security, scalability and performance are major concerns as laid out in the NFRs for the system and so the choosen architecture must be able to meet the standards set in the NFRs

## Considered Options

* Microservices
* Layered Architecture
* Data centered architecture

## Decision Outcome

Chosen option: "Microservices", because the benefits best fit with AFS systems functional and non functional requirements

## Pros and Cons of the Options

### Microservices

An architectural style that arranges the application as a collection of loosely coupled services that communicate with each other via lightweight protocols

### Layered Architecture

An architectural style where modules or components with similar functions are grouped together in horizontal layers

### Data centered architecture

A architectural style where the data is designed first and then the application is designed to create and use it

* Good, because Effiecent way to process a large amount of data
* Good, because Data is more secure
* Good, because Components can be independent
* Bad, because Single point of failure
* Bad, because Components are highly dependent on the data strucutre of the data store
* Bad, because Changing the Data structure in the data store will lead all components to fail.
