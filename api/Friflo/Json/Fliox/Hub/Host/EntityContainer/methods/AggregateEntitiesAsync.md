﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EntityContainer.AggregateEntitiesAsync Method

**Declaring Type:** [EntityContainer](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Performs an aggregation specified in the given `command`

```csharp
public Task<AggregateEntitiesResult> AggregateEntitiesAsync(AggregateEntities command, SyncContext syncContext);
```

## Parameters

`command`  [AggregateEntities](../../../Protocol/Tasks/AggregateEntities/index.md)

`syncContext`  [SyncContext](../../SyncContext/index.md)

## Returns

Task\<[AggregateEntitiesResult](../../../Protocol/Tasks/AggregateEntitiesResult/index.md)\>

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
