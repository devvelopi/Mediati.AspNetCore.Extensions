# Mediati AspNetCore Extensions
Extensions for configuring Mediati command, query and event handlers automatically with dependency injection.

## Installation

```bash
dotnet add package Mediati.AspNetCore
```

## Usage

Usage is simple. In Startup:

```c#
using Microsoft.Extensions.DependencyInjection;
using Mediati.AspNetCore.Extensions;

namespace SomeNamespace
{
    public class Startup
    {
        public void ConfigureServices(IServiceCollection services)
        {
            services.AddMediati();
            services.AddMediatiHandlers();
        }
    }
}
```