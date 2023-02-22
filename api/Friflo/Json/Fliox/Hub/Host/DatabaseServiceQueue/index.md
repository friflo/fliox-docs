﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# DatabaseServiceQueue Class

**Namespace:** [Friflo.Json.Fliox.Hub.Host](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

```csharp
public class DatabaseServiceQueue
```

**Inheritance:** object → DatabaseServiceQueue

## Constructors

| Name                                            | Description |
| ----------------------------------------------- | ----------- |
| [DatabaseServiceQueue()](constructors/index.md) |             |

## Methods

| Name                                                                                                                             | Description                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| [ExecuteQueuedRequests(AsyncServiceJobs)](methods/ExecuteQueuedRequests.md)                                                      | Execute queued requests which can be executed synchronous. Return all requests which require asynchronous execution in `asyncServiceJobs`        |
| [ExecuteQueuedRequestsAsync()](methods/ExecuteQueuedRequestsAsync.md#executequeuedrequestsasync)                                 | Execute queued requests in case request queueing is enabled in the [DatabaseService](../DatabaseService/index.md) constructor                    |
| [ExecuteQueuedRequestsAsync(AsyncServiceJobs)](methods/ExecuteQueuedRequestsAsync.md#executequeuedrequestsasyncasyncservicejobs) | Execute requests returned from [ExecuteQueuedRequests(AsyncServiceJobs)](methods/ExecuteQueuedRequests.md) which require asynchronous execution. |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*