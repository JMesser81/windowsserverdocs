# HcnEnumerateNetworks

## Syntax
`HRESULT result = HcnEnumerateNetworks(query, networks, error)
### Parameters
|Parameter     |Description|
|---|---|---|---|---|---|---|---| 
|`Query`| [String] [In] [Optional] specifies a JSON document for a query containing properties of the specific networks to be returned. By default, all networks are returned|
|`Networks`| [Out] Receives a JSON document with the list of networks|
|`ErrorRecord`| [Out] [Optional] Receives a JSON document on failure with extended result information. The call must release the buffer using CoTaskMemFree|
|    |    | 



## Return Values
|Return | Description|
|---|---|
|`S_OK`|On success|
|HResult error code|Failure|
|     |     |

## Remarks