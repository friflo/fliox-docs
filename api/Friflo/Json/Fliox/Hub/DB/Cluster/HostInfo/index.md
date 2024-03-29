﻿<!--  
  <auto-generated>   
    The contents of this file were generated by a tool.  
    Changes to this file may be list if the file is regenerated  
  </auto-generated>   
-->

# HostInfo Class

**Namespace:** [Friflo.Json.Fliox.Hub.DB.Cluster](../index.md)  
**Assembly:** Friflo.Json.Fliox.Hub

general information about a Hub

```csharp
public sealed class HostInfo
```

**Inheritance:** object → HostInfo

## Constructors

| Name                                | Description |
| ----------------------------------- | ----------- |
| [HostInfo()](constructors/index.md) |             |

## Fields

| Name                                       | Description                                                                                                                                              |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [envColor](fields/envColor.md)             | the color used to display the environment name in GUI's using CSS color format.E.g. using red for a production environment: "\#ff0000" or "rgb(255 0 0)" |
| [envName](fields/envName.md)               | environment name. e.g. 'dev', 'test', 'staging', 'prod'                                                                                                  |
| [flioxVersion](fields/flioxVersion.md)     | Fliox library version                                                                                                                                    |
| [hostName](fields/hostName.md)             | host name used to identify a specific host in a network.                                                                                                 |
| [hostVersion](fields/hostVersion.md)       | host version                                                                                                                                             |
| [memory](fields/memory.md)                 |                                                                                                                                                          |
| [projectName](fields/projectName.md)       | project name                                                                                                                                             |
| [projectWebsite](fields/projectWebsite.md) | link to a website describing project and Hub                                                                                                             |
| [pubSub](fields/pubSub.md)                 |  is true if host support Pub\-Sub.                                                                                                                       |
| [routes](fields/routes.md)                 | routes configures by [HttpHost](../../../Remote/HttpHost/index.md) \- commonly below `/fliox`                                                            |

___

*Documentation generated by [MdDocs](https://github.com/ap0llo/mddocs)*
