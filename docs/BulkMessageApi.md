# statflo_python_sdk.BulkMessageApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulk_message_create**](BulkMessageApi.md#bulk_message_create) | **POST** /v4/api/bulk-message | 
[**bulk_message_get**](BulkMessageApi.md#bulk_message_get) | **GET** /v4/api/bulk-message/{id} | 
[**bulk_message_search**](BulkMessageApi.md#bulk_message_search) | **GET** /v4/api/bulk-message | 
[**bulk_message_update**](BulkMessageApi.md#bulk_message_update) | **PUT** /v4/api/bulk-message/{id} | 


# **bulk_message_create**
> BulkMessage bulk_message_create(bulk_message_create=bulk_message_create)

Create a Bulk Message.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.bulk_message import BulkMessage
from statflo_python_sdk.models.bulk_message_create import BulkMessageCreate
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
    api_instance = statflo_python_sdk.BulkMessageApi(api_client)
    bulk_message_create = statflo_python_sdk.BulkMessageCreate() # BulkMessageCreate |  (optional)

    try:
        api_response = api_instance.bulk_message_create(bulk_message_create=bulk_message_create)
        print("The response of BulkMessageApi->bulk_message_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BulkMessageApi->bulk_message_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulk_message_create** | [**BulkMessageCreate**](BulkMessageCreate.md)|  | [optional] 

### Return type

[**BulkMessage**](BulkMessage.md)

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

# **bulk_message_get**
> BulkMessage bulk_message_get(id)

Retrieve a Bulk Message.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.bulk_message import BulkMessage
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
    api_instance = statflo_python_sdk.BulkMessageApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.bulk_message_get(id)
        print("The response of BulkMessageApi->bulk_message_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BulkMessageApi->bulk_message_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**BulkMessage**](BulkMessage.md)

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

# **bulk_message_search**
> BulkMessagePaginationResponse bulk_message_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search bulkMessages.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.bulk_message_pagination_response import BulkMessagePaginationResponse
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
    api_instance = statflo_python_sdk.BulkMessageApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.bulk_message_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of BulkMessageApi->bulk_message_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BulkMessageApi->bulk_message_search: %s\n" % e)
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

[**BulkMessagePaginationResponse**](BulkMessagePaginationResponse.md)

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

# **bulk_message_update**
> BulkMessage bulk_message_update(id, bulk_message_update=bulk_message_update)

Update a Bulk Message.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.bulk_message import BulkMessage
from statflo_python_sdk.models.bulk_message_update import BulkMessageUpdate
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
    api_instance = statflo_python_sdk.BulkMessageApi(api_client)
    id = 'id_example' # str | 
    bulk_message_update = statflo_python_sdk.BulkMessageUpdate() # BulkMessageUpdate |  (optional)

    try:
        api_response = api_instance.bulk_message_update(id, bulk_message_update=bulk_message_update)
        print("The response of BulkMessageApi->bulk_message_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BulkMessageApi->bulk_message_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **bulk_message_update** | [**BulkMessageUpdate**](BulkMessageUpdate.md)|  | [optional] 

### Return type

[**BulkMessage**](BulkMessage.md)

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

