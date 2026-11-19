# statflo_python_sdk.WidgetMetadataApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**widget_metadata_create**](WidgetMetadataApi.md#widget_metadata_create) | **POST** /v4/api/widget-metadata | 
[**widget_metadata_delete**](WidgetMetadataApi.md#widget_metadata_delete) | **DELETE** /v4/api/widget-metadata/{id} | 
[**widget_metadata_get**](WidgetMetadataApi.md#widget_metadata_get) | **GET** /v4/api/widget-metadata/{id} | 
[**widget_metadata_search**](WidgetMetadataApi.md#widget_metadata_search) | **GET** /v4/api/widget-metadata | 
[**widget_metadata_update**](WidgetMetadataApi.md#widget_metadata_update) | **PUT** /v4/api/widget-metadata/{id} | 


# **widget_metadata_create**
> WidgetMetadata widget_metadata_create(widget_metadata_create=widget_metadata_create)

Create a widget metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.widget_metadata import WidgetMetadata
from statflo_python_sdk.models.widget_metadata_create import WidgetMetadataCreate
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
    api_instance = statflo_python_sdk.WidgetMetadataApi(api_client)
    widget_metadata_create = statflo_python_sdk.WidgetMetadataCreate() # WidgetMetadataCreate |  (optional)

    try:
        api_response = api_instance.widget_metadata_create(widget_metadata_create=widget_metadata_create)
        print("The response of WidgetMetadataApi->widget_metadata_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetMetadataApi->widget_metadata_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **widget_metadata_create** | [**WidgetMetadataCreate**](WidgetMetadataCreate.md)|  | [optional] 

### Return type

[**WidgetMetadata**](WidgetMetadata.md)

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

# **widget_metadata_delete**
> widget_metadata_delete(id)

Remove a widget metadata.

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
    api_instance = statflo_python_sdk.WidgetMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.widget_metadata_delete(id)
    except Exception as e:
        print("Exception when calling WidgetMetadataApi->widget_metadata_delete: %s\n" % e)
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

# **widget_metadata_get**
> WidgetMetadata widget_metadata_get(id)

Retrieve a widget metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.widget_metadata import WidgetMetadata
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
    api_instance = statflo_python_sdk.WidgetMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.widget_metadata_get(id)
        print("The response of WidgetMetadataApi->widget_metadata_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetMetadataApi->widget_metadata_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**WidgetMetadata**](WidgetMetadata.md)

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

# **widget_metadata_search**
> WidgetMetadataPaginationResponse widget_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search widget metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.widget_metadata_pagination_response import WidgetMetadataPaginationResponse
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
    api_instance = statflo_python_sdk.WidgetMetadataApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.widget_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of WidgetMetadataApi->widget_metadata_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetMetadataApi->widget_metadata_search: %s\n" % e)
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

[**WidgetMetadataPaginationResponse**](WidgetMetadataPaginationResponse.md)

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

# **widget_metadata_update**
> WidgetMetadata widget_metadata_update(id, widget_metadata_update=widget_metadata_update)

Update a widget metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.widget_metadata import WidgetMetadata
from statflo_python_sdk.models.widget_metadata_update import WidgetMetadataUpdate
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
    api_instance = statflo_python_sdk.WidgetMetadataApi(api_client)
    id = 'id_example' # str | 
    widget_metadata_update = statflo_python_sdk.WidgetMetadataUpdate() # WidgetMetadataUpdate |  (optional)

    try:
        api_response = api_instance.widget_metadata_update(id, widget_metadata_update=widget_metadata_update)
        print("The response of WidgetMetadataApi->widget_metadata_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetMetadataApi->widget_metadata_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **widget_metadata_update** | [**WidgetMetadataUpdate**](WidgetMetadataUpdate.md)|  | [optional] 

### Return type

[**WidgetMetadata**](WidgetMetadata.md)

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

