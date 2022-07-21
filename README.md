# API Reference

This project contains the API Reference of [**Json.Fliox**](https://github.com/friflo/Friflo.Json.Fliox) library.    
Following sections list fundamental [Friflo.Json.Fliox.Hub.*](api/Friflo/Json/Fliox/Hub/index.md) classes grouped by their **use case**.  
These groups fit mainly to their namespaces. Except `.Remote` containing client as well server classes. 

### Client

*Example client*
[`Todo/Client/TodoClient.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Todo/Client/TodoClient.cs)
*and client utilization*
[`Todo/Test/Trial.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Todo/Test/Trial.cs)

| Namespace    | Class                                                                                 | Description                                                                                          |
| -------------|-------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| .Client      | [FlioxClient](api/Friflo/Json/Fliox/Hub/Client/FlioxClient/index.md)                  | `FlioxClient` subclasses are used as **database clients** and **database schema**                    |
| .Client      | [EntitySet<,>](api/Friflo/Json/Fliox/Hub/Client/EntitySet-2/index.md)                 | **Strongly typed** API to a access a database container used as property in a `FlioxClient` subclass |
| .Remote      | [HttpClientHub](api/Friflo/Json/Fliox/Hub/Remote/HttpClientHub/index.md)              | Connects to a Hub via **HTTP** by passing it to a `FlioxClient` constructor                          |
| .Remote      | [WebSocketClientHub](api/Friflo/Json/Fliox/Hub/Remote/WebSocketClientHub/index.md)    | Connects to a Hub via **Websocket** by passing it to a `FlioxClient` constructor                     |


### Host

*HTTP Hub bootstrapping examples* 
[`Todo/Hub/Program.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Todo/Hub/Program.cs) *and*
[`Todo/Demo/Program.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Demo/Hub/Program.cs)

| Namespace    | Class                                                                                 | Description                                                                     |
| ------------ |-------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| .Remote      | [HttpHost](api/Friflo/Json/Fliox/Hub/Remote/HttpHost/index.md)                        | Host a `FlioxHub` as **HTTP** / **WebSocket** server                            |
| .Remote      | [StaticFileHandler](api/Friflo/Json/Fliox/Hub/Remote/StaticFileHandler/index.md)      | Add static web files to the `HttpHost` like the **Hub Explorer**                |
| .Host        | [FlioxHub](api/Friflo/Json/Fliox/Hub/Host/FlioxHub/index.md)                          | Used as a Proxy between a `FlioxClient` and a concrete database                 |
| .Host        | [FileDatabase](api/Friflo/Json/Fliox/Hub/Host/FileDatabase/index.md)                  | Database storing records in the `file-system`                                   |
| .Host        | [MemoryDatabase](api/Friflo/Json/Fliox/Hub/Host/MemoryDatabase/index.md)              | Database storing records `in-memory`                                            |
| .Host        | [DatabaseSchema](api/Friflo/Json/Fliox/Hub/Host/DatabaseSchema/index.md)              | Used to assign a **schema** to a database                                       |
| .Host        | [TaskHandler](api/Friflo/Json/Fliox/Hub/Host/TaskHandler/index.md)                    | Used to implement custom database commands declared in a `FlioxClient` subclass |
| .Host.Event  | [EventDispatcher](api/Friflo/Json/Fliox/Hub/Host/Event/EventDispatcher/index.md)      | Enables **Pub-Sub** by a `FlioxHub`                                             |


### DB

*Adding support databases example*
[`Demo/Hub/Program.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Demo/Hub/Program.cs)

| Namespace    | Class                                                                                 | Description                                               |
| ------------ |-------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| .DB.Cluster  | [ClusterDB](api/Friflo/Json/Fliox/Hub/DB/Cluster/ClusterDB/index.md)                  | Expose information of hosted databases as a database      |
| .DB.Monitor  | [MonitorDB](api/Friflo/Json/Fliox/Hub/DB/Monitor/MonitorDB/index.md)                  | Expose request information of a `FlioxHob` as a database  |
| .DB.UserAuth | [UserAuthenticator](api/Friflo/Json/Fliox/Hub/DB/UserAuth/UserAuthenticator/index.md) | Performs user authentication and authorization            |





