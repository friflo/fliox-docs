﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# Friflo.Json.Fliox.Hub.Host.Event Namespace

**Namespace:** [Friflo.Json.Fliox.Hub.Host](../index.md)  

## Classes

| Name                                        | Description                                                                |
| ------------------------------------------- | -------------------------------------------------------------------------- |
| [EventDispatcher](EventDispatcher/index.md) | An [EventDispatcher](EventDispatcher/index.md) is used to enable Pub\-Sub. |
| [EventReceiver](EventReceiver/index.md)     |                                                                            |

## Structs

| Name                                    | Description                                                                                                                                                                                        |
| --------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [SendEventArgs](SendEventArgs/index.md) | Optimization for sending remote events.Avoids frequent allocations of eventBuffer lists [EventMessage](../../Protocol/EventMessage/index.md)[events](../../Protocol/EventMessage/fields/events.md) |

## Enums

| Name                                          | Description                                                                                                                                                                                                       |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [EventDispatching](EventDispatching/index.md) | Specify the way in which events are send to their targets by an [EventDispatcher](EventDispatcher/index.md)Events are generated from the database changes and messages send to a [FlioxHub](../FlioxHub/index.md) |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
