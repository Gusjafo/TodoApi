# Web Api

[referencia](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-6.0&tabs=visual-studio-code)

- App que muestra el uso de los controladores con una API web del lado front, usando ASP.NET Core.

## model class

A model is a set of classes that represent the data that the app manages. The model for this app is a single `TodoItem` class.

The `Id` property functions as the unique key in a relational database.

Model classes can go anywhere in the project, but the _Models_ folder is used by convention.

## database context

The _database context_ is the main class that coordinates Entity Framework functionality for a data model. This class is created by deriving from the Microsoft.EntityFrameworkCore.DbContext class.

## register the database context

In ASP.NET Core, services such as the DB context must be registered with the [dependency injection (DI)](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-6.0) container. The container provides the service to controllers.

