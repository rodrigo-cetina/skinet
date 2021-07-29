# Installation

## Create a solution

`dotnet new sln`

## Create a web api

`dotnet new webapi -o API`

`dotnet sln add API`

`code .`

## Run the web api project

`cd API`

`dotnet dev-certs https --trust`

`dotnet build`

`dotnet run`

`dotnet watch run`

## Create a class library

`dotnet new classlib -o Core`

`dotnet sln add Core`

## Add Reference

`cd API`

`dotnet add reference ../Infrastructure`

`cd ..`

`dotnet restore`

## Installation Entity Framework Net Core

`dotnet tool install --global dotnet-ef`

`dotnet add package Microsoft.EntityFrameworkCore.Sqlite`

`dotnet add package Microsoft.EntityFrameworkCore.Design`

`dotnet restore`

## Commands Entity Framework Net Core

`dotnet ef migrations add [migration_name] -o Data/Migrations`

`dotnet ef database update`

`dotnet ef database drop -p Infrastructure -s API`

`dotnet ef migrations remove -p Infrastructure -s API`

`dotnet ef migrations add InitialCreate -p Infrastructure -s API -o Data/Migrations`

## NuGet Packages

`AutoMapper.Extensions.Microsoft.DependencyInjection`

## Git

`git init`

create file .gitignore and add:

```.gitignore
obj
bin
appsettings.json
*.db
```

`git add .`

`git commit -m "Initial Commit"`

`git remote add origin https://github.com/rodrigo-cetina/skinet.git`

`git push -u origin master`

## Extensions VSCode

- C#
- C# Extensions
- NuGet Package Manager
- NuGet Gallery
