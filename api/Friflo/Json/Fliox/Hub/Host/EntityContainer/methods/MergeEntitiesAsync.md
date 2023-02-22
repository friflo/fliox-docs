﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EntityContainer.MergeEntitiesAsync Method

**Declaring Type:** [EntityContainer](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Apply the given `mergeEntities` to the container entities

```csharp
[AsyncStateMachine(Friflo.Json.Fliox.Hub.Host.EntityContainer/<MergeEntitiesAsync>d__22)]
[DebuggerStepThrough]
public Task<MergeEntitiesResult> MergeEntitiesAsync(MergeEntities mergeEntities, SyncContext syncContext);
```

## Parameters

`mergeEntities`  [MergeEntities](../../../Protocol/Tasks/MergeEntities/index.md)

`syncContext`  [SyncContext](../../SyncContext/index.md)

## Remarks

Default implementation to apply patches to entities. The implementation perform three steps: 1. Read entities to be patches from a database 2. Apply merge patches 3. Write back the merged entities  If the used database has integrated support for merging (patching) JSON its [EntityContainer](../index.md)implementation can override this method to replace two database requests by one.

## Returns

Task\<[MergeEntitiesResult](../../../Protocol/Tasks/MergeEntitiesResult/index.md)\>

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*