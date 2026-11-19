# statflo_python_sdk.AccountCredentialApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**account_credential_create**](AccountCredentialApi.md#account_credential_create) | **POST** /v4/api/account-credential | 
[**account_credential_get**](AccountCredentialApi.md#account_credential_get) | **GET** /v4/api/account-credential/{id} | 
[**account_credential_search**](AccountCredentialApi.md#account_credential_search) | **GET** /v4/api/account-credential | 
[**account_credential_update**](AccountCredentialApi.md#account_credential_update) | **PUT** /v4/api/account-credential/{id} | 


# **account_credential_create**
> AccountCredential account_credential_create(account_credential_create=account_credential_create)

Create a account credential.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_credential import AccountCredential
from statflo_python_sdk.models.account_credential_create import AccountCredentialCreate
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
    api_instance = statflo_python_sdk.AccountCredentialApi(api_client)
    account_credential_create = statflo_python_sdk.AccountCredentialCreate() # AccountCredentialCreate |  (optional)

    try:
        api_response = api_instance.account_credential_create(account_credential_create=account_credential_create)
        print("The response of AccountCredentialApi->account_credential_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountCredentialApi->account_credential_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_credential_create** | [**AccountCredentialCreate**](AccountCredentialCreate.md)|  | [optional] 

### Return type

[**AccountCredential**](AccountCredential.md)

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

# **account_credential_get**
> AccountCredential account_credential_get(id)

Retrieve a account credential.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_credential import AccountCredential
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
    api_instance = statflo_python_sdk.AccountCredentialApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.account_credential_get(id)
        print("The response of AccountCredentialApi->account_credential_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountCredentialApi->account_credential_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**AccountCredential**](AccountCredential.md)

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

# **account_credential_search**
> AccountCredentialPaginationResponse account_credential_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search account credentials.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_credential_pagination_response import AccountCredentialPaginationResponse
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
    api_instance = statflo_python_sdk.AccountCredentialApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.account_credential_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of AccountCredentialApi->account_credential_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountCredentialApi->account_credential_search: %s\n" % e)
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

[**AccountCredentialPaginationResponse**](AccountCredentialPaginationResponse.md)

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

# **account_credential_update**
> AccountCredential account_credential_update(id, account_credential_update=account_credential_update)

Update a account credential.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_credential import AccountCredential
from statflo_python_sdk.models.account_credential_update import AccountCredentialUpdate
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
    api_instance = statflo_python_sdk.AccountCredentialApi(api_client)
    id = 'id_example' # str | 
    account_credential_update = statflo_python_sdk.AccountCredentialUpdate() # AccountCredentialUpdate |  (optional)

    try:
        api_response = api_instance.account_credential_update(id, account_credential_update=account_credential_update)
        print("The response of AccountCredentialApi->account_credential_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountCredentialApi->account_credential_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **account_credential_update** | [**AccountCredentialUpdate**](AccountCredentialUpdate.md)|  | [optional] 

### Return type

[**AccountCredential**](AccountCredential.md)

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

