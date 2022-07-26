﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# MessageContext.Error Method

**Declaring Type:** [MessageContext](../index.md)  
**Namespace:** [Friflo.Json.Fliox.Hub.Host](../../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

## Overloads

| Signature                                       | Description                                                                                                                                                                                                               |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Error(string)](#errorstring)                   | Set result of [MessageContext](../index.md) execution to an error                                                                                                                                                         |
| [Error\<TResult\>(string)](#errortresultstring) | Set result of [MessageContext](../index.md) execution to an error.             It returns the default value of the given `TResult` to simplify             returning from a command handler with a single statement like: |

## Error(string)

Set result of [MessageContext](../index.md) execution to an error

```csharp
public void Error(string message);
```

### Parameters

`message`  string

## Error\<TResult\>(string)

Set result of [MessageContext](../index.md) execution to an error.             It returns the default value of the given `TResult` to simplify             returning from a command handler with a single statement like:

```
if (!command.ValidateParam(out var param, out var error))
    return command.Error <int>(error);
```
```csharp
public TResult Error<TResult>(string message);
```

### Type Parameters

`TResult`

### Parameters

`message`  string

### Returns

TResult

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
