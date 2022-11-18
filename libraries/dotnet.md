---
title: C# / .Net Library
category: Official Libraries
description: Cache every single thing your app could ever do ahead of time, so your code never even has to run at all.
---

We propose a C# package compatible with `.NET Standard`, to add it just type this in a terminal, you can also get it on [NuGet](https://www.nuget.org/packages/ClintSharp/1.0.0.5).

```bash
dotnet add package HypeProxyClient --version 1.0.0.5
```

## How to use it?

Pretty easy, create an instance of the `HypeProxyClient` class and authenticate yourself via a JWT token or email and password.

```clike
var client = HypeProxyClient.Connect("API_TOKEN");
bool healthy = client.HealthCheck();
```