# Get-SFSubNameInfoList
Enumerates all the Service Fabric names under a given name.
## Description

Enumerates all the Service Fabric names under a given name. If the subnames do not fit in a page, one page of results 
is returned as well as a continuation token, which can be used to get the next page. Querying a name that doesn't 
exist will fail.



## Optional Parameters
#### -Recursive

Allows specifying that the search performed should be recursive.



#### -ServerTimeout

The server timeout for performing the operation in seconds. This timeout specifies the time duration that the client 
is willing to wait for the requested operation to complete. The default value for this parameter is 60 seconds.



