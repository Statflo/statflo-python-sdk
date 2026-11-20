# statflo_python_sdk.InStoreActivityApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**in_store_activity_create**](InStoreActivityApi.md#in_store_activity_create) | **POST** /v4/api/in-store-activity | 
[**in_store_activity_delete**](InStoreActivityApi.md#in_store_activity_delete) | **DELETE** /v4/api/in-store-activity/{id} | 
[**in_store_activity_get**](InStoreActivityApi.md#in_store_activity_get) | **GET** /v4/api/in-store-activity/{id} | 
[**in_store_activity_search**](InStoreActivityApi.md#in_store_activity_search) | **GET** /v4/api/in-store-activity | 
[**in_store_activity_update**](InStoreActivityApi.md#in_store_activity_update) | **PUT** /v4/api/in-store-activity/{id} | 


# **in_store_activity_create**
> InStoreActivity in_store_activity_create(in_store_activity_create=in_store_activity_create)

Create an in-store activity.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.in_store_activity import InStoreActivity
from statflo_python_sdk.models.in_store_activity_create import InStoreActivityCreate
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
    api_instance = statflo_python_sdk.InStoreActivityApi(api_client)
    in_store_activity_create = statflo_python_sdk.InStoreActivityCreate() # InStoreActivityCreate |  (optional)

    try:
        api_response = api_instance.in_store_activity_create(in_store_activity_create=in_store_activity_create)
        print("The response of InStoreActivityApi->in_store_activity_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InStoreActivityApi->in_store_activity_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **in_store_activity_create** | [**InStoreActivityCreate**](InStoreActivityCreate.md)|  | [optional] 

### Return type

[**InStoreActivity**](InStoreActivity.md)

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

# **in_store_activity_delete**
> in_store_activity_delete(id)

Remove an in-store activity.

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
    api_instance = statflo_python_sdk.InStoreActivityApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.in_store_activity_delete(id)
    except Exception as e:
        print("Exception when calling InStoreActivityApi->in_store_activity_delete: %s\n" % e)
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

# **in_store_activity_get**
> InStoreActivity in_store_activity_get(id)

Retrieve an in-store activity.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.in_store_activity import InStoreActivity
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
    api_instance = statflo_python_sdk.InStoreActivityApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.in_store_activity_get(id)
        print("The response of InStoreActivityApi->in_store_activity_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InStoreActivityApi->in_store_activity_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**InStoreActivity**](InStoreActivity.md)

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

# **in_store_activity_search**
> InStoreActivityPaginationResponse in_store_activity_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search in-store activities.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.in_store_activity_pagination_response import InStoreActivityPaginationResponse
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
    api_instance = statflo_python_sdk.InStoreActivityApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.in_store_activity_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of InStoreActivityApi->in_store_activity_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InStoreActivityApi->in_store_activity_search: %s\n" % e)
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

[**InStoreActivityPaginationResponse**](InStoreActivityPaginationResponse.md)

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

# **in_store_activity_update**
> InStoreActivity in_store_activity_update(id, in_store_activity_update=in_store_activity_update)

Update an in-store activity.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.in_store_activity import InStoreActivity
from statflo_python_sdk.models.in_store_activity_update import InStoreActivityUpdate
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
    api_instance = statflo_python_sdk.InStoreActivityApi(api_client)
    id = 'id_example' # str | 
    in_store_activity_update = statflo_python_sdk.InStoreActivityUpdate() # InStoreActivityUpdate |  (optional)

    try:
        api_response = api_instance.in_store_activity_update(id, in_store_activity_update=in_store_activity_update)
        print("The response of InStoreActivityApi->in_store_activity_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InStoreActivityApi->in_store_activity_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **in_store_activity_update** | [**InStoreActivityUpdate**](InStoreActivityUpdate.md)|  | [optional] 

### Return type

[**InStoreActivity**](InStoreActivity.md)

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

