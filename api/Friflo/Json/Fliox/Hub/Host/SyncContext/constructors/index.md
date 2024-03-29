﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# SyncContext Constructors

**Declaring Type:** [SyncContext](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

## Overloads

| Signature                                                                                                                  | Description                                                                                     |
| -------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| [SyncContext(SharedEnv, EventReceiver)](#synccontextsharedenv-eventreceiver)                                               |                                                                                                 |
| [SyncContext(SharedEnv, EventReceiver, MemoryBuffer)](#synccontextsharedenv-eventreceiver-memorybuffer)                    |                                                                                                 |
| [SyncContext(SharedEnv, EventReceiver, SyncBuffers, SyncPools)](#synccontextsharedenv-eventreceiver-syncbuffers-syncpools) | Special constructor used to minimize heap allocation. [SyncBuffers](../../SyncBuffers/index.md) |

## SyncContext(SharedEnv, EventReceiver)

```csharp
public SyncContext(SharedEnv sharedEnv, EventReceiver eventReceiver);
```

### Parameters

`sharedEnv`  [SharedEnv](../../SharedEnv/index.md)

`eventReceiver`  [EventReceiver](../../Event/EventReceiver/index.md)

## SyncContext(SharedEnv, EventReceiver, MemoryBuffer)

```csharp
public SyncContext(SharedEnv sharedEnv, EventReceiver eventReceiver, MemoryBuffer memoryBuffer);
```

### Parameters

`sharedEnv`  [SharedEnv](../../SharedEnv/index.md)

`eventReceiver`  [EventReceiver](../../Event/EventReceiver/index.md)

`memoryBuffer`  MemoryBuffer

## SyncContext(SharedEnv, EventReceiver, SyncBuffers, SyncPools)

Special constructor used to minimize heap allocation. [SyncBuffers](../../SyncBuffers/index.md)

```csharp
public SyncContext(SharedEnv sharedEnv, EventReceiver eventReceiver, in SyncBuffers syncBuffers, SyncPools syncPools);
```

### Parameters

`sharedEnv`  [SharedEnv](../../SharedEnv/index.md)

`eventReceiver`  [EventReceiver](../../Event/EventReceiver/index.md)

`syncBuffers`  SyncBuffers

`syncPools`  [SyncPools](../../SyncPools/index.md)

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
