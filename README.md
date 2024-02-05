# DotNet Exercise 1: DotNet Dependencies
 
This program was created following Microsoft Learn's .NET tutorial under the '[Build .NET applications with C#](https://learn.microsoft.com/en-us/training/paths/build-dotnet-applications-csharp/)' training path. The exercise is meant to familiarize learners with creation of .NET projects in VS Code using the .NET cli, and also introduce learners with adding packages to a project. The section of the learning path this exercise is from is titled '[Create a new .NET project and work with dependencies](https://learn.microsoft.com/en-us/training/modules/dotnet-dependencies/3-exercise-dependency)'. 

## Notes

`dotnet --list-sdks`

This command prints a list of the .NET sdks the user has installed. <br>
[dotnet command](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet)

`dotnet new console -f net8.0`

This command creates a new .NET console application, as noted by the `console` argument following `dotnet new` command, and uses the framework option `-f <FRAMEWORK>` to specify which .NET sdk framework is used in the app. <br>
[dotnet new](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-new) <br>
[Target frameworks in SDK-style projects](https://learn.microsoft.com/en-us/dotnet/standard/frameworks)

`dotnet add package Humanizer --version 2.7.9`

This command adds a package to the project, as noted by `add package <PACKAGE_NAME>`, however it is also used to update an existing package according to the reference page. In this project, the package "Humanizer" is added, specifically version 2.7.9 using the `--version 2.7.9` option. <br>
[dotnet add package](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-add-package)

`dotnet run`

This command runs the project source code. There is more to learn about the command and its options in the reference. <br>
[dotnet run](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-run)

`dotnet list package`

This command lists installed dependencies within the project. <br>
[dotnet list package](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-list-package)

`dotnet list package --outdated`

This command lists the dependencies within the project that have a newer version available.

`dotnet add package Humanizer`

This command normally adds the Humanizer package to the project, but since the project already has it, it will instead seek to update the package to the latest release version found on NuGet, the .NET package repository.