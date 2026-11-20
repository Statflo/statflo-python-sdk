# statflo_python_sdk.SmsActivityApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sms_activity_create**](SmsActivityApi.md#sms_activity_create) | **POST** /v4/api/sms-activity | 
[**sms_activity_delete**](SmsActivityApi.md#sms_activity_delete) | **DELETE** /v4/api/sms-activity/{id} | 
[**sms_activity_get**](SmsActivityApi.md#sms_activity_get) | **GET** /v4/api/sms-activity/{id} | 
[**sms_activity_search**](SmsActivityApi.md#sms_activity_search) | **GET** /v4/api/sms-activity | 
[**sms_activity_update**](SmsActivityApi.md#sms_activity_update) | **PUT** /v4/api/sms-activity/{id} | 


# **sms_activity_create**
> SmsActivity sms_activity_create(sms_activity_create=sms_activity_create)

Create sms activity

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.sms_activity import SmsActivity
from statflo_python_sdk.models.sms_activity_create import SmsActivityCreate
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
    api_instance = statflo_python_sdk.SmsActivityApi(api_client)
    sms_activity_create = statflo_python_sdk.SmsActivityCreate() # SmsActivityCreate |  (optional)

    try:
        api_response = api_instance.sms_activity_create(sms_activity_create=sms_activity_create)
        print("The response of SmsActivityApi->sms_activity_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsActivityApi->sms_activity_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_activity_create** | [**SmsActivityCreate**](SmsActivityCreate.md)|  | [optional] 

### Return type

[**SmsActivity**](SmsActivity.md)

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

# **sms_activity_delete**
> sms_activity_delete(id)

Remove an sms activity

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
    api_instance = statflo_python_sdk.SmsActivityApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.sms_activity_delete(id)
    except Exception as e:
        print("Exception when calling SmsActivityApi->sms_activity_delete: %s\n" % e)
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

# **sms_activity_get**
> SmsActivity sms_activity_get(id)

Retrieve an sms activity

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.sms_activity import SmsActivity
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
    api_instance = statflo_python_sdk.SmsActivityApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.sms_activity_get(id)
        print("The response of SmsActivityApi->sms_activity_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsActivityApi->sms_activity_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**SmsActivity**](SmsActivity.md)

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

# **sms_activity_search**
> SmsActivityPaginationResponse sms_activity_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search sms activity

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.sms_activity_pagination_response import SmsActivityPaginationResponse
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
    api_instance = statflo_python_sdk.SmsActivityApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.sms_activity_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of SmsActivityApi->sms_activity_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsActivityApi->sms_activity_search: %s\n" % e)
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

[**SmsActivityPaginationResponse**](SmsActivityPaginationResponse.md)

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

# **sms_activity_update**
> SmsActivity sms_activity_update(id, sms_activity_update=sms_activity_update)

Update an sms activity

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.sms_activity import SmsActivity
from statflo_python_sdk.models.sms_activity_update import SmsActivityUpdate
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
    api_instance = statflo_python_sdk.SmsActivityApi(api_client)
    id = 'id_example' # str | 
    sms_activity_update = statflo_python_sdk.SmsActivityUpdate() # SmsActivityUpdate |  (optional)

    try:
        api_response = api_instance.sms_activity_update(id, sms_activity_update=sms_activity_update)
        print("The response of SmsActivityApi->sms_activity_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsActivityApi->sms_activity_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **sms_activity_update** | [**SmsActivityUpdate**](SmsActivityUpdate.md)|  | [optional] 

### Return type

[**SmsActivity**](SmsActivity.md)

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

