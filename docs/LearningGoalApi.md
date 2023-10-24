# CoKoMo.CoKoMoApiClient.Api.LearningGoalApi

All URIs are relative to *https://cokomo.code4you.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**LearningGoalIdDetailsGet**](LearningGoalApi.md#learninggoaliddetailsget) | **GET** /LearningGoal/{id}/details |  |
| [**LearningGoalIdGet**](LearningGoalApi.md#learninggoalidget) | **GET** /LearningGoal/{id} |  |

<a id="learninggoaliddetailsget"></a>
# **LearningGoalIdDetailsGet**
> LearningGoal LearningGoalIdDetailsGet (string id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using CoKoMo.CoKoMoApiClient.Api;
using CoKoMo.CoKoMoApiClient.Client;
using CoKoMo.CoKoMoApiClient.Model;

namespace Example
{
    public class LearningGoalIdDetailsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://cokomo.code4you.com";
            var apiInstance = new LearningGoalApi(config);
            var id = "id_example";  // string | 

            try
            {
                LearningGoal result = apiInstance.LearningGoalIdDetailsGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LearningGoalApi.LearningGoalIdDetailsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LearningGoalIdDetailsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<LearningGoal> response = apiInstance.LearningGoalIdDetailsGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LearningGoalApi.LearningGoalIdDetailsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**LearningGoal**](LearningGoal.md)

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

<a id="learninggoalidget"></a>
# **LearningGoalIdGet**
> LearningGoal LearningGoalIdGet (string id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using CoKoMo.CoKoMoApiClient.Api;
using CoKoMo.CoKoMoApiClient.Client;
using CoKoMo.CoKoMoApiClient.Model;

namespace Example
{
    public class LearningGoalIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://cokomo.code4you.com";
            var apiInstance = new LearningGoalApi(config);
            var id = "id_example";  // string | 

            try
            {
                LearningGoal result = apiInstance.LearningGoalIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LearningGoalApi.LearningGoalIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LearningGoalIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<LearningGoal> response = apiInstance.LearningGoalIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LearningGoalApi.LearningGoalIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**LearningGoal**](LearningGoal.md)

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

