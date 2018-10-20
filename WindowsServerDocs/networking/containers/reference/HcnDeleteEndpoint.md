# HcnDeleteEndpoint

## Syntax
`HRESULT result = HcnDeleteEndpoint(Id, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Id`| **[In]** the Unique Id (GUID) string of the existing Endpoint|
|`ErrorRecord`| **[Out] [Optional]** Receives a JSON document on failure with extended result information|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks

All clients/callers are responsible for cleaning up ErrorRecord buffer upon exit