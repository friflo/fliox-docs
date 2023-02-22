﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# DatabaseServiceQueue.ExecuteQueuedRequests Method

**Declaring Type:** [DatabaseServiceQueue](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Execute queued requests which can be executed synchronous. Return all requests which require asynchronous execution in `asyncServiceJobs`

```csharp
public int ExecuteQueuedRequests(out AsyncServiceJobs asyncServiceJobs);
```

## Parameters

`asyncServiceJobs`  AsyncServiceJobs

## Returns

int

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*