﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# HttpServer Class

**Namespace:** [Friflo.Json.Fliox.Hub.Remote](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

HttpServer is a utility class to enable running a simple HTTP Server by using a HttpListener

```csharp
public sealed class HttpServer : IServer, IDisposable, ILogSource
```

**Inheritance:** object → HttpServer

**Implements:** [IServer](../IServer/index.md),IDisposable,ILogSource

## Remarks

Via its utility methods is manages the lifecycle of a HttpListener. Lifecycle methods:

## Constructors

| Name                                                                                        | Description |
| ------------------------------------------------------------------------------------------- | ----------- |
| [HttpServer(HttpListener, HttpHost)](constructors/index.md#httpserverhttplistener-httphost) |             |
| [HttpServer(string, HttpHost)](constructors/index.md#httpserverstring-httphost)             |             |

## Fields

| Name                                                   | Description |
| ------------------------------------------------------ | ----------- |
| [customRequestHandler](fields/customRequestHandler.md) |             |

## Properties

| Name                                 | Description |
| ------------------------------------ | ----------- |
| [IsRunning](properties/IsRunning.md) |             |
| [Logger](properties/Logger.md)       |             |

## Methods

| Name                                                             | Description |
| ---------------------------------------------------------------- | ----------- |
| [Dispose()](methods/Dispose.md)                                  |             |
| [ExecuteRequest(HttpListenerContext)](methods/ExecuteRequest.md) |             |
| [Run()](methods/Run.md)                                          |             |
| [RunAsync()](methods/RunAsync.md)                                |             |
| [RunHost(string, HttpHost)](methods/RunHost.md)                  |             |
| [Start()](methods/Start.md)                                      |             |
| [Stop()](methods/Stop.md)                                        |             |
| [ToString()](methods/ToString.md)                                |             |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*