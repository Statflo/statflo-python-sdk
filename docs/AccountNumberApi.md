# statflo_python_sdk.AccountNumberApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**account_number_create**](AccountNumberApi.md#account_number_create) | **POST** /v4/api/account-number | 
[**account_number_get**](AccountNumberApi.md#account_number_get) | **GET** /v4/api/account-number/{id} | 
[**account_number_search**](AccountNumberApi.md#account_number_search) | **GET** /v4/api/account-number | 
[**account_number_update**](AccountNumberApi.md#account_number_update) | **PUT** /v4/api/account-number/{id} | 


# **account_number_create**
> AccountNumber account_number_create(account_number_create=account_number_create)

Create a account number.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_number import AccountNumber
from statflo_python_sdk.models.account_number_create import AccountNumberCreate
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
    api_instance = statflo_python_sdk.AccountNumberApi(api_client)
    account_number_create = statflo_python_sdk.AccountNumberCreate() # AccountNumberCreate |  (optional)

    try:
        api_response = api_instance.account_number_create(account_number_create=account_number_create)
        print("The response of AccountNumberApi->account_number_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountNumberApi->account_number_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_number_create** | [**AccountNumberCreate**](AccountNumberCreate.md)|  | [optional] 

### Return type

[**AccountNumber**](AccountNumber.md)

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

# **account_number_get**
> AccountNumber account_number_get(id)

Retrieve a message template.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_number import AccountNumber
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
    api_instance = statflo_python_sdk.AccountNumberApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.account_number_get(id)
        print("The response of AccountNumberApi->account_number_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountNumberApi->account_number_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**AccountNumber**](AccountNumber.md)

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

# **account_number_search**
> AccountNumberPaginationResponse account_number_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search Account Number.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_number_pagination_response import AccountNumberPaginationResponse
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
    api_instance = statflo_python_sdk.AccountNumberApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.account_number_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of AccountNumberApi->account_number_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountNumberApi->account_number_search: %s\n" % e)
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

[**AccountNumberPaginationResponse**](AccountNumberPaginationResponse.md)

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

# **account_number_update**
> AccountNumber account_number_update(id, account_number_update=account_number_update)

Update a account number.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.account_number import AccountNumber
from statflo_python_sdk.models.account_number_update import AccountNumberUpdate
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
    api_instance = statflo_python_sdk.AccountNumberApi(api_client)
    id = 'id_example' # str | 
    account_number_update = statflo_python_sdk.AccountNumberUpdate() # AccountNumberUpdate |  (optional)

    try:
        api_response = api_instance.account_number_update(id, account_number_update=account_number_update)
        print("The response of AccountNumberApi->account_number_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountNumberApi->account_number_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **account_number_update** | [**AccountNumberUpdate**](AccountNumberUpdate.md)|  | [optional] 

### Return type

[**AccountNumber**](AccountNumber.md)

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

