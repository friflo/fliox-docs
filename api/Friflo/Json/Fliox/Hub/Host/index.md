﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# Friflo.Json.Fliox.Hub.Host Namespace

**Namespace:** [Friflo.Json.Fliox.Hub](../index.md)  

## Namespaces

- [Friflo.Json.Fliox.Hub.Host.Auth](Auth/index.md)
- [Friflo.Json.Fliox.Hub.Host.Event](Event/index.md)
- [Friflo.Json.Fliox.Hub.Host.Internal](Internal/index.md)
- [Friflo.Json.Fliox.Hub.Host.Utils](Utils/index.md)

## Classes

| Name                                                                    | Description                                                                                                                                                                                                                                                |
| ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [CustomContainerName](CustomContainerName/index.md)                     |                                                                                                                                                                                                                                                            |
| [DatabaseSchema](DatabaseSchema/index.md)                               | A [DatabaseSchema](DatabaseSchema/index.md) can be assigned to a [Schema](EntityDatabase/properties/Schema.md) to enable validation of entities represented as JSON used in write operations \- create, upsert and patch.                                  |
| [DatabaseService](DatabaseService/index.md)                             | A [DatabaseService](DatabaseService/index.md) is attached to every [EntityDatabase](EntityDatabase/index.md) to handle all[tasks](../Protocol/SyncRequest/fields/tasks.md) of a [SyncRequest](../Protocol/SyncRequest/index.md).                           |
| [DatabaseServiceQueue](DatabaseServiceQueue/index.md)                   |                                                                                                                                                                                                                                                            |
| [EntityContainer](EntityContainer/index.md)                             | An [EntityContainer](EntityContainer/index.md) is the abstraction of a collection \/ table used to store entities \/ records  as key value pairs.                                                                                                          |
| [EntityDatabase](EntityDatabase/index.md)                               | [EntityDatabase](EntityDatabase/index.md) is the abstraction for specific database adapter \/ implementation e.g. a[MemoryDatabase](MemoryDatabase/index.md) or [FileDatabase](FileDatabase/index.md).                                                     |
| [EntityFilterContext](EntityFilterContext/index.md)                     |                                                                                                                                                                                                                                                            |
| [FileContainer](FileContainer/index.md)                                 |                                                                                                                                                                                                                                                            |
| [FileDatabase](FileDatabase/index.md)                                   | A [FileDatabase](FileDatabase/index.md) is used to store the entities \/ records of its containers as files in the .                                                                                                                                       |
| [FlioxHub](FlioxHub/index.md)                                           | A [FlioxHub](FlioxHub/index.md) act as a Proxy between a [FlioxClient](../Client/FlioxClient/index.md) or a web browser and an [EntityDatabase](EntityDatabase/index.md).                                                                                  |
| [HostCommandHandler\<TParam, TResult\>](HostCommandHandler-2/index.md)  |                                                                                                                                                                                                                                                            |
| [HostMessageHandler\<TParam\>](HostMessageHandler-1/index.md)           |                                                                                                                                                                                                                                                            |
| [HostMessageHandlerAsync\<TParam\>](HostMessageHandlerAsync-1/index.md) |                                                                                                                                                                                                                                                            |
| [HubInfo](HubInfo/index.md)                                             | Contains general information about a Hub describing the development environment. Clients can request this information with the command                                                                                                                     |
| [MemoryContainer](MemoryContainer/index.md)                             |                                                                                                                                                                                                                                                            |
| [MemoryDatabase](MemoryDatabase/index.md)                               | A [MemoryDatabase](MemoryDatabase/index.md) is a non\-persistent database used to store records in memory.                                                                                                                                                 |
| [MessageContext](MessageContext/index.md)                               | [MessageContext](MessageContext/index.md) expose all data relevant for command execution as properties or methods.                                                                                                                                         |
| [MessageUtils](MessageUtils/index.md)                                   |  all `Create` methods return a JsonValue which are only valid until the             passed ObjectReader it reused                                                                                                                                          |
| [SharedEnv](SharedEnv/index.md)                                         | [SharedEnv](SharedEnv/index.md) provide a set of shared resources available via [sharedEnv](FlioxHub/fields/sharedEnv.md).                                                                                                                                 |
| [SyncContext](SyncContext/index.md)                                     | One [SyncContext](SyncContext/index.md) is created per [ExecuteRequestAsync(SyncRequest, SyncContext)](FlioxHub/methods/ExecuteRequestAsync.md) call to enable multi threaded \/ concurrent handling of a [SyncRequest](../Protocol/SyncRequest/index.md). |
| [SyncPools](SyncPools/index.md)                                         |                                                                                                                                                                                                                                                            |

## Structs

| Name                                              | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [AsyncServiceJobs](AsyncServiceJobs/index.md)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [ExecuteSyncResult](ExecuteSyncResult/index.md)   | Contains the result of a [ExecuteRequestAsync(SyncRequest, SyncContext)](FlioxHub/methods/ExecuteRequestAsync.md) call. After execution either [success](ExecuteSyncResult/fields/success.md) or [error](ExecuteSyncResult/fields/error.md) is set. Never both.                                                                                                                                                                                                                                                                         |
| [Param\<TParam\>](Param-1/index.md)               |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [RemoteEventMessage](RemoteEventMessage/index.md) |  Reflect the shape of a [EventMessage](../Protocol/EventMessage/index.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [RemoteSyncEvent](RemoteSyncEvent/index.md)       |  Reflect the shape of a [SyncEvent](../Protocol/SyncEvent/index.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [SyncBuffers](SyncBuffers/index.md)               | [SyncBuffers](SyncBuffers/index.md) can be used to minimize heap allocations by passing to [SyncContext](SyncContext/index.md) constructor.  The the caller of [ExecuteRequestAsync(SyncRequest, SyncContext)](FlioxHub/methods/ExecuteRequestAsync.md) ensure that only one call to[ExecuteRequestAsync(SyncRequest, SyncContext)](FlioxHub/methods/ExecuteRequestAsync.md) is running at a time.            This requirement is fulfilled if request execution is stream based like [WebSocketHost](../Remote/WebSocketHost/index.md) |

## Interfaces

| Name                    | Description |
| ----------------------- | ----------- |
| [IHost](IHost/index.md) |             |

## Enums

| Name                                              | Description                                                               |
| ------------------------------------------------- | ------------------------------------------------------------------------- |
| [ExecutionType](ExecutionType/index.md)           |  Defines how to execute a [SyncRequest](../Protocol/SyncRequest/index.md) |
| [FilterEntityResult](FilterEntityResult/index.md) |                                                                           |
| [MemoryType](MemoryType/index.md)                 |                                                                           |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
