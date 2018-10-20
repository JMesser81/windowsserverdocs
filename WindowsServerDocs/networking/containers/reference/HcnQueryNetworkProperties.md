# HcnQueryNetworkProperties

## Syntax
`HRESULT result = HcnQueryNetworkProperties(Network, Query, Properties, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Network`| **[In]** handle to an open Network|
|`Query`| **[In] [Optional]** Optionally specifies a JSON document for a query containing specific properties of the Network returned. By default, all properties are returned.|
|`Properties`| **[Out]** Receives a JSON document with Network properties.|
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