# Disable-SFNode
Deactivate a Service Fabric cluster node with the specified deactivation intent.
## Description

Deactivate a Service Fabric cluster node with the specified deactivation intent. Once the deactivation is in progress, 
the deactivation intent can be increased, but not decreased (for example, a node that is deactivated with the Pause 
intent can be deactivated further with Restart, but not the other way around. Nodes may be reactivated using the 
Activate a node operation any time after they are deactivated. If the deactivation is not complete, this will cancel 
the deactivation. A node that goes down and comes back up while deactivated will still need to be reactivated before 
services will be placed on that node.



## Optional Parameters
#### -DeactivationIntent

Describes the intent or reason for deactivating the node. The possible values are following.
                    . Possible values include: 'Pause', 'Restart', 'RemoveData'



#### -ServerTimeout

The server timeout for performing the operation in seconds. This timeout specifies the time duration that the client 
is willing to wait for the requested operation to complete. The default value for this parameter is 60 seconds.



