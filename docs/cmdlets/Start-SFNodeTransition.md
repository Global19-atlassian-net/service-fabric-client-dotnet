# Start-SFNodeTransition
Starts or stops a cluster node.
## Description

Starts or stops a cluster node.  A cluster node is a process, not the OS instance itself.  To start a node, pass in 
"Start" for the NodeTransitionType parameter.
                To stop a node, pass in "Stop" for the NodeTransitionType parameter.  This API starts the operation - 
when the API returns the node may not have finished transitioning yet.
                Call GetNodeTransitionProgress with the same OperationId to get the progress of the operation.



## Required Parameters
#### -NodeName

The name of the node.



#### -OperationId

A GUID that identifies a call of this API.  This is passed into the corresponding GetProgress API



#### -NodeTransitionType

Indicates the type of transition to perform.  NodeTransitionType.Start will start a stopped node.  
NodeTransitionType.Stop will stop a node that is up. Possible values include: 'Invalid', 'Start', 'Stop'



#### -NodeInstanceId

The node instance ID of the target node.  This can be determined through GetNodeInfo API.



#### -StopDurationInSeconds

The duration, in seconds, to keep the node stopped.  The minimum value is 600, the maximum is 14400.  After this time 
expires, the node will automatically come back up.



