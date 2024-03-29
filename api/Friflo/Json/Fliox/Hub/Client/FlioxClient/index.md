﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# FlioxClient Class

**Namespace:** [Friflo.Json.Fliox.Hub.Client](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

Application classes extending FlioxClient offer two main functionalities:  Define a  by declaring its containers, commands and messages  Its instances are  providing type\-safe access to database containers, commands and messages

```csharp
[CLSCompliant(true)]
[TypeMapper(Friflo.Json.Fliox.Hub.Client.Internal.Map.FlioxClientMatcher)]
public class FlioxClient : IDisposable, IResetable, ILogSource
```

**Inheritance:** object → FlioxClient

**Attributes:** CLSCompliantAttribute,TypeMapperAttribute

**Implements:** IDisposable,IResetable,ILogSource

## Remarks

Its containers are fields or properties of type [EntitySet\<T1, T2\>](../EntitySet-2/index.md).Its commands are methods returning a [CommandTask\<T\>](../CommandTask-1/index.md).Its messages are methods returning a [MessageTask](../MessageTask/index.md).FlioxClient instances can be used in server and client code.The FlioxClient features and utilization available at

## Constructors

| Name                                                                  | Description                                                                                                                                            |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [FlioxClient(FlioxHub, string, ClientOptions)](constructors/index.md) | Instantiate a FlioxClient for the `dbName` exposed by the given `hub`. If `dbName` is null the client uses the default database assigned to the `hub`. |

## Fields

| Name                 | Description                                                                     |
| -------------------- | ------------------------------------------------------------------------------- |
| [std](fields/std.md) |  access to standard database commands \- [StdCommands](../StdCommands/index.md) |

## Properties

| Name                                                               | Description                                                                                                                          |
| ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| [ClientId](properties/ClientId.md)                                 | client id \- identifies the client at a Hub                                                                                          |
| [ClientInfo](properties/ClientInfo.md)                             |  general client information: attached database, the number of cached entities and scheduled [Tasks](properties/Tasks.md)             |
| [DatabaseName](properties/DatabaseName.md)                         |  name of the database the client is attached to                                                                                      |
| [Functions](properties/Functions.md)                               |                                                                                                                                      |
| [Logger](properties/Logger.md)                                     |                                                                                                                                      |
| [SubscriptionEventHandler](properties/SubscriptionEventHandler.md) | [SubscriptionEventHandler](properties/SubscriptionEventHandler.md) is called for all subscription events received by the FlioxClient |
| [Tasks](properties/Tasks.md)                                       |  List of tasks created by its FlioxClient methods. These tasks are executed when calling [SyncTasks()](methods/SyncTasks.md)         |
| [Token](properties/Token.md)                                       | [Token](properties/Token.md) \- used to authenticate the [UserId](properties/UserId.md) at the Hub                                   |
| [UserId](properties/UserId.md)                                     | user id \- identifies the user at a Hub                                                                                              |
| [UserInfo](properties/UserInfo.md)                                 | Is the tuple of [UserId](properties/UserId.md), [Token](properties/Token.md) and [ClientId](properties/ClientId.md)                  |
| [WriteNull](properties/WriteNull.md)                               |  If true the serialization of entities to JSON write null fields. Otherwise null fields are omitted                                  |
| [WritePretty](properties/WritePretty.md)                           |  If true the serialization of entities to JSON is prettified                                                                         |

## Methods

| Name                                                                                                                                                                                | Description                                                                                                                                                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [CancelPendingSyncs()](methods/CancelPendingSyncs.md)                                                                                                                               |  Cancel execution of pending calls to [SyncTasks()](methods/SyncTasks.md) and [TrySyncTasks()](methods/TrySyncTasks.md)                                                                                                                                                               |
| [DetectAllPatches()](methods/DetectAllPatches.md)                                                                                                                                   | Detect the  made to all tracked entities in all s of the client. Detected patches are applied to the database containers when calling [SyncTasks()](methods/SyncTasks.md).                                                                                                            |
| [Dispose()](methods/Dispose.md)                                                                                                                                                     |                                                                                                                                                                                                                                                                                       |
| [GetEntitySets(FlioxClient)](methods/GetEntitySets.md)                                                                                                                              |                                                                                                                                                                                                                                                                                       |
| [GetEntityTypes(Type)](methods/GetEntityTypes.md)                                                                                                                                   | Return the Type's used by the [EntitySet\<T1, T2\>](../EntitySet-2/index.md) members of a FlioxClient as entity Type.                                                                                                                                                                 |
| [GetPendingSyncCount()](methods/GetPendingSyncCount.md)                                                                                                                             |  Return the number of pending [SyncTasks()](methods/SyncTasks.md) and [TrySyncTasks()](methods/TrySyncTasks.md) calls                                                                                                                                                                 |
| [GetSyncCount()](methods/GetSyncCount.md)                                                                                                                                           |  Return the number of calls to [SyncTasks()](methods/SyncTasks.md) and [TrySyncTasks()](methods/TrySyncTasks.md)                                                                                                                                                                      |
| [Reset()](methods/Reset.md)                                                                                                                                                         |  Remove all tasks and all tracked entities of the FlioxClient                                                                                                                                                                                                                         |
| [SendCommand\<TParam, TResult\>(string, TParam)](methods/SendCommand.md#sendcommandtparam-tresultstring-tparam)                                                                     | Send a command with the given `name` and `param` value to a database. Other clients can subscribe the command to receive an event with [SubscribeMessage(string, MessageSubscriptionHandler)](methods/SubscribeMessage.md#subscribemessagestring-messagesubscriptionhandler).         |
| [SendCommand\<TResult\>(string)](methods/SendCommand.md#sendcommandtresultstring)                                                                                                   | Send a command with the given `name` (without a command value) to a database. Other clients can subscribe the command to receive an event with [SubscribeMessage(string, MessageSubscriptionHandler)](methods/SubscribeMessage.md#subscribemessagestring-messagesubscriptionhandler). |
| [SendMessage(string)](methods/SendMessage.md#sendmessagestring)                                                                                                                     | Send a message with the given `name` (without a value) to a database. Other clients can subscribe the message to receive an event with [SubscribeMessage(string, MessageSubscriptionHandler)](methods/SubscribeMessage.md#subscribemessagestring-messagesubscriptionhandler).         |
| [SendMessage\<TMessage\>(string, TMessage)](methods/SendMessage.md#sendmessagetmessagestring-tmessage)                                                                              | Send a message with the given `name` and `param` value to a database. Other clients can subscribe the message to receive an event with [SubscribeMessage(string, MessageSubscriptionHandler)](methods/SubscribeMessage.md#subscribemessagestring-messagesubscriptionhandler).         |
| [SetEventProcessor(EventProcessor)](methods/SetEventProcessor.md)                                                                                                                   | Set the [EventProcessor](../EventProcessor/index.md) used to process subscription events subscribed by a FlioxClient                                                                                                                                                                  |
| [SubscribeAllChanges(Change, ChangeSubscriptionHandler)](methods/SubscribeAllChanges.md)                                                                                            | Subscribe to database changes of all [EntityContainer](../../Host/EntityContainer/index.md)'s with the given `change`. To unsubscribe from receiving change events set `change` to None.                                                                                              |
| [SubscribeMessage(string, MessageSubscriptionHandler)](methods/SubscribeMessage.md#subscribemessagestring-messagesubscriptionhandler)                                               |  Subscribe message \/ command with the given `name` send to the database used by the client                                                                                                                                                                                           |
| [SubscribeMessage\<TMessage\>(string, MessageSubscriptionHandler\<TMessage\>)](methods/SubscribeMessage.md#subscribemessagetmessagestring-messagesubscriptionhandlertmessage)       |                                                                                                                                                                                                                                                                                       |
| [SyncTasks()](methods/SyncTasks.md)                                                                                                                                                 |  Execute all tasks created by methods of [EntitySet\<T1, T2\>](../EntitySet-2/index.md) and FlioxClient                                                                                                                                                                               |
| [SyncTasksSynchronous()](methods/SyncTasksSynchronous.md)                                                                                                                           |  Execute all tasks created by methods of [EntitySet\<T1, T2\>](../EntitySet-2/index.md) and FlioxClient                                                                                                                                                                               |
| [ToString()](methods/ToString.md)                                                                                                                                                   |                                                                                                                                                                                                                                                                                       |
| [TrySyncTasks()](methods/TrySyncTasks.md)                                                                                                                                           |  Execute all tasks created by methods of [EntitySet\<T1, T2\>](../EntitySet-2/index.md) and FlioxClient                                                                                                                                                                               |
| [TrySyncTasksSynchronous()](methods/TrySyncTasksSynchronous.md)                                                                                                                     |  Execute all tasks created by methods of [EntitySet\<T1, T2\>](../EntitySet-2/index.md) and FlioxClient                                                                                                                                                                               |
| [UnsubscribeMessage(string, MessageSubscriptionHandler)](methods/UnsubscribeMessage.md#unsubscribemessagestring-messagesubscriptionhandler)                                         |  Remove subscription of message \/ command with the given `name` send to the database used by the client                                                                                                                                                                              |
| [UnsubscribeMessage\<TMessage\>(string, MessageSubscriptionHandler\<TMessage\>)](methods/UnsubscribeMessage.md#unsubscribemessagetmessagestring-messagesubscriptionhandlertmessage) |                                                                                                                                                                                                                                                                                       |

## Nested Types

| Name                                      | Description |
| ----------------------------------------- | ----------- |
| [FlioxClient.SendTask](SendTask/index.md) |             |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
