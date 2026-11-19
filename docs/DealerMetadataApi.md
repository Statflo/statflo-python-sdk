# statflo_python_sdk.DealerMetadataApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dealer_metadata_create**](DealerMetadataApi.md#dealer_metadata_create) | **POST** /v4/api/dealer-metadata | 
[**dealer_metadata_delete**](DealerMetadataApi.md#dealer_metadata_delete) | **DELETE** /v4/api/dealer-metadata/{id} | 
[**dealer_metadata_get**](DealerMetadataApi.md#dealer_metadata_get) | **GET** /v4/api/dealer-metadata/{id} | 
[**dealer_metadata_search**](DealerMetadataApi.md#dealer_metadata_search) | **GET** /v4/api/dealer-metadata | 
[**dealer_metadata_update**](DealerMetadataApi.md#dealer_metadata_update) | **PUT** /v4/api/dealer-metadata/{id} | 


# **dealer_metadata_create**
> DealerMetadata dealer_metadata_create(dealer_metadata_create=dealer_metadata_create)

Create a dealer metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_metadata import DealerMetadata
from statflo_python_sdk.models.dealer_metadata_create import DealerMetadataCreate
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
    api_instance = statflo_python_sdk.DealerMetadataApi(api_client)
    dealer_metadata_create = statflo_python_sdk.DealerMetadataCreate() # DealerMetadataCreate |  (optional)

    try:
        api_response = api_instance.dealer_metadata_create(dealer_metadata_create=dealer_metadata_create)
        print("The response of DealerMetadataApi->dealer_metadata_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerMetadataApi->dealer_metadata_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dealer_metadata_create** | [**DealerMetadataCreate**](DealerMetadataCreate.md)|  | [optional] 

### Return type

[**DealerMetadata**](DealerMetadata.md)

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

# **dealer_metadata_delete**
> dealer_metadata_delete(id)

Remove a dealer metadata.

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
    api_instance = statflo_python_sdk.DealerMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.dealer_metadata_delete(id)
    except Exception as e:
        print("Exception when calling DealerMetadataApi->dealer_metadata_delete: %s\n" % e)
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

# **dealer_metadata_get**
> DealerMetadata dealer_metadata_get(id)

Retrieve a dealer metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_metadata import DealerMetadata
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
    api_instance = statflo_python_sdk.DealerMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.dealer_metadata_get(id)
        print("The response of DealerMetadataApi->dealer_metadata_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerMetadataApi->dealer_metadata_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**DealerMetadata**](DealerMetadata.md)

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

# **dealer_metadata_search**
> DealerMetadataPaginationResponse dealer_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search dealer metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_metadata_pagination_response import DealerMetadataPaginationResponse
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
    api_instance = statflo_python_sdk.DealerMetadataApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.dealer_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of DealerMetadataApi->dealer_metadata_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerMetadataApi->dealer_metadata_search: %s\n" % e)
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

[**DealerMetadataPaginationResponse**](DealerMetadataPaginationResponse.md)

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

# **dealer_metadata_update**
> DealerMetadata dealer_metadata_update(id, dealer_metadata_update=dealer_metadata_update)

Update a dealer metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.dealer_metadata import DealerMetadata
from statflo_python_sdk.models.dealer_metadata_update import DealerMetadataUpdate
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
    api_instance = statflo_python_sdk.DealerMetadataApi(api_client)
    id = 'id_example' # str | 
    dealer_metadata_update = statflo_python_sdk.DealerMetadataUpdate() # DealerMetadataUpdate |  (optional)

    try:
        api_response = api_instance.dealer_metadata_update(id, dealer_metadata_update=dealer_metadata_update)
        print("The response of DealerMetadataApi->dealer_metadata_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DealerMetadataApi->dealer_metadata_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **dealer_metadata_update** | [**DealerMetadataUpdate**](DealerMetadataUpdate.md)|  | [optional] 

### Return type

[**DealerMetadata**](DealerMetadata.md)

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

