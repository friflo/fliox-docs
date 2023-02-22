﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# FlioxClient.SyncTasksSynchronous Method

**Declaring Type:** [FlioxClient](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Client](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

 Execute all tasks created by methods of [EntitySet\<T1, T2\>](../../EntitySet-2/index.md) and [FlioxClient](../index.md)

```csharp
public SyncResult SyncTasksSynchronous();
```

## Remarks

In case any task failed a [SyncTasksException](../../SyncTasksException/index.md) is thrown. As an alternative use [TrySyncTasks()](TrySyncTasks.md) to execute tasks which does not throw an exception. The method can be called without awaiting the result of a previous call. 

## Returns

[SyncResult](../../SyncResult/index.md)

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*