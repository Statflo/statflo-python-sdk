# statflo_python_sdk.AccountContactMetadataApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**account_contact_metadata_create**](AccountContactMetadataApi.md#account_contact_metadata_create) | **POST** /v4/api/account-contact-metadata | 
[**account_contact_metadata_delete**](AccountContactMetadataApi.md#account_contact_metadata_delete) | **DELETE** /v4/api/account-contact-metadata/{id} | 
[**account_contact_metadata_get**](AccountContactMetadataApi.md#account_contact_metadata_get) | **GET** /v4/api/account-contact-metadata/{id} | 
[**account_contact_metadata_search**](AccountContactMetadataApi.md#account_contact_metadata_search) | **GET** /v4/api/account-contact-metadata | 
[**account_contact_metadata_update**](AccountContactMetadataApi.md#account_contact_metadata_update) | **PUT** /v4/api/account-contact-metadata/{id} | 


# **account_contact_metadata_create**
> AccountContactMetadata account_contact_metadata_create(account_contact_metadata_create=account_contact_metadata_create)

Create a account contact metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_contact_metadata import AccountContactMetadata
from statflo_python_sdk.models.account_contact_metadata_create import AccountContactMetadataCreate
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
    api_instance = statflo_python_sdk.AccountContactMetadataApi(api_client)
    account_contact_metadata_create = statflo_python_sdk.AccountContactMetadataCreate() # AccountContactMetadataCreate |  (optional)

    try:
        api_response = api_instance.account_contact_metadata_create(account_contact_metadata_create=account_contact_metadata_create)
        print("The response of AccountContactMetadataApi->account_contact_metadata_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountContactMetadataApi->account_contact_metadata_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_contact_metadata_create** | [**AccountContactMetadataCreate**](AccountContactMetadataCreate.md)|  | [optional] 

### Return type

[**AccountContactMetadata**](AccountContactMetadata.md)

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

# **account_contact_metadata_delete**
> account_contact_metadata_delete(id)

Remove a account contact metadata.

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
    api_instance = statflo_python_sdk.AccountContactMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.account_contact_metadata_delete(id)
    except Exception as e:
        print("Exception when calling AccountContactMetadataApi->account_contact_metadata_delete: %s\n" % e)
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

# **account_contact_metadata_get**
> AccountContactMetadata account_contact_metadata_get(id)

Retrieve a account contact metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_contact_metadata import AccountContactMetadata
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
    api_instance = statflo_python_sdk.AccountContactMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.account_contact_metadata_get(id)
        print("The response of AccountContactMetadataApi->account_contact_metadata_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountContactMetadataApi->account_contact_metadata_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**AccountContactMetadata**](AccountContactMetadata.md)

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

# **account_contact_metadata_search**
> AccountContactMetadataPaginationResponse account_contact_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search account contact metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_contact_metadata_pagination_response import AccountContactMetadataPaginationResponse
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
    api_instance = statflo_python_sdk.AccountContactMetadataApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.account_contact_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of AccountContactMetadataApi->account_contact_metadata_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountContactMetadataApi->account_contact_metadata_search: %s\n" % e)
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

[**AccountContactMetadataPaginationResponse**](AccountContactMetadataPaginationResponse.md)

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

# **account_contact_metadata_update**
> AccountContactMetadata account_contact_metadata_update(id, account_contact_metadata_update=account_contact_metadata_update)

Update a account contact metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_contact_metadata import AccountContactMetadata
from statflo_python_sdk.models.account_contact_metadata_update import AccountContactMetadataUpdate
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
    api_instance = statflo_python_sdk.AccountContactMetadataApi(api_client)
    id = 'id_example' # str | 
    account_contact_metadata_update = statflo_python_sdk.AccountContactMetadataUpdate() # AccountContactMetadataUpdate |  (optional)

    try:
        api_response = api_instance.account_contact_metadata_update(id, account_contact_metadata_update=account_contact_metadata_update)
        print("The response of AccountContactMetadataApi->account_contact_metadata_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountContactMetadataApi->account_contact_metadata_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **account_contact_metadata_update** | [**AccountContactMetadataUpdate**](AccountContactMetadataUpdate.md)|  | [optional] 

### Return type

[**AccountContactMetadata**](AccountContactMetadata.md)

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

