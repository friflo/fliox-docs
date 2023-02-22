﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# ClientResult Class

**Namespace:** [Friflo.Json.Fliox.Hub.DB.Cluster](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

```csharp
public sealed class ClientResult
```

**Inheritance:** object → ClientResult

## Constructors

| Name                                    | Description |
| --------------------------------------- | ----------- |
| [ClientResult()](constructors/index.md) |             |

## Fields

| Name                                               | Description                                                                                                                                                                                                                                                                                                                                                                                                              |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [clientId](fields/clientId.md)                     | return the client id set in the [SyncRequest](../../../Protocol/SyncRequest/index.md). Can be null.            A new client id is created in case any task requires a client id and the [SyncRequest](../../../Protocol/SyncRequest/index.md) did not set a client id.            E.g. [ensureClientId](../ClientParam/fields/ensureClientId.md) \= true or [queueEvents](../ClientParam/fields/queueEvents.md) \= true  |
| [queueEvents](fields/queueEvents.md)               |  returns true if the host queue events for the client in case of disconnects                                                                                                                                                                                                                                                                                                                                             |
| [queuedEvents](fields/queuedEvents.md)             | return number of queued events not acknowledged by the client. Events are queued only if the client instruct the Hub to queue events by setting [queueEvents](../ClientParam/fields/queueEvents.md) \= true                                                                                                                                                                                                              |
| [subscriptionEvents](fields/subscriptionEvents.md) | number of sent or queued client events and its message and change subscriptions                                                                                                                                                                                                                                                                                                                                          |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*