# DotArch

A reusable ASP.NET Core Web API architecture template.

## Installation

```bash
dotnet new install DotArch
```

## Create a project

```bash
dotnet new dotarch -n MyApi
```

## Generated structure

```text
MyApi/
├── MyApi.sln
│
├── src/
│   ├── MyApi.Api/
│   ├── MyApi.Application/
│   ├── MyApi.Domain/
│   └── MyApi.Infrastructure/
│
└── tests/
    ├── MyApi.UnitTests/
    └── MyApi.IntegrationTests/
```

## Architecture

```text
MyApi.Api
    │
    ▼
MyApi.Application
    │
    ▼
MyApi.Domain

MyApi.Infrastructure
    │
    ├── Application
    └── Domain
```

### Projects

**Api**

HTTP endpoints, controllers, middleware, dependency injection and API configuration.

**Application**

Use cases, commands, queries, DTOs, validators and application interfaces.

**Domain**

Entities, value objects, enums and business rules.

**Infrastructure**

Database access, repositories, external services, caching, authentication implementations and other infrastructure concerns.

**Tests**

Unit and integration tests.

## Build

```bash
dotnet build
```

## Run

```bash
dotnet run --project src/MyApi.Api
```
