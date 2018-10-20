# HcnCreateEndpoint

## Syntax
`HRESULT result = HcnCreateEndpoint(Network, Id, Settings, Endpoint, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Network`| **[In]** Handle to the network on which endpoint is to be created.|
|`Id`| **[In]** specifies a unique GUID string by which the Endpoint will be referenced|
|`Settings`| **[In]** JSON document specifying the settings of the new Endpoint|
|`Endpoint`| **[Out]** Receives a handle to the newly created Endpoint|
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