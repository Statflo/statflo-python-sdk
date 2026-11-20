# statflo_python_sdk.MessageDeliveryStatusApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**message_delivery_status_create**](MessageDeliveryStatusApi.md#message_delivery_status_create) | **POST** /v4/api/message-delivery-status | 
[**message_delivery_status_delete**](MessageDeliveryStatusApi.md#message_delivery_status_delete) | **DELETE** /v4/api/message-delivery-status/{id} | 
[**message_delivery_status_get**](MessageDeliveryStatusApi.md#message_delivery_status_get) | **GET** /v4/api/message-delivery-status/{id} | 
[**message_delivery_status_search**](MessageDeliveryStatusApi.md#message_delivery_status_search) | **GET** /v4/api/message-delivery-status | 
[**message_delivery_status_update**](MessageDeliveryStatusApi.md#message_delivery_status_update) | **PUT** /v4/api/message-delivery-status/{id} | 


# **message_delivery_status_create**
> MessageDeliveryStatus message_delivery_status_create(message_delivery_status_create=message_delivery_status_create)

Create a message delivery status.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.message_delivery_status import MessageDeliveryStatus
from statflo_python_sdk.models.message_delivery_status_create import MessageDeliveryStatusCreate
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
    api_instance = statflo_python_sdk.MessageDeliveryStatusApi(api_client)
    message_delivery_status_create = statflo_python_sdk.MessageDeliveryStatusCreate() # MessageDeliveryStatusCreate |  (optional)

    try:
        api_response = api_instance.message_delivery_status_create(message_delivery_status_create=message_delivery_status_create)
        print("The response of MessageDeliveryStatusApi->message_delivery_status_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageDeliveryStatusApi->message_delivery_status_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_delivery_status_create** | [**MessageDeliveryStatusCreate**](MessageDeliveryStatusCreate.md)|  | [optional] 

### Return type

[**MessageDeliveryStatus**](MessageDeliveryStatus.md)

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

# **message_delivery_status_delete**
> message_delivery_status_delete(id)

Remove a Message Delivery Status.

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
    api_instance = statflo_python_sdk.MessageDeliveryStatusApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.message_delivery_status_delete(id)
    except Exception as e:
        print("Exception when calling MessageDeliveryStatusApi->message_delivery_status_delete: %s\n" % e)
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

# **message_delivery_status_get**
> MessageDeliveryStatus message_delivery_status_get(id)

Retrieve message delivery status.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.message_delivery_status import MessageDeliveryStatus
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
    api_instance = statflo_python_sdk.MessageDeliveryStatusApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.message_delivery_status_get(id)
        print("The response of MessageDeliveryStatusApi->message_delivery_status_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageDeliveryStatusApi->message_delivery_status_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**MessageDeliveryStatus**](MessageDeliveryStatus.md)

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

# **message_delivery_status_search**
> MessageDeliveryStatusPaginationResponse message_delivery_status_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search message delivery status.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.message_delivery_status_pagination_response import MessageDeliveryStatusPaginationResponse
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
    api_instance = statflo_python_sdk.MessageDeliveryStatusApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.message_delivery_status_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of MessageDeliveryStatusApi->message_delivery_status_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageDeliveryStatusApi->message_delivery_status_search: %s\n" % e)
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

[**MessageDeliveryStatusPaginationResponse**](MessageDeliveryStatusPaginationResponse.md)

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

# **message_delivery_status_update**
> MessageDeliveryStatus message_delivery_status_update(id, message_delivery_status_update=message_delivery_status_update)

Update a message delivery status.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.message_delivery_status import MessageDeliveryStatus
from statflo_python_sdk.models.message_delivery_status_update import MessageDeliveryStatusUpdate
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
    api_instance = statflo_python_sdk.MessageDeliveryStatusApi(api_client)
    id = 'id_example' # str | 
    message_delivery_status_update = statflo_python_sdk.MessageDeliveryStatusUpdate() # MessageDeliveryStatusUpdate |  (optional)

    try:
        api_response = api_instance.message_delivery_status_update(id, message_delivery_status_update=message_delivery_status_update)
        print("The response of MessageDeliveryStatusApi->message_delivery_status_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageDeliveryStatusApi->message_delivery_status_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **message_delivery_status_update** | [**MessageDeliveryStatusUpdate**](MessageDeliveryStatusUpdate.md)|  | [optional] 

### Return type

[**MessageDeliveryStatus**](MessageDeliveryStatus.md)

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

