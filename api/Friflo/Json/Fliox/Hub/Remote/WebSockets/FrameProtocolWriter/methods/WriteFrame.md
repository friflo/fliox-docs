﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# FrameProtocolWriter.WriteFrame Method

**Declaring Type:** [FrameProtocolWriter](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Remote.WebSockets](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

```csharp
[AsyncStateMachine(Friflo.Json.Fliox.Hub.Remote.WebSockets.FrameProtocolWriter/<WriteFrame>d__6)]
[DebuggerStepThrough]
public Task WriteFrame(Stream stream, byte[] data, int dataOffset, int dataCount, WebSocketMessageType messageType, bool endOfMessage, CancellationToken cancellationToken);
```

## Parameters

`stream`  Stream

`data`  byte\[\]

`dataOffset`  int

`dataCount`  int

`messageType`  WebSocketMessageType

`endOfMessage`  bool

`cancellationToken`  CancellationToken

## Returns

Task

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
