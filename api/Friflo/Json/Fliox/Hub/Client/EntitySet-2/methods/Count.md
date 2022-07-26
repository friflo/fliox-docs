﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EntitySet\<TKey, T\>.Count Method

**Declaring Type:** [EntitySet\<TKey, T\>](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Client](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Create a [CountTask\<T\>](../../CountTask-1/index.md) counting all entities matching to the given LINQ query `filter`

```csharp
public CountTask<T> Count(Expression<Func<T, bool>> filter);
```

## Parameters

`filter`  Expression\<Func\<T, bool\>\>

## Remarks

 To execute the task call [SyncTasks()](../../FlioxClient/methods/SyncTasks.md)

## Returns

CountTask\<T\>

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
