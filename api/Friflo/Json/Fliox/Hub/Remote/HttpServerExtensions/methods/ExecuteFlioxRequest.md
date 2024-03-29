﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# HttpServerExtensions.ExecuteFlioxRequest Method

**Declaring Type:** [HttpServerExtensions](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Remote](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Execute the request return a RequestContext containing the execution result. To return a HTTP response [WriteFlioxResponse(HttpListenerContext, RequestContext)](WriteFlioxResponse.md) need to be called. 

```csharp
[AsyncStateMachine(Friflo.Json.Fliox.Hub.Remote.HttpServerExtensions/<ExecuteFlioxRequest>d__0)]
[DebuggerStepThrough]
public static Task<RequestContext> ExecuteFlioxRequest(this HttpListenerContext context, HttpHost httpHost);
```

## Parameters

`context`  HttpListenerContext

`httpHost`  [HttpHost](../../HttpHost/index.md)

## Returns

Task\<[RequestContext](../../RequestContext/index.md)\>

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
