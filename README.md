

### Client

*Example client*
[`Todo/Client/TodoClient.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Todo/Client/TodoClient.cs)
and its utilization
[`Todo/Test/Trial.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Todo/Test/Trial.cs)
| Namespace    | Class                                                                                 | Description                                                                             |
| -------------|-------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| .Client      | [FlioxClient](api/Friflo/Json/Fliox/Hub/Client/FlioxClient/index.md)                  | `FlioxClient` subclasses are used as database clients and database schema               |
| .Client      | [EntitySet<,>](api/Friflo/Json/Fliox/Hub/Client/EntitySet-2/index.md)                 | Strongly typed API to a database container used as property in a `FlioxClient` subclass |
| .Remote      | [HttpClientHub](api/Friflo/Json/Fliox/Hub/Remote/HttpClientHub/index.md)              | Connects to a Hub via **HTTP** by passing it to a `FlioxClient` constructor             |
| .Remote      | [WebSocketClientHub](api/Friflo/Json/Fliox/Hub/Remote/WebSocketClientHub/index.md)    | Connects to a Hub via **Websocket** by passing it to a `FlioxClient` constructor        |


### Host

*Example HTTP Hub* 
[`Todo/Hub/Program.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Todo/Hub/Program.cs)

| Namespace    | Class                                                                                 | Description                                                          |
| ------------ |-------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| .Remote      | [HttpHost](api/Friflo/Json/Fliox/Hub/Remote/HttpHost/index.md)                        | Enable access to a `FlioxHub` via **HTTP** and **WebSocket**         |
| .Remote      | [StaticFileHandler](api/Friflo/Json/Fliox/Hub/Remote/StaticFileHandler/index.md)      | Used to add static files to the `HttpHost` like the **Hub Explorer** |
| .Host        | [FlioxHub](api/Friflo/Json/Fliox/Hub/Host/FlioxHub/index.md)                          | Used as a Proxy between a `FlioxClient` and a database               |
| .Host        | [FileDatabase](api/Friflo/Json/Fliox/Hub/Host/FileDatabase/index.md)                  | Database storing records in the `file-system`                        |
| .Host        | [MemoryDatabase](api/Friflo/Json/Fliox/Hub/Host/MemoryDatabase/index.md)              | Database storing records `in-memory`                                 |
| .Host        | [DatabaseSchema](api/Friflo/Json/Fliox/Hub/Host/DatabaseSchema/index.md)              | Used to assign a **schema** to a database                            |
| .Host.Event  | [EventDispatcher](api/Friflo/Json/Fliox/Hub/Host/Event/EventDispatcher/index.md)      | Enables **Pub-Sub** by a `FlioxHub`                                  |


### DB

*Configure support databases*
[`Demo/Hub/Program.cs`](https://github.com/friflo/FlioxHub.Demos/blob/main/Demo/Hub/Program.cs)
| Namespace    | Class                                                                                 | Description                                               |
| ------------ |-------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| .DB.Cluster  | [ClusterDB](api/Friflo/Json/Fliox/Hub/DB/Cluster/ClusterDB/index.md)                  | Expose information of hosted databases as a database      |
| .DB.Monitor  | [MonitorDB](api/Friflo/Json/Fliox/Hub/DB/Monitor/MonitorDB/index.md)                  | Expose request information of a `FlioxHob` as a database  |
| .DB.UserAuth | [UserAuthenticator](api/Friflo/Json/Fliox/Hub/DB/UserAuth/UserAuthenticator/index.md) | Performs user authentication and authorization            |





