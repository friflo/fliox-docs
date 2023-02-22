﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# SyncFunction.OnSync Field

**Declaring Type:** [SyncFunction](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Client](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

A handler method assigned to OnSync is called after executing a [SyncTask](../../SyncTask/index.md) with[SyncTasks()](../../FlioxClient/methods/SyncTasks.md). This is an alternative way to process a [SyncTask](../../SyncTask/index.md) result to the common task processing shown below.

```csharp
[DebuggerBrowsable(DebuggerBrowsableState.Never)]
public Action<TaskError> OnSync;
```

## Field Value

Action\<[TaskError](../../TaskError/index.md)\>

## Remarks

It is intended to be used in scenarios where a set of tasks are not created in a single function block like in the example below. This is typical for game applications where [SyncTasks()](../../FlioxClient/methods/SyncTasks.md) is called by the game loop for every frame to batch multiple [SyncTask](../../SyncTask/index.md)'s created on various places. 

```
// Common task processing
var articles = client.articles.QueryAll();
var orders   = client.orders.QueryAll();
await client.SyncTasks(); 
foreach (var article in articles) { ... }
foreach (var order in orders) { ... }
```
___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*