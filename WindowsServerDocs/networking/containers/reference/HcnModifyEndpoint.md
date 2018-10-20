# HcnModifyEndpoint

## Syntax
`HRESULT result = HcnModifyEndpoint(Endpoint, Settings, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Endpoint`| **[In]** handle to the Endpoint (received from call to HcnOpenEndpoint)|
|`Settings`| **[Out]** JSON document specifying the new settings of the Endpoint|
|`ErrorRecord`| **[Out] [Optional]** Receives a JSON document on failure with extended result information|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks
