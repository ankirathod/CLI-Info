## Nuget
``dotnet nuget list source`` list the sources
``dotnet nuget add source <source> -n <source name>`` add a new package source
``dotnet nuget disable source <source name>`` disable nuget source
``dotnet nuget enable source <source name>`` enable nuget source
``dotnet nuget remove source <source name>`` remove package source
``dotnet nuget update source <source name>`` update package source

``dotnet nuget delete [<package name> <package version>]`` delete specific package from project

Ref: https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-nuget-delete
