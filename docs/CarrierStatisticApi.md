# statflo_python_sdk.CarrierStatisticApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**carrier_statistic_create**](CarrierStatisticApi.md#carrier_statistic_create) | **POST** /v4/api/carrier-statistic | 
[**carrier_statistic_delete**](CarrierStatisticApi.md#carrier_statistic_delete) | **DELETE** /v4/api/carrier-statistic/{id} | 
[**carrier_statistic_get**](CarrierStatisticApi.md#carrier_statistic_get) | **GET** /v4/api/carrier-statistic/{id} | 
[**carrier_statistic_search**](CarrierStatisticApi.md#carrier_statistic_search) | **GET** /v4/api/carrier-statistic | 
[**carrier_statistic_update**](CarrierStatisticApi.md#carrier_statistic_update) | **PUT** /v4/api/carrier-statistic/{id} | 


# **carrier_statistic_create**
> CarrierStatistic carrier_statistic_create(carrier_statistic_create=carrier_statistic_create)

Create carrier statistic.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.carrier_statistic import CarrierStatistic
from statflo_python_sdk.models.carrier_statistic_create import CarrierStatisticCreate
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.statflo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "https://app.statflo.com"
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
    api_instance = statflo_python_sdk.CarrierStatisticApi(api_client)
    carrier_statistic_create = statflo_python_sdk.CarrierStatisticCreate() # CarrierStatisticCreate |  (optional)

    try:
        api_response = api_instance.carrier_statistic_create(carrier_statistic_create=carrier_statistic_create)
        print("The response of CarrierStatisticApi->carrier_statistic_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarrierStatisticApi->carrier_statistic_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **carrier_statistic_create** | [**CarrierStatisticCreate**](CarrierStatisticCreate.md)|  | [optional] 

### Return type

[**CarrierStatistic**](CarrierStatistic.md)

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

# **carrier_statistic_delete**
> carrier_statistic_delete(id)

Remove carrier statistic.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.statflo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "https://app.statflo.com"
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
    api_instance = statflo_python_sdk.CarrierStatisticApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.carrier_statistic_delete(id)
    except Exception as e:
        print("Exception when calling CarrierStatisticApi->carrier_statistic_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

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

# **carrier_statistic_get**
> CarrierStatistic carrier_statistic_get(id)

Retrieve carrier statistic.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.carrier_statistic import CarrierStatistic
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.statflo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "https://app.statflo.com"
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
    api_instance = statflo_python_sdk.CarrierStatisticApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.carrier_statistic_get(id)
        print("The response of CarrierStatisticApi->carrier_statistic_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarrierStatisticApi->carrier_statistic_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**CarrierStatistic**](CarrierStatistic.md)

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

# **carrier_statistic_search**
> CarrierStatisticPaginationResponse carrier_statistic_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search carrier statistic.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.carrier_statistic_pagination_response import CarrierStatisticPaginationResponse
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.statflo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "https://app.statflo.com"
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
    api_instance = statflo_python_sdk.CarrierStatisticApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.carrier_statistic_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of CarrierStatisticApi->carrier_statistic_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarrierStatisticApi->carrier_statistic_search: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | [**Dict[str, object]**](object.md)|  | [optional] 
 **query** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 
 **per_page** | **int**|  | [optional] 
 **sort** | **str**|  | [optional] 

### Return type

[**CarrierStatisticPaginationResponse**](CarrierStatisticPaginationResponse.md)

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

# **carrier_statistic_update**
> CarrierStatistic carrier_statistic_update(id, carrier_statistic_update=carrier_statistic_update)

Update carrier statistic.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.carrier_statistic import CarrierStatistic
from statflo_python_sdk.models.carrier_statistic_update import CarrierStatisticUpdate
from statflo_python_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.statflo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = statflo_python_sdk.Configuration(
    host = "https://app.statflo.com"
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
    api_instance = statflo_python_sdk.CarrierStatisticApi(api_client)
    id = 'id_example' # str | 
    carrier_statistic_update = statflo_python_sdk.CarrierStatisticUpdate() # CarrierStatisticUpdate |  (optional)

    try:
        api_response = api_instance.carrier_statistic_update(id, carrier_statistic_update=carrier_statistic_update)
        print("The response of CarrierStatisticApi->carrier_statistic_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarrierStatisticApi->carrier_statistic_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **carrier_statistic_update** | [**CarrierStatisticUpdate**](CarrierStatisticUpdate.md)|  | [optional] 

### Return type

[**CarrierStatistic**](CarrierStatistic.md)

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

