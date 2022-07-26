﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# FlioxClient.SetEventProcessor Method

**Declaring Type:** [FlioxClient](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Client](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Set the [EventProcessor](../../EventProcessor/index.md) used to process subscription events subscribed by a [FlioxClient](../index.md)

```csharp
public void SetEventProcessor(EventProcessor eventProcessor);
```

## Parameters

`eventProcessor`  [EventProcessor](../../EventProcessor/index.md)

## Remarks

By default a [FlioxClient](../index.md) uses a [DirectEventProcessor](../../DirectEventProcessor/index.md) to handle subscription events in the thread an event arrives.In case of an  application consider using a [SynchronizationContextProcessor](../../SynchronizationContextProcessor/index.md) used to process subscription events in the  thread.

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
