# Getting started

To get a project up and running:

    dotnet new sln -o sln2.
    dotnet new classlib -lang F# -o src/Library
    dotnet add src/Library/Library.fsproj package FSharp.Data
    dotnet sln add src/Library/Library.fsproj.
    dotnet build
    dotnet new console -lang F# -o src/App
    dotnet sln add src/App/App.fsproj
    dotnet add src/App/App.fsproj reference src/Library/Library.fsproj
    dotnet restore
    dotnet build
    dotnet run
