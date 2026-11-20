# statflo_python_sdk.UserExternalIdApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**user_external_id_create**](UserExternalIdApi.md#user_external_id_create) | **POST** /v4/api/user-external-id | 
[**user_external_id_delete**](UserExternalIdApi.md#user_external_id_delete) | **DELETE** /v4/api/user-external-id/{id} | 
[**user_external_id_get**](UserExternalIdApi.md#user_external_id_get) | **GET** /v4/api/user-external-id/{id} | 
[**user_external_id_search**](UserExternalIdApi.md#user_external_id_search) | **GET** /v4/api/user-external-id | 
[**user_external_id_update**](UserExternalIdApi.md#user_external_id_update) | **PUT** /v4/api/user-external-id/{id} | 


# **user_external_id_create**
> UserExternalId user_external_id_create(user_external_id_create=user_external_id_create)

Create a user external id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.user_external_id import UserExternalId
from statflo_python_sdk.models.user_external_id_create import UserExternalIdCreate
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
    api_instance = statflo_python_sdk.UserExternalIdApi(api_client)
    user_external_id_create = statflo_python_sdk.UserExternalIdCreate() # UserExternalIdCreate |  (optional)

    try:
        api_response = api_instance.user_external_id_create(user_external_id_create=user_external_id_create)
        print("The response of UserExternalIdApi->user_external_id_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserExternalIdApi->user_external_id_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_external_id_create** | [**UserExternalIdCreate**](UserExternalIdCreate.md)|  | [optional] 

### Return type

[**UserExternalId**](UserExternalId.md)

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

# **user_external_id_delete**
> user_external_id_delete(id)

Remove a user external id.

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
    api_instance = statflo_python_sdk.UserExternalIdApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.user_external_id_delete(id)
    except Exception as e:
        print("Exception when calling UserExternalIdApi->user_external_id_delete: %s\n" % e)
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

# **user_external_id_get**
> UserExternalId user_external_id_get(id)

Retrieve a user external id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.user_external_id import UserExternalId
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
    api_instance = statflo_python_sdk.UserExternalIdApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.user_external_id_get(id)
        print("The response of UserExternalIdApi->user_external_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserExternalIdApi->user_external_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**UserExternalId**](UserExternalId.md)

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

# **user_external_id_search**
> UserExternalIdPaginationResponse user_external_id_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search user external ids.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.user_external_id_pagination_response import UserExternalIdPaginationResponse
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
    api_instance = statflo_python_sdk.UserExternalIdApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.user_external_id_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of UserExternalIdApi->user_external_id_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserExternalIdApi->user_external_id_search: %s\n" % e)
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

[**UserExternalIdPaginationResponse**](UserExternalIdPaginationResponse.md)

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

# **user_external_id_update**
> UserExternalId user_external_id_update(id, user_external_id_update=user_external_id_update)

Update a user external id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.user_external_id import UserExternalId
from statflo_python_sdk.models.user_external_id_update import UserExternalIdUpdate
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
    api_instance = statflo_python_sdk.UserExternalIdApi(api_client)
    id = 'id_example' # str | 
    user_external_id_update = statflo_python_sdk.UserExternalIdUpdate() # UserExternalIdUpdate |  (optional)

    try:
        api_response = api_instance.user_external_id_update(id, user_external_id_update=user_external_id_update)
        print("The response of UserExternalIdApi->user_external_id_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserExternalIdApi->user_external_id_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **user_external_id_update** | [**UserExternalIdUpdate**](UserExternalIdUpdate.md)|  | [optional] 

### Return type

[**UserExternalId**](UserExternalId.md)

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

