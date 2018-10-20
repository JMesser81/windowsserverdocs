# HcnModifyNetwork

## Syntax
`HRESULT result = HcnModifyNetwork(Id, Settings, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Id`| **[In]** handle to the network (received from call to HcnOpenNetwork)|
|`Settings`| **[Out]** JSON document specifying the new settings of the Network|
|`ErrorRecord`| **[Out] [Optional]** Receives a JSON document on failure with extended result information|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks
