# HcnOpenNetwork

## Syntax
`HRESULT result = HcnOpenNetwork(Id, Network, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Id`| **[In]** the Unique Id (GUID) string of the existing network|
|`Network`| **[Out]** Receives a handle to the Network|
|`ErrorRecord`| **[Out] [Optional]** Receives a JSON document on failure with extended result information|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks

The caller must release any buffers created using CoTaskMemFree