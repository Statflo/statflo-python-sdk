# statflo_python_sdk.EWCAcceptanceApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ewc_acceptance_create**](EWCAcceptanceApi.md#ewc_acceptance_create) | **POST** /v4/api/ewc-acceptance | 
[**ewc_acceptance_delete**](EWCAcceptanceApi.md#ewc_acceptance_delete) | **DELETE** /v4/api/ewc-acceptance/{id} | 
[**ewc_acceptance_get**](EWCAcceptanceApi.md#ewc_acceptance_get) | **GET** /v4/api/ewc-acceptance/{id} | 
[**ewc_acceptance_search**](EWCAcceptanceApi.md#ewc_acceptance_search) | **GET** /v4/api/ewc-acceptance | 
[**ewc_acceptance_update**](EWCAcceptanceApi.md#ewc_acceptance_update) | **PUT** /v4/api/ewc-acceptance/{id} | 


# **ewc_acceptance_create**
> EwcAcceptance ewc_acceptance_create(ewc_acceptance_create=ewc_acceptance_create)

Create EWC acceptance

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.ewc_acceptance import EwcAcceptance
from statflo_python_sdk.models.ewc_acceptance_create import EwcAcceptanceCreate
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
    api_instance = statflo_python_sdk.EWCAcceptanceApi(api_client)
    ewc_acceptance_create = statflo_python_sdk.EwcAcceptanceCreate() # EwcAcceptanceCreate |  (optional)

    try:
        api_response = api_instance.ewc_acceptance_create(ewc_acceptance_create=ewc_acceptance_create)
        print("The response of EWCAcceptanceApi->ewc_acceptance_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EWCAcceptanceApi->ewc_acceptance_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ewc_acceptance_create** | [**EwcAcceptanceCreate**](EwcAcceptanceCreate.md)|  | [optional] 

### Return type

[**EwcAcceptance**](EwcAcceptance.md)

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

# **ewc_acceptance_delete**
> ewc_acceptance_delete(id)

Remove an EWC acceptance

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
    api_instance = statflo_python_sdk.EWCAcceptanceApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.ewc_acceptance_delete(id)
    except Exception as e:
        print("Exception when calling EWCAcceptanceApi->ewc_acceptance_delete: %s\n" % e)
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

# **ewc_acceptance_get**
> EwcAcceptance ewc_acceptance_get(id)

Retrieve an EWC acceptance

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.ewc_acceptance import EwcAcceptance
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
    api_instance = statflo_python_sdk.EWCAcceptanceApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.ewc_acceptance_get(id)
        print("The response of EWCAcceptanceApi->ewc_acceptance_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EWCAcceptanceApi->ewc_acceptance_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**EwcAcceptance**](EwcAcceptance.md)

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

# **ewc_acceptance_search**
> EwcAcceptancePaginationResponse ewc_acceptance_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search EWC acceptance

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.ewc_acceptance_pagination_response import EwcAcceptancePaginationResponse
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
    api_instance = statflo_python_sdk.EWCAcceptanceApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.ewc_acceptance_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of EWCAcceptanceApi->ewc_acceptance_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EWCAcceptanceApi->ewc_acceptance_search: %s\n" % e)
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

[**EwcAcceptancePaginationResponse**](EwcAcceptancePaginationResponse.md)

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

# **ewc_acceptance_update**
> EwcAcceptance ewc_acceptance_update(id, ewc_acceptance_update=ewc_acceptance_update)

Update an EWC acceptance

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.ewc_acceptance import EwcAcceptance
from statflo_python_sdk.models.ewc_acceptance_update import EwcAcceptanceUpdate
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
    api_instance = statflo_python_sdk.EWCAcceptanceApi(api_client)
    id = 'id_example' # str | 
    ewc_acceptance_update = statflo_python_sdk.EwcAcceptanceUpdate() # EwcAcceptanceUpdate |  (optional)

    try:
        api_response = api_instance.ewc_acceptance_update(id, ewc_acceptance_update=ewc_acceptance_update)
        print("The response of EWCAcceptanceApi->ewc_acceptance_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EWCAcceptanceApi->ewc_acceptance_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **ewc_acceptance_update** | [**EwcAcceptanceUpdate**](EwcAcceptanceUpdate.md)|  | [optional] 

### Return type

[**EwcAcceptance**](EwcAcceptance.md)

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

