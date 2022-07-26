﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# StaticFileHandler Class

**Namespace:** [Friflo.Json.Fliox.Hub.Remote](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

A StaticFileHandler is used to serve static files by a [HttpHost](../HttpHost/index.md).

```csharp
public sealed class StaticFileHandler : IRequestHandler
```

**Inheritance:** object → StaticFileHandler

**Implements:** [IRequestHandler](../IRequestHandler/index.md)

## Remarks

Therefore add an instance of StaticFileHandler with [AddHandler(IRequestHandler)](../HttpHost/methods/AddHandler.md) to the Hub.The  assigned to the response `Content-Type` header is derived from the file name extension.Add additional mappings for  to  with [AddFileExtension(string, string)](methods/AddFileExtension.md).

## Constructors

| Name                                                                                      | Description |
| ----------------------------------------------------------------------------------------- | ----------- |
| [StaticFileHandler(Stream, string)](constructors/index.md#staticfilehandlerstream-string) |             |
| [StaticFileHandler(string)](constructors/index.md#staticfilehandlerstring)                |             |
| [StaticFileHandler(string, string)](constructors/index.md#staticfilehandlerstring-string) |             |

## Properties

| Name                                       | Description |
| ------------------------------------------ | ----------- |
| [CacheControl](properties/CacheControl.md) |             |
| [Routes](properties/Routes.md)             |             |

## Methods

| Name                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [AddFileExtension(string, string)](methods/AddFileExtension.md) |             |
| [HandleRequest(RequestContext)](methods/HandleRequest.md)       |             |
| [IsMatch(RequestContext)](methods/IsMatch.md)                   |             |
| [ToString()](methods/ToString.md)                               |             |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
