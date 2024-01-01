# Second Design Pattern

## Context and Problem Statement

## Status
Accepted

## Context
After choosing the event driven design pattern, the problem of how each microservice will communicate with other parts of the system remains. Therefore I need to pick another design pattern that can help solve this problem.

## Considered Options

* API Gateway
* Microgateways

## Decision Outcome

Chosen option: "Microgateways", because allows for microservices to communicate effectively

## Pros and Cons of the Options

### API Gateway

Provides centralised handling of APIs that is located between clients view and the services

### Microgateways

A Microgateway is a small API that serves as the single communication point for each microservice to communicate between different microservices without exposing the services to the application

## Links

* https://www.mountaingoatsoftware.com/agile/user-stories#:~:text=User%20stories%20are%20part%20of,functionality%20the%20user%20story%20represents.
