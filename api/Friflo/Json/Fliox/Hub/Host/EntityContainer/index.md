﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EntityContainer Class

**Namespace:** [Friflo.Json.Fliox.Hub.Host](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

An EntityContainer is the abstraction of a collection \/ table used to store entities \/ records  as key value pairs.

```csharp
[CLSCompliant(true)]
public abstract class EntityContainer : IDisposable
```

**Inheritance:** object → EntityContainer

**Attributes:** CLSCompliantAttribute

**Implements:** IDisposable

## Remarks

It uses a string as key and a JSON object as value. Each container is intended to store the entities \/ records of a specific type. E.g. one container for storing JSON objects representing 'articles' another one for storing 'orders'.

EntityContainer define the entire set of interfaces a database adapter needs to implement to               enable the complete feature set of [EntitySet\<T1, T2\>](../../Client/EntitySet-2/index.md) and [FlioxClient](../../Client/FlioxClient/index.md).EntityContainer and all its implementations must be thread safe.

The interface methods are designed to enable clear, compact and efficient implementations of database operations. E.g. operations like SELECT, INSERT, DELETE or UPDATE in case of an SQL database adapter.[MemoryContainer](../MemoryContainer/index.md), [FileContainer](../FileContainer/index.md) and `CosmosContainer` show straight forward implementation of EntityContainer. Additional to memory implementation [FileContainer](../FileContainer/index.md) shows also how to handle database errors. These errors fall into two categories:

1. A complete database request fails. E.g. a SELECT in SQL.                     \=\> [Error](../../Protocol/Models/ICommandResult/properties/Error.md) need to be set.

2. The database request was successful, but one or more entities (key\/values) had an error when accessing.                     E.g. Writing an entity to a file with a [FileContainer](../FileContainer/index.md) fails because it is used by another process.                     \=\> An [EntityError](../../Protocol/Models/EntityError/index.md) need to be added to task result errors.                        E.g. add an error to [errors](../../Protocol/Tasks/CreateEntitiesResult/fields/errors.md) in case of[CreateEntitiesAsync(CreateEntities, SyncContext)](../FileContainer/methods/CreateEntitiesAsync.md)All ...Result types returned by the interface methods of EntityContainer like[CreateEntitiesAsync(CreateEntities, SyncContext)](methods/CreateEntitiesAsync.md), [ReadEntitiesAsync(ReadEntities, SyncContext)](methods/ReadEntitiesAsync.md), ... implement [ICommandResult](../../Protocol/Models/ICommandResult/index.md). In case a database command fails completely  [Error](../../Protocol/Models/ICommandResult/properties/Error.md) needs to be set. See [ExecuteRequestAsync(SyncRequest, SyncContext)](../FlioxHub/methods/ExecuteRequestAsync.md) for proper error handling.

## Fields

| Name                             | Description      |
| -------------------------------- | ---------------- |
| [name](fields/name.md)           |  container name  |
| [nameShort](fields/nameShort.md) |                  |

## Properties

| Name                           | Description |
| ------------------------------ | ----------- |
| [Pretty](properties/Pretty.md) |             |

## Methods

| Name                                                                                        | Description                                                              |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [AggregateEntitiesAsync(AggregateEntities, SyncContext)](methods/AggregateEntitiesAsync.md) | Performs an aggregation specified in the given `command`                 |
| [CreateEntities(CreateEntities, SyncContext)](methods/CreateEntities.md)                    |                                                                          |
| [CreateEntitiesAsync(CreateEntities, SyncContext)](methods/CreateEntitiesAsync.md)          | Create the entities specified in the given `command`                     |
| [DeleteEntities(DeleteEntities, SyncContext)](methods/DeleteEntities.md)                    | Delete entities by id with the ids passed in the given `command`         |
| [DeleteEntitiesAsync(DeleteEntities, SyncContext)](methods/DeleteEntitiesAsync.md)          | Delete entities by id with the ids passed in the given `command`         |
| [Dispose()](methods/Dispose.md)                                                             |                                                                          |
| [MergeEntities(MergeEntities, SyncContext)](methods/MergeEntities.md)                       | Can be implemented used to merge entities synchronously for optimization |
| [MergeEntitiesAsync(MergeEntities, SyncContext)](methods/MergeEntitiesAsync.md)             | Apply the given `mergeEntities` to the container entities                |
| [QueryEntities(QueryEntities, SyncContext)](methods/QueryEntities.md)                       | Query entities using the filter in the given `command`                   |
| [QueryEntitiesAsync(QueryEntities, SyncContext)](methods/QueryEntitiesAsync.md)             | Query entities using the filter in the given `command`                   |
| [ReadEntities(ReadEntities, SyncContext)](methods/ReadEntities.md)                          | Read entities by id with the ids passed in the given `command`           |
| [ReadEntitiesAsync(ReadEntities, SyncContext)](methods/ReadEntitiesAsync.md)                | Read entities by id with the ids passed in the given `command`           |
| [ToString()](methods/ToString.md)                                                           |                                                                          |
| [UpsertEntities(UpsertEntities, SyncContext)](methods/UpsertEntities.md)                    | Upsert the entities specified in the given `command`                     |
| [UpsertEntitiesAsync(UpsertEntities, SyncContext)](methods/UpsertEntitiesAsync.md)          | Upsert the entities specified in the given `command`                     |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
