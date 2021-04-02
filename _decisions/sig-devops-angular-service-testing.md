---
type: decision
acronym: devops-angular-service-testing
title: >
    Angular Service Testing
decision_type: should
belongs_to: devops
status: _5_presented
todos: 
responsible: HBU
deadline: 2021-04-16
implemented: partially
history:
    v1:
        date: 2021-04-2
        comment: created initially
---

## Why is there need for such a decision?

All code should be tested. Services in angular are no exception. How to test the services is also important.

## Additional sources for better understanding the background

- [Unit Testing Mock Services](https://codecraft.tv/courses/angular/unit-testing/mocks-and-spies/)
- [Testing in Angular](https://angular.io/guide/testing)
- [Testing Serices in Angular](https://angular.io/guide/testing-services)

## Viable Options

- Using spies to return dummy data
- Using mocked versions of the services

## Alternatives not seriously considered

- Manually setting the dependencies in the Testbed

## How has this decision been evaluated?

First, the method with spies was implemented. But it became quickly apparent, that it is not comfortable to manually set spies on
every single method of the rest service. This had to be done in **ALL** services/components that use the rest serice. In order to make in easy
to use a mocked version of the service instead, the second option was chosen. A rest service should have a mocked version that returns data
and can be easily injection into all services/components that use it.

## Resolution Details

[Wiki Article](https://github.com/EVATool/evatool-frontend/wiki/AngularServiceTesting)

The following table shows advatanges and disavantages both options.

|  | Pro | Contra|
|-|:-:|:-:|
| Spies | Can locally override behavior | Overriding must be done locally (outsourcing it would be very tedious)|
| Mocked Service | Mocked version can be used anywhere easily Can still utilize spies | All methods need to be overridden and maintained |

Using spies would lead to code duplication and would make it much more tedious to maintain the tests. Using a mocked version we only have
to maintain a single mocked service class per service. It is a simple class returning dummy data and is centralized. The biggest advantage though
is that the mocked service is super easy to use in tests instead of the real service. 

## Reasons for the resolution

The main reasons are the code maintanability and ease of use when injecting the mocked service into other service/components that require it.
