﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# UpsertEntitiesResult Class

**Namespace:** [Friflo.Json.Fliox.Hub.Protocol.Tasks](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Result of a [UpsertEntities](../UpsertEntities/index.md) task

```csharp
public sealed class UpsertEntitiesResult : SyncTaskResult, ICommandResult
```

**Inheritance:** object → [SyncTaskResult](../SyncTaskResult/index.md) → UpsertEntitiesResult

**Implements:** [ICommandResult](../../Models/ICommandResult/index.md)

## Constructors

| Name                                            | Description |
| ----------------------------------------------- | ----------- |
| [UpsertEntitiesResult()](constructors/index.md) |             |

## Fields

| Name                       | Description                            |
| -------------------------- | -------------------------------------- |
| [errors](fields/errors.md) | list of entity errors failed to upsert |

## Properties

| Name                         | Description |
| ---------------------------- | ----------- |
| [Error](properties/Error.md) |             |

## Methods

| Name                                                          | Description |
| ------------------------------------------------------------- | ----------- |
| [Create(SyncContext, List\<EntityError\>)](methods/Create.md) |             |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
