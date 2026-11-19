# statflo_python_sdk.ExternalDNCApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**external_dnc_create**](ExternalDNCApi.md#external_dnc_create) | **POST** /v4/api/external-dnc | 
[**external_dnc_delete**](ExternalDNCApi.md#external_dnc_delete) | **DELETE** /v4/api/external-dnc/{id} | 
[**external_dnc_get**](ExternalDNCApi.md#external_dnc_get) | **GET** /v4/api/external-dnc/{id} | 
[**external_dnc_search**](ExternalDNCApi.md#external_dnc_search) | **GET** /v4/api/external-dnc | 
[**external_dnc_update**](ExternalDNCApi.md#external_dnc_update) | **PUT** /v4/api/external-dnc/{id} | 


# **external_dnc_create**
> ExternalDnc external_dnc_create(external_dnc_create=external_dnc_create)

Create an external DNC.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.external_dnc import ExternalDnc
from statflo_python_sdk.models.external_dnc_create import ExternalDncCreate
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
    api_instance = statflo_python_sdk.ExternalDNCApi(api_client)
    external_dnc_create = statflo_python_sdk.ExternalDncCreate() # ExternalDncCreate |  (optional)

    try:
        api_response = api_instance.external_dnc_create(external_dnc_create=external_dnc_create)
        print("The response of ExternalDNCApi->external_dnc_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExternalDNCApi->external_dnc_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **external_dnc_create** | [**ExternalDncCreate**](ExternalDncCreate.md)|  | [optional] 

### Return type

[**ExternalDnc**](ExternalDnc.md)

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

# **external_dnc_delete**
> external_dnc_delete(id)

Remove an external DNC entry.

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
    api_instance = statflo_python_sdk.ExternalDNCApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.external_dnc_delete(id)
    except Exception as e:
        print("Exception when calling ExternalDNCApi->external_dnc_delete: %s\n" % e)
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

# **external_dnc_get**
> ExternalDnc external_dnc_get(id)

Retrieve an external DNC.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.external_dnc import ExternalDnc
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
    api_instance = statflo_python_sdk.ExternalDNCApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.external_dnc_get(id)
        print("The response of ExternalDNCApi->external_dnc_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExternalDNCApi->external_dnc_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ExternalDnc**](ExternalDnc.md)

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

# **external_dnc_search**
> ExternalDncPaginationResponse external_dnc_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search external DNC.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.external_dnc_pagination_response import ExternalDncPaginationResponse
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
    api_instance = statflo_python_sdk.ExternalDNCApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.external_dnc_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of ExternalDNCApi->external_dnc_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExternalDNCApi->external_dnc_search: %s\n" % e)
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

[**ExternalDncPaginationResponse**](ExternalDncPaginationResponse.md)

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

# **external_dnc_update**
> ExternalDnc external_dnc_update(id, external_dnc_update=external_dnc_update)

Update an external DNC.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.external_dnc import ExternalDnc
from statflo_python_sdk.models.external_dnc_update import ExternalDncUpdate
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
    api_instance = statflo_python_sdk.ExternalDNCApi(api_client)
    id = 'id_example' # str | 
    external_dnc_update = statflo_python_sdk.ExternalDncUpdate() # ExternalDncUpdate |  (optional)

    try:
        api_response = api_instance.external_dnc_update(id, external_dnc_update=external_dnc_update)
        print("The response of ExternalDNCApi->external_dnc_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExternalDNCApi->external_dnc_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **external_dnc_update** | [**ExternalDncUpdate**](ExternalDncUpdate.md)|  | [optional] 

### Return type

[**ExternalDnc**](ExternalDnc.md)

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

