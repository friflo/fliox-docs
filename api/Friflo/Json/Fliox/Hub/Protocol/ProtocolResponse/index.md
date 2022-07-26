﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# ProtocolResponse Class

**Namespace:** [Friflo.Json.Fliox.Hub.Protocol](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Base type for response messages send from a host to a client in reply of [SyncRequest](../SyncRequest/index.md)

```csharp
[Discriminator("msg", "response type")]
[PolymorphType(Friflo.Json.Fliox.Hub.Protocol.SyncResponse, "resp")]
[PolymorphType(Friflo.Json.Fliox.Hub.Protocol.ErrorResponse, "error")]
public abstract class ProtocolResponse : ProtocolMessage
```

**Inheritance:** object → [ProtocolMessage](../ProtocolMessage/index.md) → ProtocolResponse

**Attributes:** DiscriminatorAttribute,PolymorphTypeAttribute,PolymorphTypeAttribute

## Remarks

A response is either a [SyncResponse](../SyncResponse/index.md) or a [ErrorResponse](../ErrorResponse/index.md) in case of a general error.

## Fields

| Name                           | Description                                                                                                                                                                                                     |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [clientId](fields/clientId.md) | Set to [clientId](../ProtocolRequest/fields/clientId.md) of a [SyncRequest](../SyncRequest/index.md) in case the given[clientId](../ProtocolRequest/fields/clientId.md) was valid. Otherwise it is set to null. |
| [reqId](fields/reqId.md)       | Set to the value of the corresponding [reqId](../ProtocolRequest/fields/reqId.md) of a [ProtocolRequest](../ProtocolRequest/index.md)                                                                           |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
