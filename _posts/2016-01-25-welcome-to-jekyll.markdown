---
layout: post
title:  "Microservices and Patterns"
date:   2016-01-25 15:39:33 +0000
categories: jekyll update
---

Microservices are Loosely coupled service oriented architecture with [Bounded Contexts][Bounded-Context].


If we are knowing too much about the other services to build a new Microservice then we are not having [Bounded Context][Bounded-Context].
If every service has to be updated at the same time it's not loosley coupled

In [Service oriented architecture] [SOA], we have dummy services and smart [enterprise service bus] [ESB], most of the validation, routing and transformation is handled in [enterprise service bus] [ESB], as the number of services grow and changes to one service will effect the others and Continous deployment will not be feasible.

 In MicroServices services are smart they do validation,transformation and handle business logic, and they use only Message Brokers like ActiveMQ or RabbitMQ but not [enterprise service buses] [ESB], with this they are loosley coupled from other services and easy implement  Continous deployment.

Principles of MicroServices

- Domain -- Bounded Contexts can help you find stable, reusable boundaries
- Culture Of Automation
	- Continous Delivery, Integration
	- Docker
	- Vagrant

- Abstraction (Hide Implementation Details)
- Decentralize All The Things
- Deploy Independently
- Consumer First
- Isolate Failure -[Circuit Breakers]
- Highly Observable



[Bounded-Context]: http://martinfowler.com/bliki/BoundedContext.html
[ESB]:https://en.wikipedia.org/wiki/Enterprise_service_bus
[SOA]:https://en.wikipedia.org/wiki/Service-oriented_architecture
