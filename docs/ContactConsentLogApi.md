# statflo_python_sdk.ContactConsentLogApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**contact_consent_log_create**](ContactConsentLogApi.md#contact_consent_log_create) | **POST** /v4/api/contact-consent-log | 
[**contact_consent_log_delete**](ContactConsentLogApi.md#contact_consent_log_delete) | **DELETE** /v4/api/contact-consent-log/{id} | 
[**contact_consent_log_get**](ContactConsentLogApi.md#contact_consent_log_get) | **GET** /v4/api/contact-consent-log/{id} | 
[**contact_consent_log_search**](ContactConsentLogApi.md#contact_consent_log_search) | **GET** /v4/api/contact-consent-log | 
[**contact_consent_log_update**](ContactConsentLogApi.md#contact_consent_log_update) | **PUT** /v4/api/contact-consent-log/{id} | 


# **contact_consent_log_create**
> ContactConsentLog contact_consent_log_create(contact_consent_log_create=contact_consent_log_create)

Create contact consent log.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.contact_consent_log import ContactConsentLog
from statflo_python_sdk.models.contact_consent_log_create import ContactConsentLogCreate
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
    api_instance = statflo_python_sdk.ContactConsentLogApi(api_client)
    contact_consent_log_create = statflo_python_sdk.ContactConsentLogCreate() # ContactConsentLogCreate |  (optional)

    try:
        api_response = api_instance.contact_consent_log_create(contact_consent_log_create=contact_consent_log_create)
        print("The response of ContactConsentLogApi->contact_consent_log_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactConsentLogApi->contact_consent_log_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contact_consent_log_create** | [**ContactConsentLogCreate**](ContactConsentLogCreate.md)|  | [optional] 

### Return type

[**ContactConsentLog**](ContactConsentLog.md)

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

# **contact_consent_log_delete**
> contact_consent_log_delete(id)

Remove contact consent log.

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
    api_instance = statflo_python_sdk.ContactConsentLogApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.contact_consent_log_delete(id)
    except Exception as e:
        print("Exception when calling ContactConsentLogApi->contact_consent_log_delete: %s\n" % e)
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

# **contact_consent_log_get**
> ContactConsentLog contact_consent_log_get(id)

Retrieve contact consent log.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.contact_consent_log import ContactConsentLog
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
    api_instance = statflo_python_sdk.ContactConsentLogApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.contact_consent_log_get(id)
        print("The response of ContactConsentLogApi->contact_consent_log_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactConsentLogApi->contact_consent_log_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ContactConsentLog**](ContactConsentLog.md)

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

# **contact_consent_log_search**
> ContactConsentLogPaginationResponse contact_consent_log_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search contact consent logs.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.contact_consent_log_pagination_response import ContactConsentLogPaginationResponse
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
    api_instance = statflo_python_sdk.ContactConsentLogApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.contact_consent_log_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of ContactConsentLogApi->contact_consent_log_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactConsentLogApi->contact_consent_log_search: %s\n" % e)
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

[**ContactConsentLogPaginationResponse**](ContactConsentLogPaginationResponse.md)

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

# **contact_consent_log_update**
> ContactConsentLog contact_consent_log_update(id, contact_consent_log_update=contact_consent_log_update)

Update contact consent log.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.contact_consent_log import ContactConsentLog
from statflo_python_sdk.models.contact_consent_log_update import ContactConsentLogUpdate
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
    api_instance = statflo_python_sdk.ContactConsentLogApi(api_client)
    id = 'id_example' # str | 
    contact_consent_log_update = statflo_python_sdk.ContactConsentLogUpdate() # ContactConsentLogUpdate |  (optional)

    try:
        api_response = api_instance.contact_consent_log_update(id, contact_consent_log_update=contact_consent_log_update)
        print("The response of ContactConsentLogApi->contact_consent_log_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactConsentLogApi->contact_consent_log_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **contact_consent_log_update** | [**ContactConsentLogUpdate**](ContactConsentLogUpdate.md)|  | [optional] 

### Return type

[**ContactConsentLog**](ContactConsentLog.md)

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

