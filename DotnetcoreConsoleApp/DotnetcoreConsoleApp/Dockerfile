FROM mcr.microsoft.com/dotnet/runtime:6.0 AS base
WORKDIR /app

FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build
WORKDIR /src
COPY ["DotnetcoreConsoleApp/DotnetcoreConsoleApp.csproj", "DotnetcoreConsoleApp/"]
RUN dotnet restore "DotnetcoreConsoleApp/DotnetcoreConsoleApp.csproj"
COPY . .
WORKDIR "/src/DotnetcoreConsoleApp"
RUN dotnet build "DotnetcoreConsoleApp.csproj" -c Release -o /app/build

FROM build AS publish
RUN dotnet publish "DotnetcoreConsoleApp.csproj" -c Release -o /app/publish

FROM base AS final
WORKDIR /app
COPY --from=publish /app/publish .
ENTRYPOINT ["dotnet", "DotnetcoreConsoleApp.dll"]
