﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# EntityUtils.CopyEntities Method

**Declaring Type:** [EntityUtils](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host.Utils](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Copy the given `entities` to the given `destEntities`. The given `keyName` identifies the key property inside the JSON value in the given list of `entities`.

```csharp
public static void CopyEntities(List<JsonValue> entities, string keyName, bool? isIntKey, string newKeyName, EntityValue[] destEntities, SyncContext syncContext);
```

## Parameters

`entities`  List\<JsonValue\>

`keyName`  string

`isIntKey`  Nullable\<bool\>

`newKeyName`  string

`destEntities`  [EntityValue](../../../../Protocol/Models/EntityValue/index.md)\[\]

`syncContext`  [SyncContext](../../../SyncContext/index.md)

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
