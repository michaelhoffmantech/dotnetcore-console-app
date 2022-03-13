# dotnetcore-console-app
Sandbox console app for testing out .NET core 6

## Project Creation

I used the Rider IDE solution generator for a .NET core console application. This created several directories:

* Main directory = C:\dev\dotnetcore-console-app\DotnetcoreConsoleApp
* Solution file = C:\dev\dotnetcore-console-app\DotnetcoreConsoleApp\DotnetcoreConsoleApp.sln
  ```
  Microsoft Visual Studio Solution File, Format Version 12.00
  Project("{FAE04EC0-301F-11D3-BF4B-00C04F79EFBC}") = "DotnetcoreConsoleApp", "DotnetcoreConsoleApp\DotnetcoreConsoleApp.csproj", "{4FC31986-116D-4286-B5D3-892C5C9DB11F}"
  EndProject
  Global
  	GlobalSection(SolutionConfigurationPlatforms) = preSolution
  		Debug|Any CPU = Debug|Any CPU
  		Release|Any CPU = Release|Any CPU
  	EndGlobalSection
  	GlobalSection(ProjectConfigurationPlatforms) = postSolution
  		{4FC31986-116D-4286-B5D3-892C5C9DB11F}.Debug|Any CPU.ActiveCfg = Debug|Any CPU
  		{4FC31986-116D-4286-B5D3-892C5C9DB11F}.Debug|Any CPU.Build.0 = Debug|Any CPU
  		{4FC31986-116D-4286-B5D3-892C5C9DB11F}.Release|Any CPU.ActiveCfg = Release|Any CPU
  		{4FC31986-116D-4286-B5D3-892C5C9DB11F}.Release|Any CPU.Build.0 = Release|Any CPU
  	EndGlobalSection
  EndGlobal
  ```
* C:\dev\dotnetcore-console-app\DotnetcoreConsoleApp\DotnetcoreConsoleApp\Program.cs = Main program
  ```
  // See https://aka.ms/new-console-template for more information

  Console.WriteLine("Hello, World!");
  ```
* C:\dev\dotnetcore-console-app\DotnetcoreConsoleApp\DotnetcoreConsoleApp\DotnetcoreConsoleApp.csproj = Project description
  ```
  <Project Sdk="Microsoft.NET.Sdk">

      <PropertyGroup>
          <OutputType>Exe</OutputType>
          <TargetFramework>net6.0</TargetFramework>
          <ImplicitUsings>enable</ImplicitUsings>
          <Nullable>enable</Nullable>
          <DockerDefaultTargetOS>Linux</DockerDefaultTargetOS>
      </PropertyGroup>

  </Project>
  ```
