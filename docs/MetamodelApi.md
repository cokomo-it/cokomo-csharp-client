# CoKoMo.CoKoMoApiClient.Api.MetamodelApi

All URIs are relative to *https://cokomo.code4you.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MetamodelGet**](MetamodelApi.md#metamodelget) | **GET** /Metamodel |  |

<a id="metamodelget"></a>
# **MetamodelGet**
> Metamodel MetamodelGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using CoKoMo.CoKoMoApiClient.Api;
using CoKoMo.CoKoMoApiClient.Client;
using CoKoMo.CoKoMoApiClient.Model;

namespace Example
{
    public class MetamodelGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://cokomo.code4you.com";
            var apiInstance = new MetamodelApi(config);

            try
            {
                Metamodel result = apiInstance.MetamodelGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MetamodelApi.MetamodelGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MetamodelGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<Metamodel> response = apiInstance.MetamodelGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MetamodelApi.MetamodelGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**Metamodel**](Metamodel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

