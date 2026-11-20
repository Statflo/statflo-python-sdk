# statflo_python_sdk.LocationExternalIdApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**location_external_id_create**](LocationExternalIdApi.md#location_external_id_create) | **POST** /v4/api/location-external-id | 
[**location_external_id_delete**](LocationExternalIdApi.md#location_external_id_delete) | **DELETE** /v4/api/location-external-id/{id} | 
[**location_external_id_get**](LocationExternalIdApi.md#location_external_id_get) | **GET** /v4/api/location-external-id/{id} | 
[**location_external_id_search**](LocationExternalIdApi.md#location_external_id_search) | **GET** /v4/api/location-external-id | 
[**location_external_id_update**](LocationExternalIdApi.md#location_external_id_update) | **PUT** /v4/api/location-external-id/{id} | 


# **location_external_id_create**
> LocationExternalId location_external_id_create(location_external_id_create=location_external_id_create)

Create a location external id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_external_id import LocationExternalId
from statflo_python_sdk.models.location_external_id_create import LocationExternalIdCreate
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
    api_instance = statflo_python_sdk.LocationExternalIdApi(api_client)
    location_external_id_create = statflo_python_sdk.LocationExternalIdCreate() # LocationExternalIdCreate |  (optional)

    try:
        api_response = api_instance.location_external_id_create(location_external_id_create=location_external_id_create)
        print("The response of LocationExternalIdApi->location_external_id_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationExternalIdApi->location_external_id_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location_external_id_create** | [**LocationExternalIdCreate**](LocationExternalIdCreate.md)|  | [optional] 

### Return type

[**LocationExternalId**](LocationExternalId.md)

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

# **location_external_id_delete**
> location_external_id_delete(id)

Remove a location external id.

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
    api_instance = statflo_python_sdk.LocationExternalIdApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.location_external_id_delete(id)
    except Exception as e:
        print("Exception when calling LocationExternalIdApi->location_external_id_delete: %s\n" % e)
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

# **location_external_id_get**
> LocationExternalId location_external_id_get(id)

Retrieve a location external id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_external_id import LocationExternalId
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
    api_instance = statflo_python_sdk.LocationExternalIdApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.location_external_id_get(id)
        print("The response of LocationExternalIdApi->location_external_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationExternalIdApi->location_external_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**LocationExternalId**](LocationExternalId.md)

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

# **location_external_id_search**
> LocationExternalIdPaginationResponse location_external_id_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search location external ids.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_external_id_pagination_response import LocationExternalIdPaginationResponse
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
    api_instance = statflo_python_sdk.LocationExternalIdApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.location_external_id_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of LocationExternalIdApi->location_external_id_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationExternalIdApi->location_external_id_search: %s\n" % e)
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

[**LocationExternalIdPaginationResponse**](LocationExternalIdPaginationResponse.md)

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

# **location_external_id_update**
> LocationExternalId location_external_id_update(id, location_external_id_update=location_external_id_update)

Update a location external id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.location_external_id import LocationExternalId
from statflo_python_sdk.models.location_external_id_update import LocationExternalIdUpdate
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
    api_instance = statflo_python_sdk.LocationExternalIdApi(api_client)
    id = 'id_example' # str | 
    location_external_id_update = statflo_python_sdk.LocationExternalIdUpdate() # LocationExternalIdUpdate |  (optional)

    try:
        api_response = api_instance.location_external_id_update(id, location_external_id_update=location_external_id_update)
        print("The response of LocationExternalIdApi->location_external_id_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocationExternalIdApi->location_external_id_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **location_external_id_update** | [**LocationExternalIdUpdate**](LocationExternalIdUpdate.md)|  | [optional] 

### Return type

[**LocationExternalId**](LocationExternalId.md)

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

