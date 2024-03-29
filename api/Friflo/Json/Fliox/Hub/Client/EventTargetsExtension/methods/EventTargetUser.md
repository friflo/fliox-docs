﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EventTargetsExtension.EventTargetUser Method

**Declaring Type:** [EventTargetsExtension](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Client](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

## Overloads

| Signature                                                                              | Description                                              |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| [EventTargetUser\<TTask\>(TTask, ShortString)](#eventtargetuserttaskttask-shortstring) |  Send the `message` as an event only to the given `user` |
| [EventTargetUser\<TTask\>(TTask, string)](#eventtargetuserttaskttask-string)           |  Send the `message` as an event only to the given `user` |

## EventTargetUser\<TTask\>(TTask, ShortString)

 Send the `message` as an event only to the given `user`

```csharp
public static TTask EventTargetUser<TTask>(this TTask message, in ShortString user);
```

### Type Parameters

`TTask`

### Parameters

`message`  TTask

`user`  ShortString

### Returns

TTask

### See Also

- [EventTargets](../../EventTargets/index.md)

## EventTargetUser\<TTask\>(TTask, string)

 Send the `message` as an event only to the given `user`

```csharp
public static TTask EventTargetUser<TTask>(this TTask message, string user);
```

### Type Parameters

`TTask`

### Parameters

`message`  TTask

`user`  string

### Returns

TTask

### See Also

- [EventTargets](../../EventTargets/index.md)

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
