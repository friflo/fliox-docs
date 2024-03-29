﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# FlioxHub Class

**Namespace:** [Friflo.Json.Fliox.Hub.Host](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

A FlioxHub act as a Proxy between a [FlioxClient](../../Client/FlioxClient/index.md) or a web browser and an [EntityDatabase](../EntityDatabase/index.md).

```csharp
[CLSCompliant(true)]
public class FlioxHub : IDisposable, ILogSource
```

**Inheritance:** object → FlioxHub

**Attributes:** CLSCompliantAttribute

**Implements:** IDisposable,ILogSource

## Remarks

The FlioxHub features and utilization is available atWhen creating a FlioxHub a  is assigned to the instance and all tasks requested by a client are applied to this [database](fields/database.md). A FlioxHub can be configured to support:

A FlioxHub instance handle  client requests by its [ExecuteRequestAsync(SyncRequest, SyncContext)](methods/ExecuteRequestAsync.md) method. A request is represented by a [SyncRequest](../../Protocol/SyncRequest/index.md) and its [tasks](../../Protocol/SyncRequest/fields/tasks.md) are executed on the given [database](../../Protocol/SyncRequest/fields/database.md). If database \=\= null the default [database](fields/database.md) of FlioxHub is used.The [tasks](../../Protocol/SyncRequest/fields/tasks.md) contains all database operations like create, read, upsert, delete and all messages \/ commands send by a client. The FlioxHub execute these tasks by the service of the specified [database](fields/database.md).Instances of FlioxHub are  enabling multiple clients e.g. [FlioxClient](../../Client/FlioxClient/index.md)operating on the same FlioxHub instance. To maintain thread safety FlioxHub implementations must not have any mutable state.

## Constructors

| Name                                                         | Description                                             |
| ------------------------------------------------------------ | ------------------------------------------------------- |
| [FlioxHub(EntityDatabase, SharedEnv)](constructors/index.md) | Construct a FlioxHub with the given default `database`. |

## Fields

| Name                             | Description                                                          |
| -------------------------------- | -------------------------------------------------------------------- |
| [database](fields/database.md)   |  The default [database](fields/database.md) assigned to the FlioxHub |
| [sharedEnv](fields/sharedEnv.md) |                                                                      |

## Properties

| Name                                               | Description                                                                                                                                                                                                                                                                                                                                  |
| -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Authenticator](properties/Authenticator.md)       | An [Authenticator](../Auth/Authenticator/index.md) performs authentication and authorization for all[tasks](../../Protocol/SyncRequest/fields/tasks.md) in a [SyncRequest](../../Protocol/SyncRequest/index.md) sent by a client. All successful authorized [tasks](../../Protocol/SyncRequest/fields/tasks.md) are executed by the service. |
| [ClientController](properties/ClientController.md) | [ClientController](properties/ClientController.md) is used to create \/ add unique client ids to enable sending events to             specific user clients.             It also enables monitoring execution statistics of [ExecuteRequestAsync(SyncRequest, SyncContext)](methods/ExecuteRequestAsync.md)                                  |
| [EventDispatcher](properties/EventDispatcher.md)   | An optional [EventDispatcher](../Event/EventDispatcher/index.md) used to enable Pub\-Sub. If assigned the database send push events to clients for database changes and messages these clients have subscribed.                                                                                                                              |
| [FlioxVersion](properties/FlioxVersion.md)         |                                                                                                                                                                                                                                                                                                                                              |
| [HostName](properties/HostName.md)                 | On server side the name can be used to identify a specific host if used within a cluster of servers.On client side any name can be assigned to simplify differentiation if using multiple FlioxHub instances.                                                                                                                                |
| [HostVersion](properties/HostVersion.md)           | host [HostVersion](properties/HostVersion.md) \- available via command                                                                                                                                                                                                                                                                       |
| [Info](properties/Info.md)                         | General descriptive Hub information \- available via command                                                                                                                                                                                                                                                                                 |
| [Logger](properties/Logger.md)                     |                                                                                                                                                                                                                                                                                                                                              |

## Methods

| Name                                                                            | Description                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [AddExtensionDB(EntityDatabase)](methods/AddExtensionDB.md)                     | Add an `extensionDB` to the Hub. The extension database is identified by its[nameShort](../EntityDatabase/fields/nameShort.md)                                                                                                                                                                                                                                                                                                                 |
| [Dispose()](methods/Dispose.md)                                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [ExecuteRequest(SyncRequest, SyncContext)](methods/ExecuteRequest.md)           | Execute all [tasks](../../Protocol/SyncRequest/fields/tasks.md) of a [SyncRequest](../../Protocol/SyncRequest/index.md) send by client.                                                                                                                                                                                                                                                                                                        |
| [ExecuteRequestAsync(SyncRequest, SyncContext)](methods/ExecuteRequestAsync.md) | Execute all [tasks](../../Protocol/SyncRequest/fields/tasks.md) of a [SyncRequest](../../Protocol/SyncRequest/index.md) send by client.Method is thread\-safe as multiple [FlioxClient](../../Client/FlioxClient/index.md) instances are allowed to use a single FlioxHub instance.                                                                                                                                                            |
| [GetFeature\<TFeature\>()](methods/GetFeature.md)                               |                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [InitSyncRequest(SyncRequest)](methods/InitSyncRequest.md)                      | Before execution of a [SyncRequest](../../Protocol/SyncRequest/index.md) with [ExecuteRequestAsync(SyncRequest, SyncContext)](methods/ExecuteRequestAsync.md) or [ExecuteRequest(SyncRequest, SyncContext)](methods/ExecuteRequest.md)the [SyncRequest](../../Protocol/SyncRequest/index.md) must be initialized. If the request can be executed synchronously the method returns SyncDoing so avoids creation of a redundant Task instance.   |
| [QueueRequestAsync(SyncRequest, SyncContext)](methods/QueueRequestAsync.md)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [SetFeature\<TFeature\>(TFeature)](methods/SetFeature.md)                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [ToString()](methods/ToString.md)                                               |                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [TryGetDatabase(string, EntityDatabase)](methods/TryGetDatabase.md)             |                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [TryGetFeature\<TFeature\>()](methods/TryGetFeature.md)                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
