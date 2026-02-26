# taskmanager-dotnet

A RESTful API for managing tasks and projects, built with .NET 10 and Clean Architecture principles.

## Tech Stack

- .NET 10 / ASP.NET Core Web API
- Entity Framework Core
- PostgreSQL
- JWT Authentication
- xUnit

## Features

- [ ] CRUD operations for tasks
- [ ] Task categories and projects
- [ ] User authentication and authorization (JWT)
- [ ] Filtering, sorting, and pagination
- [ ] Swagger / OpenAPI documentation
- [ ] Global error handling
- [ ] Docker support

## Getting Started

### Prerequisites

- [.NET 10 SDK](https://dotnet.microsoft.com/download)
- PostgreSQL (or Docker)

### Installation

```bash
git clone https://github.com/OlivierGawronek/taskmanager-dotnet.git
cd taskmanager-dotnet
dotnet restore
dotnet run --project TaskManager.API
```

API will be available at `https://localhost:5001/swagger`

## Project Structure

```
TaskManager/
├── TaskManager.API/            # Controllers, middleware, configuration
├── TaskManager.Application/    # Services, DTOs, interfaces
├── TaskManager.Domain/         # Entities, enums, domain logic
├── TaskManager.Infrastructure/ # EF Core, repositories, migrations
└── TaskManager.Tests/          # Unit tests (xUnit)
```

## Architecture

This project follows **Clean Architecture** to maintain separation of concerns:

- **Domain** — core entities with no external dependencies
- **Application** — business logic, service interfaces, DTOs
- **Infrastructure** — database access, external services
- **API** — HTTP layer, controllers, middleware

## Status

🚧 Work in progress

## License

This project is licensed under the [MIT License](LICENSE).