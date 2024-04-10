<div align="center">
<a href="https://github.com/NicoFilips/csharp-designpatterns/">
  <img src="https://github.com/NicoFilips/csharp-designpatterns/assets/35654361/9989426c-1af2-4ddb-b499-3ad81a12552f" alt="Logo" width="200" height="200">
</a>
<blockquote>
  <p>Source: DALL-E 3</p>
</blockquote>

  <h3 align="center"> 🍫 SwissChocolateAPI 🇨🇭 </h3>

  <p align="center">
    This is a practical Example how a domain driven REST API with clean architecture looks like
  </p>

[![Use Dotnet Pipeline Template](https://github.com/NicoFilips/SwissChocolateAPI/actions/workflows/dotnet.yml/badge.svg)](https://github.com/NicoFilips/csharp-designpatterns/actions/workflows/dotnet.yml)

![C# Logo](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![](https://img.shields.io/badge/.NET-8-512BD4?style=for-the-badge&logo=.net&logoColor=white)
</div>


## About the Project
  <h3 align="center">Sali zeme</h3>
## Domain

The Domain Layer in software architecture, particularly within the context of Domain-Driven Design (DDD), is a critical layer that encapsulates the business logic and domain knowledge of the application. It is the heart of the system where the concepts, constraints, and logic that are specific to the problem domain are implemented. This layer is designed to be independent of the infrastructure or data access layers, ensuring that the business rules and policies are decoupled from external concerns.

Components of the Domain Layer
The Domain Layer contains several key DDD components, each serving a distinct purpose within the domain model:

Entities
Entities are objects that have a distinct identity that runs through time and different states. An entity is defined not by its attributes but by its identity, meaning two entities can have the same attributes but are considered different because they have different identities. For example, two people with the same name are still distinct individuals.

Value Objects
Value Objects are objects that do not have an identity and are defined solely by their attributes. They are immutable; once created, they cannot be altered. If any attribute of a Value Object changes, a new instance of the Value Object is created. Value Objects are used to describe aspects of the domain with no conceptual identity, like a color or a date range.

Aggregates
An Aggregate is a cluster of domain objects (entities and value objects) that can be treated as a single unit. An Aggregate has a root and a boundary. The root is a single, specific entity known as the Aggregate Root, through which all external access to the objects of the Aggregate is controlled. The boundary defines what is inside the Aggregate, and it's this boundary that helps maintain the consistency of changes to the Aggregate's internal state.

Aggregate Roots
Aggregate Roots are special entities that serve as the entry point to an Aggregate. They ensure the integrity of the Aggregate by controlling how its objects are accessed and modified. Aggregate Roots can enforce rules that must be applied across the Aggregate, ensuring that all changes leave the Aggregate in a valid state.

Domain Events
Domain Events are significant business events that trigger side effects within the domain. They represent something important that happened in the domain, and other parts of the domain can react to these events. For example, an order being placed might be a domain event that triggers the allocation of stock to the order.

Repositories
Repositories are used to abstract the way aggregates are persisted and retrieved from the storage mechanism. They provide a collection-like interface for accessing domain objects. Repositories handle querying the database and mapping the data to domain objects, ensuring that the domain model doesn't need to know about the details of data access.

Domain Services
Domain Services are stateless operations or behaviors that don't naturally fit within an entity or value object. They can perform calculations or combine domain objects in a way that implements domain rules and logic. Services are defined in the domain layer but can orchestrate actions across multiple Aggregates or domain objects.

The Domain Layer is pivotal in DDD as it focuses on the core business logic and rules, making it the most important part of any system built with DDD principles. It allows for the separation of concerns, ensuring that business logic is not tied to the application's UI, database, or any other infrastructure.

## Infrastructure

## Application

## API
