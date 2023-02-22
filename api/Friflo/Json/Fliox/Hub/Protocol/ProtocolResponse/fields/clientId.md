﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# ProtocolResponse.clientId Field

**Declaring Type:** [ProtocolResponse](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Protocol](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Set to [clientId](../../ProtocolRequest/fields/clientId.md) of a [SyncRequest](../../SyncRequest/index.md) in case the given[clientId](../../ProtocolRequest/fields/clientId.md) was valid. Otherwise it is set to null.

```csharp
[Serialize("clt")]
public ShortString clientId;
```

## Field Value

ShortString

## Remarks

Calling [EnsureValidClientId(ClientController, SyncContext, string)](../../../Host/Auth/Authenticator/methods/EnsureValidClientId.md) when clientId \=\= null a new unique client id will be assigned. For tasks which require a clientId a client need to set [clientId](../../ProtocolRequest/fields/clientId.md)to clientId. This enables tasks like [SubscribeMessage](../../Tasks/SubscribeMessage/index.md) or [SubscribeChanges](../../Tasks/SubscribeChanges/index.md) identifying the[SyncEvent](../../SyncEvent/index.md) target. 

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*