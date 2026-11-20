# statflo_python_sdk.LocationFallbackUserApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**location_fallback_user_create**](LocationFallbackUserApi.md#location_fallback_user_create) | **POST** /v4/api/location-fallback-user | 
[**location_fallback_user_delete**](LocationFallbackUserApi.md#location_fallback_user_delete) | **DELETE** /v4/api/location-fallback-user/{id} | 
[**location_fallback_user_get**](LocationFallbackUserApi.md#location_fallback_user_get) | **GET** /v4/api/location-fallback-user/{id} | 
[**location_fallback_user_search**](LocationFallbackUserApi.md#location_fallback_user_search) | **GET** /v4/api/location-fallback-user | 
[**location_fallback_user_update**](LocationFallbackUserApi.md#location_fallback_user_update) | **PUT** /v4/api/location-fallback-user/{id} | 


# **location_fallback_user_create**
> LocationFallbackUser location_fallback_user_create(location_fallback_user_create=location_fallback_user_create)

Create a location fallback user.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_fallback_user import LocationFallbackUser
from statflo_python_sdk.models.location_fallback_user_create import LocationFallbackUserCreate
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
    api_instance = statflo_python_sdk.LocationFallbackUserApi(api_client)
    location_fallback_user_create = statflo_python_sdk.LocationFallbackUserCreate() # LocationFallbackUserCreate |  (optional)

    try:
        api_response = api_instance.location_fallback_user_create(location_fallback_user_create=location_fallback_user_create)
        print("The response of LocationFallbackUserApi->location_fallback_user_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationFallbackUserApi->location_fallback_user_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location_fallback_user_create** | [**LocationFallbackUserCreate**](LocationFallbackUserCreate.md)|  | [optional] 

### Return type

[**LocationFallbackUser**](LocationFallbackUser.md)

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

# **location_fallback_user_delete**
> location_fallback_user_delete(id)

Remove a location fallback user.

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
    api_instance = statflo_python_sdk.LocationFallbackUserApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.location_fallback_user_delete(id)
    except Exception as e:
        print("Exception when calling LocationFallbackUserApi->location_fallback_user_delete: %s\n" % e)
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

# **location_fallback_user_get**
> LocationFallbackUser location_fallback_user_get(id)

Retrieve a location fallback user.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_fallback_user import LocationFallbackUser
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
    api_instance = statflo_python_sdk.LocationFallbackUserApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.location_fallback_user_get(id)
        print("The response of LocationFallbackUserApi->location_fallback_user_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationFallbackUserApi->location_fallback_user_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**LocationFallbackUser**](LocationFallbackUser.md)

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

# **location_fallback_user_search**
> LocationFallbackUserPaginationResponse location_fallback_user_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search location fallback users.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_fallback_user_pagination_response import LocationFallbackUserPaginationResponse
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
    api_instance = statflo_python_sdk.LocationFallbackUserApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.location_fallback_user_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of LocationFallbackUserApi->location_fallback_user_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationFallbackUserApi->location_fallback_user_search: %s\n" % e)
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

[**LocationFallbackUserPaginationResponse**](LocationFallbackUserPaginationResponse.md)

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

# **location_fallback_user_update**
> LocationFallbackUser location_fallback_user_update(id, location_fallback_user_update=location_fallback_user_update)

Update a location fallback user.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_fallback_user import LocationFallbackUser
from statflo_python_sdk.models.location_fallback_user_update import LocationFallbackUserUpdate
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
    api_instance = statflo_python_sdk.LocationFallbackUserApi(api_client)
    id = 'id_example' # str | 
    location_fallback_user_update = statflo_python_sdk.LocationFallbackUserUpdate() # LocationFallbackUserUpdate |  (optional)

    try:
        api_response = api_instance.location_fallback_user_update(id, location_fallback_user_update=location_fallback_user_update)
        print("The response of LocationFallbackUserApi->location_fallback_user_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationFallbackUserApi->location_fallback_user_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **location_fallback_user_update** | [**LocationFallbackUserUpdate**](LocationFallbackUserUpdate.md)|  | [optional] 

### Return type

[**LocationFallbackUser**](LocationFallbackUser.md)

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

