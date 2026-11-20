# statflo_python_sdk.DealerExternalIdApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dealer_external_id_create**](DealerExternalIdApi.md#dealer_external_id_create) | **POST** /v4/api/dealer-external-id | 
[**dealer_external_id_delete**](DealerExternalIdApi.md#dealer_external_id_delete) | **DELETE** /v4/api/dealer-external-id/{id} | 
[**dealer_external_id_get**](DealerExternalIdApi.md#dealer_external_id_get) | **GET** /v4/api/dealer-external-id/{id} | 
[**dealer_external_id_search**](DealerExternalIdApi.md#dealer_external_id_search) | **GET** /v4/api/dealer-external-id | 
[**dealer_external_id_update**](DealerExternalIdApi.md#dealer_external_id_update) | **PUT** /v4/api/dealer-external-id/{id} | 


# **dealer_external_id_create**
> DealerExternalId dealer_external_id_create(dealer_external_id_create=dealer_external_id_create)

Create a Dealer External id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_external_id import DealerExternalId
from statflo_python_sdk.models.dealer_external_id_create import DealerExternalIdCreate
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
    api_instance = statflo_python_sdk.DealerExternalIdApi(api_client)
    dealer_external_id_create = statflo_python_sdk.DealerExternalIdCreate() # DealerExternalIdCreate |  (optional)

    try:
        api_response = api_instance.dealer_external_id_create(dealer_external_id_create=dealer_external_id_create)
        print("The response of DealerExternalIdApi->dealer_external_id_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerExternalIdApi->dealer_external_id_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dealer_external_id_create** | [**DealerExternalIdCreate**](DealerExternalIdCreate.md)|  | [optional] 

### Return type

[**DealerExternalId**](DealerExternalId.md)

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

# **dealer_external_id_delete**
> dealer_external_id_delete(id)

Remove a Dealer External id.

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
    api_instance = statflo_python_sdk.DealerExternalIdApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.dealer_external_id_delete(id)
    except Exception as e:
        print("Exception when calling DealerExternalIdApi->dealer_external_id_delete: %s\n" % e)
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

# **dealer_external_id_get**
> DealerExternalId dealer_external_id_get(id)

Retrieve a Dealer External id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_external_id import DealerExternalId
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
    api_instance = statflo_python_sdk.DealerExternalIdApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.dealer_external_id_get(id)
        print("The response of DealerExternalIdApi->dealer_external_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerExternalIdApi->dealer_external_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**DealerExternalId**](DealerExternalId.md)

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

# **dealer_external_id_search**
> DealerExternalIdPaginationResponse dealer_external_id_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search Dealer External ids.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_external_id_pagination_response import DealerExternalIdPaginationResponse
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
    api_instance = statflo_python_sdk.DealerExternalIdApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.dealer_external_id_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of DealerExternalIdApi->dealer_external_id_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerExternalIdApi->dealer_external_id_search: %s\n" % e)
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

[**DealerExternalIdPaginationResponse**](DealerExternalIdPaginationResponse.md)

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

# **dealer_external_id_update**
> DealerExternalId dealer_external_id_update(id, dealer_external_id_update=dealer_external_id_update)

Update a Dealer External id.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_external_id import DealerExternalId
from statflo_python_sdk.models.dealer_external_id_update import DealerExternalIdUpdate
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
    api_instance = statflo_python_sdk.DealerExternalIdApi(api_client)
    id = 'id_example' # str | 
    dealer_external_id_update = statflo_python_sdk.DealerExternalIdUpdate() # DealerExternalIdUpdate |  (optional)

    try:
        api_response = api_instance.dealer_external_id_update(id, dealer_external_id_update=dealer_external_id_update)
        print("The response of DealerExternalIdApi->dealer_external_id_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerExternalIdApi->dealer_external_id_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **dealer_external_id_update** | [**DealerExternalIdUpdate**](DealerExternalIdUpdate.md)|  | [optional] 

### Return type

[**DealerExternalId**](DealerExternalId.md)

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

