# HcnEnumerateEndpoints

## Syntax
`HRESULT result = HcnEnumerateEndpoints(Query, Endpoints, ErrorRecord)`

### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Query`| **[In] [Optional]** specifies a JSON document for a query containing properties of the specific Endpoints to be returned. By default, all Endpoints are returned|
|`Endpoints`| **[Out]** Receives a JSON document with the list of Endpoints|
|`ErrorRecord`| **[Out] [Optional]** Receives a JSON document on failure with extended result information. The call must release the buffer using CoTaskMemFree|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks