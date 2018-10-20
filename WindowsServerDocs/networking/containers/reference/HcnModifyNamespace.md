# HcnModifyNamespace

## Syntax
`HRESULT result = HcnModifyNamespace(Namespace, Settings, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Namespace`| **[In]** handle to the Namespace (received from call to HcnOpenNamespace)|
|`Settings`| **[In]** JSON document specifying the new settings of the Namespace|
|`ErrorRecord`| **[Out] [Optional]** Receives a JSON document on failure with extended result information|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks
