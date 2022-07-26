﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# OperationType Enum

**Namespace:** [Friflo.Json.Fliox.Hub.Host.Auth.Rights](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Use to allow specific container operations in [ContainerAccess](../ContainerAccess/index.md)

```csharp
public enum OperationType
{
    create = 0,
    upsert = 1,
    delete = 2,
    deleteAll = 3,
    merge = 4,
    read = 5,
    query = 6,
    aggregate = 7,
    mutate = 8,
    full = 9
}
```

**Inheritance:** object → ValueType → Enum → OperationType

## Fields

| Name      | Description                                                                    |
| --------- | ------------------------------------------------------------------------------ |
| aggregate | allow to aggregate \- count \- entities in a container                         |
| create    | allow to create entities in a container                                        |
| delete    | allow to delete entities in a container                                        |
| deleteAll | allow to delete all container entities                                         |
| full      | allow all operation types in a container                                       |
| merge     | allow to patch entities in a container                                         |
| mutate    | allow to mutate \- create, upsert, delete and patch \- entities in a container |
| query     | allow to query entities in a container                                         |
| read      | allow to read entities in a container                                          |
| upsert    | allow to upsert entities in a container                                        |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
