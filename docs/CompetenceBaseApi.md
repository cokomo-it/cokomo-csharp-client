# CoKoMo.CoKoMoApiClient.Api.CompetenceBaseApi

All URIs are relative to *https://cokomo.code4you.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CompetenceBaseIdDetailsGet**](CompetenceBaseApi.md#competencebaseiddetailsget) | **GET** /CompetenceBase/{id}/details |  |
| [**CompetenceBaseIdGet**](CompetenceBaseApi.md#competencebaseidget) | **GET** /CompetenceBase/{id} |  |
| [**CompetenceBaseIdNeighboursGet**](CompetenceBaseApi.md#competencebaseidneighboursget) | **GET** /CompetenceBase/{id}/neighbours |  |

<a id="competencebaseiddetailsget"></a>
# **CompetenceBaseIdDetailsGet**
> CompetenceBase CompetenceBaseIdDetailsGet (string id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using CoKoMo.CoKoMoApiClient.Api;
using CoKoMo.CoKoMoApiClient.Client;
using CoKoMo.CoKoMoApiClient.Model;

namespace Example
{
    public class CompetenceBaseIdDetailsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://cokomo.code4you.com";
            var apiInstance = new CompetenceBaseApi(config);
            var id = "id_example";  // string | 

            try
            {
                CompetenceBase result = apiInstance.CompetenceBaseIdDetailsGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CompetenceBaseApi.CompetenceBaseIdDetailsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CompetenceBaseIdDetailsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CompetenceBase> response = apiInstance.CompetenceBaseIdDetailsGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CompetenceBaseApi.CompetenceBaseIdDetailsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**CompetenceBase**](CompetenceBase.md)

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

<a id="competencebaseidget"></a>
# **CompetenceBaseIdGet**
> CompetenceBase CompetenceBaseIdGet (string id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using CoKoMo.CoKoMoApiClient.Api;
using CoKoMo.CoKoMoApiClient.Client;
using CoKoMo.CoKoMoApiClient.Model;

namespace Example
{
    public class CompetenceBaseIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://cokomo.code4you.com";
            var apiInstance = new CompetenceBaseApi(config);
            var id = "id_example";  // string | 

            try
            {
                CompetenceBase result = apiInstance.CompetenceBaseIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CompetenceBaseApi.CompetenceBaseIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CompetenceBaseIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<CompetenceBase> response = apiInstance.CompetenceBaseIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CompetenceBaseApi.CompetenceBaseIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**CompetenceBase**](CompetenceBase.md)

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

<a id="competencebaseidneighboursget"></a>
# **CompetenceBaseIdNeighboursGet**
> Neighbour CompetenceBaseIdNeighboursGet (string id, int? depth = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using CoKoMo.CoKoMoApiClient.Api;
using CoKoMo.CoKoMoApiClient.Client;
using CoKoMo.CoKoMoApiClient.Model;

namespace Example
{
    public class CompetenceBaseIdNeighboursGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://cokomo.code4you.com";
            var apiInstance = new CompetenceBaseApi(config);
            var id = "id_example";  // string | 
            var depth = 10;  // int? |  (optional)  (default to 10)

            try
            {
                Neighbour result = apiInstance.CompetenceBaseIdNeighboursGet(id, depth);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling CompetenceBaseApi.CompetenceBaseIdNeighboursGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the CompetenceBaseIdNeighboursGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<Neighbour> response = apiInstance.CompetenceBaseIdNeighboursGetWithHttpInfo(id, depth);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling CompetenceBaseApi.CompetenceBaseIdNeighboursGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **depth** | **int?** |  | [optional] [default to 10] |

### Return type

[**Neighbour**](Neighbour.md)

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

