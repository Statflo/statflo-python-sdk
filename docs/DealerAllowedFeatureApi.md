# statflo_python_sdk.DealerAllowedFeatureApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dealer_allowed_feature_create**](DealerAllowedFeatureApi.md#dealer_allowed_feature_create) | **POST** /v4/api/dealer-allowed-feature | 
[**dealer_allowed_feature_delete**](DealerAllowedFeatureApi.md#dealer_allowed_feature_delete) | **DELETE** /v4/api/dealer-allowed-feature/{dealer}/{feature} | 
[**dealer_allowed_feature_get**](DealerAllowedFeatureApi.md#dealer_allowed_feature_get) | **GET** /v4/api/dealer-allowed-feature/{dealer}/{feature} | 


# **dealer_allowed_feature_create**
> DealerAllowedFeature dealer_allowed_feature_create(dealer_allowed_feature_create=dealer_allowed_feature_create)

Create a dealer allowed feature.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_allowed_feature import DealerAllowedFeature
from statflo_python_sdk.models.dealer_allowed_feature_create import DealerAllowedFeatureCreate
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): Bearer
configuration = statflo_python_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with statflo_python_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = statflo_python_sdk.DealerAllowedFeatureApi(api_client)
    dealer_allowed_feature_create = statflo_python_sdk.DealerAllowedFeatureCreate() # DealerAllowedFeatureCreate |  (optional)

    try:
        api_response = api_instance.dealer_allowed_feature_create(dealer_allowed_feature_create=dealer_allowed_feature_create)
        print("The response of DealerAllowedFeatureApi->dealer_allowed_feature_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerAllowedFeatureApi->dealer_allowed_feature_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dealer_allowed_feature_create** | [**DealerAllowedFeatureCreate**](DealerAllowedFeatureCreate.md)|  | [optional] 

### Return type

[**DealerAllowedFeature**](DealerAllowedFeature.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dealer_allowed_feature_delete**
> dealer_allowed_feature_delete(dealer, feature)

Remove a dealer allowed feature.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): Bearer
configuration = statflo_python_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with statflo_python_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = statflo_python_sdk.DealerAllowedFeatureApi(api_client)
    dealer = 'dealer_example' # str | 
    feature = 'feature_example' # str | 

    try:
        api_instance.dealer_allowed_feature_delete(dealer, feature)
    except Exception as e:
        print("Exception when calling DealerAllowedFeatureApi->dealer_allowed_feature_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dealer** | **str**|  | 
 **feature** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Success |  -  |
**400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **dealer_allowed_feature_get**
> DealerAllowedFeature dealer_allowed_feature_get(dealer, feature)

Retrieve a dealer allowed feature.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_allowed_feature import DealerAllowedFeature
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): Bearer
configuration = statflo_python_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with statflo_python_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = statflo_python_sdk.DealerAllowedFeatureApi(api_client)
    dealer = 'dealer_example' # str | 
    feature = 'feature_example' # str | 

    try:
        api_response = api_instance.dealer_allowed_feature_get(dealer, feature)
        print("The response of DealerAllowedFeatureApi->dealer_allowed_feature_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerAllowedFeatureApi->dealer_allowed_feature_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dealer** | **str**|  | 
 **feature** | **str**|  | 

### Return type

[**DealerAllowedFeature**](DealerAllowedFeature.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

