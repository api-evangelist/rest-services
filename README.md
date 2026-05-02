# REST Services

Representational State Transfer (REST) is an architectural style for designing networked applications using stateless communication and standard HTTP methods (GET, POST, PUT, DELETE, PATCH) to interact with resources identified by URLs. REST services underpin modern web APIs and support the full software development lifecycle from design through deployment and maintenance. This index covers REST service implementations, frameworks, best practices, patterns, tooling, and educational resources that guide how REST services are built, managed, and consumed.

**Website:** [restfulapi.net](https://restfulapi.net)  
**Reference:** [Roy Fielding Dissertation](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm)

## Tags

`Architecture` `HTTP` `Web Services` `REST` `Service Design`

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-05-02

## Artifacts

| Type | Name | Link |
|---|---|---|
| Vocabulary | REST Services Vocabulary | [vocabulary/rest-services-vocabulary.yml](vocabulary/rest-services-vocabulary.yml) |
| JSON-LD Context | REST Services Context | [json-ld/rest-services-context.jsonld](json-ld/rest-services-context.jsonld) |

## REST Service Patterns

REST services are organized around resources and follow several key design patterns:

- **Collection Resources** (`/users`) — Lists of entities with GET (list) and POST (create)
- **Singleton Resources** (`/users/{id}`) — Individual entities with GET, PUT, PATCH, DELETE
- **Sub-Resources** (`/users/{id}/orders`) — Nested resources expressing relationships
- **CRUD Mapping** — POST→Create, GET→Read, PUT/PATCH→Update, DELETE→Delete

## Service Architecture Concerns

- **API Gateway** — Single entry point providing routing, authentication, and rate limiting
- **Service Mesh** — Infrastructure layer for service-to-service communication
- **Microservices** — Collection of small, independently deployable REST services
- **Circuit Breaker** — Resilience pattern for handling downstream service failures
- **Caching** — Cache-Control, ETag, and Last-Modified headers for performance

## Maintainers

**Kin Lane** — kin@apievangelist.com
