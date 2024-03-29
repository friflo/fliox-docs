﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# ProtocolRequest.reqId Field

**Declaring Type:** [ProtocolRequest](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Protocol](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Used only for [SocketClientHub](../../../Remote/SocketClientHub/index.md) to enable:

1. Out of order response handling for their corresponding requests.

2. Multiplexing of requests and their responses for multiple clients e.g. [FlioxClient](../../../Client/FlioxClient/index.md)   using the same connection.    This is not a common scenario but it enables using a single [WebSocketClientHub](../../../Remote/WebSocketClientHub/index.md)   used by multiple clients.            The host itself only echos the reqId to [reqId](../../ProtocolResponse/fields/reqId.md) and             does  utilize it internally.

```csharp
[Serialize("req")]
public int? reqId;
```

## Field Value

Nullable\<int\>

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
