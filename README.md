# Bedrock Framework

[![feedz.io](https://img.shields.io/badge/endpoint.svg?url=https%3A%2F%2Ff.feedz.io%2Fdavidfowl%2Fbedrockframework%2Fshield%2FBedrock.Framework%2Flatest&label=Bedrock.Framework)](https://f.feedz.io/davidfowl/bedrockframework/packages/Bedrock.Framework/latest/download)

[![Gitter](https://badges.gitter.im/BedrockFramework/BedrockFramework.svg)](https://gitter.im/BedrockFramework/BedrockFramework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

[Project Bedrock](https://github.com/aspnet/AspNetCore/issues/4772) is a set of .NET 5 APIs for doing transport agnostic networking. In .NET Core 5.0 we've introduced some new abstractions
as part of [System.Net.Connections](https://github.com/dotnet/runtime/issues/1793) for client-server communication. 

See the presentation [here](https://speakerdeck.com/davidfowl/project-bedrock)

This project is split into 2 packages:
- **Bedrock.Framework** - The core framework, server and client builder APIs, built in middleware and transports (sockets and memory).
- **Bedrock.Framework.Experimental** - A set of protocol and transport implementations that may eventually make their way into core. Some of them are incomplete at this time.

## Using CI builds

To use CI builds add the following nuget feed:

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
    <packageSources>
        <clear />
        <add key="bedrockframework" value="https://f.feedz.io/davidfowl/bedrockframework/nuget/index.json" />
        <add key="NuGet.org" value="https://api.nuget.org/v3/index.json" />
    </packageSources>
</configuration>
```
