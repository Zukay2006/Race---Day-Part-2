
# RaceDay API – Programming Assignment Part 2

## Project Overview

RaceDay API is a RESTful Web API developed using C# and ASP.NET Core. It manages race-day information, including participants, organisers, events, categories, routes, enrolments, and results.

The project uses Entity Framework Core with SQL Server for database operations and Swagger for exploring and testing API endpoints.

## Technologies Used

- C#
- ASP.NET Core Web API (.NET 10)
- Entity Framework Core
- SQL Server
- Swagger / OpenAPI
- xUnit testing
- GitHub Actions

## Main Features

- User registration and authentication
- Participant and Organiser roles
- Event and category management
- Race enrolments
- Race result management
- Database migrations
- Automated testing

## Project Structure

- `Part 2/` – API source code, controllers, models, DTOs, database context, and migrations.
- `RaceDay.API.Tests/` – Unit and integration tests.
- `.github/workflows/dotnet.yml` – GitHub Actions workflow for building the project and running tests.

## Prerequisites

Before running the project, install:

- .NET 10 SDK
- SQL Server
- Visual Studio 2022 or a compatible IDE
- A web browser for Swagger

## How to Run the Project

1. Clone or download this repository.
2. Open `Part 2/RaceDay.API.slnx` in a compatible IDE.
3. Update the `DefaultConnection` connection string in `Part 2/appsettings.json` to match your local SQL Server configuration.
4. Restore the NuGet packages.
5. Apply the Entity Framework Core migrations if required by your database setup.
6. Run the API project.
7. Open the Swagger URL shown in the application output to explore the available endpoints.

## Running the Tests

From the repository root, run:

```bash
dotnet restore "Part 2/RaceDay.API.slnx"
dotnet build "Part 2/RaceDay.API.slnx" --configuration Release
dotnet test "Part 2/RaceDay.API.slnx" --configuration Release
```

The GitHub Actions workflow automatically builds the project and runs the tests when changes are pushed to the `main` branch or a pull request targets `main`.


## Successful Build and Tests

The GitHub Actions workflow successfully builds the RaceDay API project and runs the automated tests.

![Successful GitHub Actions build](github-actions-success.png)


## Demonstration Video

[Watch the RaceDay API demonstration on YouTube](https://youtu.be/-y-IOMPq_Ms)

## Repository

[RaceDay API – Programming Assignment Part 2](https://github.com/Zukay2006/Race---Day-Part-2)
