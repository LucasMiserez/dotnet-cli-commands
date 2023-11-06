# .NET CLI Commands

As a Linux user who doesn't have access to Visual Studio, I rely on [VSCodium](https://vscodium.com/) (or any other IDE of your choice) to create my .NET applications and webpages. This repository is a simple and straightforward guide designed to help you navigate the world of .NET development from the command line.

## Introduction

When using .NET on a Linux system, understanding the essential command-line tools is crucial. This guide will walk you through the must-know commands, providing clear explanations and practical examples to help you become proficient in .NET development. 

## Getting Started with .NET CLI

## Before You Begin

Before you dive into using the .NET CLI, there are a few preliminary steps to ensure a smooth development experience:

1. **Install .NET:** If you haven't already, make sure you have the .NET SDK installed on your system. You can download it from the official [.NET website](https://dotnet.microsoft.com/download/dotnet).

2. **Choose Your IDE:** Select your preferred Integrated Development Environment (IDE) for .NET development. Whether you're using [Visual Studio Code](https://code.visualstudio.com/), [VSCodium](https://vscodium.com/), or any other IDE, ensure it's set up and ready for .NET development.

   - *For Visual Studio Code/VSCodium Users:* Install the C# extension. This extension enhances your .NET development experience within the IDE.

With these steps completed, you'll be well-prepared to utilize the .NET CLI for your development projects.

## Exploring Useful .NET CLI Commands

In addition to the essential commands for development, the .NET CLI offers a set of useful commands to help you manage your development environment and gather information about your .NET setup. Here are a few commands that you may find handy:

1. **Check .NET Version:**
   To verify the installed .NET SDK versions on your system, run:
   ```sh
   dotnet --list-sdks
    ```
2. **Explore Available Templates:**
    Discover available project templates and their descriptions by using:
    ```sh
   dotnet new list
    ```
    This command lists all the project templates you can use to kickstart your .NET projects.

3. **List Installed Runtimes:**
    To see the installed .NET runtime versions, use:
    ```sh
   dotnet --list-runtimes
    ```

4. **Manage Global Tools:**
    If you have installed global .NET tools, list them with:
     ```sh
   dotnet tool list -g
    ```

5. **Find Information About a Tool:**
    For more details about a specific global tool, including its version and description, run:
     ```sh
   dotnet tool show -g <tool-name>
    ```

6. **Create gitgnore:**
    if you want to create a gitignore file for your git repository, you can use this command:
     ```sh
   dotnet new gitignore
    ```

7. **Get all dotnet commands:**
     ```sh
   dotnet -h
    ```

These commands allow you to explore your .NET environment, check versions, and manage global tools, enhancing your control and understanding of your .NET setup.

## Basic Commands For Your .NET Project

In this section, you'll discover important .NET CLI commands that help you create, organize, and simplify tasks for your .NET projects. These commands are essential for an efficient and productive project development experience.

1. **Create a solution:**
    ```sh
   dotnet new sln --name SolutionName
    ```

2. **Create a project:**
    ```sh
   dotnet new ProjectType -f netVersion(E.g. net6.0) --name "ProjectName"
    ```

3. **Add a project to a solution:**
    ```sh
   dotnet sln SolutionName.sln add ProjectFolder/ProjectName.csproj
    ```

4. **Add reference from one project to another project:**
    ```sh
   dotnet add Project1Folder/Project1Name.csproj reference Project2Folder/Project2Name.csproj
    ```
    This will establish a reference from Project1 to Project2.

5. **Add reference to a NuGet package:**
    ```sh
    cd ProjectFolder/
   dotnet add package PackageName
    ```
    NuGet packages and their name can be found on the [NuGet Gallery | Packages](https://www.nuget.org/packages).


