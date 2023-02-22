﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EventDispatcher.EnableChangeAccumulation Method

**Declaring Type:** [EventDispatcher](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host.Event](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Enable container change accumulation.Container changes \- create, upsert, merge and delete \- send as [SyncEvent](../../../../Protocol/SyncEvent/index.md)'s tasks to subscribers are accumulated for the given `database`

```csharp
public void EnableChangeAccumulation(EntityDatabase database);
```

## Parameters

`database`  [EntityDatabase](../../../EntityDatabase/index.md)

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*