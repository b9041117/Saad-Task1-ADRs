# Testing Framework

## Context and Problem Statement

## Status
Accepted

## Context
During development of the application I would like to use Test Driven development, therefore I need to decide on which testing framework would be the most suited for the task.

## Considered Options

* Moq (Before version 4.20)
* XUnit

## Decision Outcome

Chosen option: "Moq", because as it provides additional functionality over XUnit

## Pros and Cons of the Options

### Moq

Moq is a mocking framework that is built for testing and can replicate the behaviour of any object, however in version 4.20 the author of the open source project introduced code that reads users emails and sends it to an external server.

* Good, because Works extremely well with C# .NET technologies
* Good, because Very effective for unit testing and test driven development
* Good, because I have extensive experience using Moq for unit test development
* Bad, because It means using a depreciated version and I would not be able to update Moq to later versions as this contains the email scraping code

### XUnit

It's a open source unit testing tool for .NET

* Good, because Extensibility, it is very easy to add custom traits and attributes onto XUnit
* Good, because Reductions in complex configurations
* Bad, because Lack of advance features including data driven testing
* Bad, because Steep learning curve for new users

## Links

* https://medium.com/checkmarx-security/popular-nuget-package-moq-silently-exfiltrates-user-data-to-cloud-service-d1888867406d
* https://northcoders.com/company/blog/the-benefits-of-test-driven-development-tdd
* https://www.headspin.io/blog/nunit-vs-xunit-vs-mstest
