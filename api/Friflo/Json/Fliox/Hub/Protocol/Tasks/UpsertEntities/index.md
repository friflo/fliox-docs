﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# UpsertEntities Class

**Namespace:** [Friflo.Json.Fliox.Hub.Protocol.Tasks](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Upsert the given [entities](fields/entities.md) in the specified [container](fields/container.md)

```csharp
public sealed class UpsertEntities : SyncRequestTask
```

**Inheritance:** object → [SyncRequestTask](../SyncRequestTask/index.md) → UpsertEntities

## Constructors

| Name                                      | Description |
| ----------------------------------------- | ----------- |
| [UpsertEntities()](constructors/index.md) |             |

## Fields

| Name                                         | Description                                                                                             |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| [container](fields/container.md)             | container name the [entities](fields/entities.md) are upserted \- created or updated                    |
| [entities](fields/entities.md)               | the [entities](fields/entities.md) which are upserted in the specified [container](fields/container.md) |
| [entityContainer](fields/entityContainer.md) |                                                                                                         |
| [keyName](fields/keyName.md)                 | name of the primary key property in [entities](fields/entities.md)                                      |

## Properties

| Name                               | Description |
| ---------------------------------- | ----------- |
| [TaskName](properties/TaskName.md) |             |
| [TaskType](properties/TaskType.md) |             |

## Methods

| Name                                                                               | Description |
| ---------------------------------------------------------------------------------- | ----------- |
| [Execute(EntityDatabase, SyncResponse, SyncContext)](methods/Execute.md)           |             |
| [ExecuteAsync(EntityDatabase, SyncResponse, SyncContext)](methods/ExecuteAsync.md) |             |
| [IsNop()](methods/IsNop.md)                                                        |             |
| [PreExecute(EntityDatabase, SharedEnv)](methods/PreExecute.md)                     |             |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
