[English](README.md) | [Русский](README.ru.md)

# Golang Project Starter Template

This repository provides a structured template for creating Golang projects, adhering to the "clean architecture" paradigm.

## Project Structure

- **api/v1**: Contains API specifications for the first version of your service, including Swagger files.

- **cmd/appname**: The entry point of your application. Here is the main function to start your service.

- **config**: A place for configuration files and code that loads them.

- **db**: Contains everything related to the database: migration files and code for working with the database.

- **Docker**: Files for creating a Docker image of your application.

- **internal**: Code that is specific to this application and is not intended for external use.

  - **middleware**: Middleware handlers for your web server.
  - **models**: Data models and business logic.
  - **utils**: Helper functions and utilities.

- **pkg**: Code that can be reused in other projects (common libraries and utilities).

- **server**: Code for setting up and running your web server.

- **tests**: Tests for your application, divided into integration and unit tests.

## Getting Started

1. Clone this repository.
2. Update the configuration files in the `config` folder according to your requirements.
3. Add your database migrations to the `db/migrations` folder.
4. Implement your business logic in the `internal` folder.
5. Start your application from the `cmd/appname` folder.

## Running in Docker

1. Build your Docker image using `Docker/dockerfile`.
2. Use `Docker/docker-compose.yaml` to run your application in a container.

## Contribution

If you have suggestions or improvements for this template, feel free to create issues or pull requests.

---
