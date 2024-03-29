﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# ClientController Class

**Namespace:** [Friflo.Json.Fliox.Hub.Host.Auth](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

ClientController us used to create unique client ids

```csharp
public abstract class ClientController
```

**Inheritance:** object → ClientController

## Remarks

It creates a unique client id for a given [User](../User/index.md) by [NewClientIdFor(User)](methods/NewClientIdFor.md) or checks if a given client id can be used (added) for a given [User](../User/index.md) by [UseClientIdFor(User, ShortString)](methods/UseClientIdFor.md). Multiple client ids can be added to a [User](../User/index.md). Once added to a [User](../User/index.md) the client id cannot be used (added) by another [User](../User/index.md).A ClientController is used to:

## Methods

| Name                                                           | Description |
| -------------------------------------------------------------- | ----------- |
| [NewClientIdFor(User)](methods/NewClientIdFor.md)              |             |
| [ToString()](methods/ToString.md)                              |             |
| [UseClientIdFor(User, ShortString)](methods/UseClientIdFor.md) |             |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
