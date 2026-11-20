# statflo_python_sdk.RcsAgentBusinessApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**rcs_agent_business_create**](RcsAgentBusinessApi.md#rcs_agent_business_create) | **POST** /v4/api/rcs-agent-business | 
[**rcs_agent_business_delete**](RcsAgentBusinessApi.md#rcs_agent_business_delete) | **DELETE** /v4/api/rcs-agent-business/{id} | 
[**rcs_agent_business_get**](RcsAgentBusinessApi.md#rcs_agent_business_get) | **GET** /v4/api/rcs-agent-business/{id} | 
[**rcs_agent_business_search**](RcsAgentBusinessApi.md#rcs_agent_business_search) | **GET** /v4/api/rcs-agent-business | 
[**rcs_agent_business_update**](RcsAgentBusinessApi.md#rcs_agent_business_update) | **PUT** /v4/api/rcs-agent-business/{id} | 


# **rcs_agent_business_create**
> RcsAgentBusiness rcs_agent_business_create(rcs_agent_business_create=rcs_agent_business_create)

Create an rcs agent business.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_business import RcsAgentBusiness
from statflo_python_sdk.models.rcs_agent_business_create import RcsAgentBusinessCreate
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
    api_instance = statflo_python_sdk.RcsAgentBusinessApi(api_client)
    rcs_agent_business_create = statflo_python_sdk.RcsAgentBusinessCreate() # RcsAgentBusinessCreate |  (optional)

    try:
        api_response = api_instance.rcs_agent_business_create(rcs_agent_business_create=rcs_agent_business_create)
        print("The response of RcsAgentBusinessApi->rcs_agent_business_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentBusinessApi->rcs_agent_business_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rcs_agent_business_create** | [**RcsAgentBusinessCreate**](RcsAgentBusinessCreate.md)|  | [optional] 

### Return type

[**RcsAgentBusiness**](RcsAgentBusiness.md)

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

# **rcs_agent_business_delete**
> rcs_agent_business_delete(id)

Remove an rcs agent business.

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
    api_instance = statflo_python_sdk.RcsAgentBusinessApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.rcs_agent_business_delete(id)
    except Exception as e:
        print("Exception when calling RcsAgentBusinessApi->rcs_agent_business_delete: %s\n" % e)
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

# **rcs_agent_business_get**
> RcsAgentBusiness rcs_agent_business_get(id)

Retrieve an rcs agent business.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_business import RcsAgentBusiness
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
    api_instance = statflo_python_sdk.RcsAgentBusinessApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.rcs_agent_business_get(id)
        print("The response of RcsAgentBusinessApi->rcs_agent_business_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentBusinessApi->rcs_agent_business_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**RcsAgentBusiness**](RcsAgentBusiness.md)

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

# **rcs_agent_business_search**
> RcsAgentBusinessPaginationResponse rcs_agent_business_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search rcs agent businesses.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_business_pagination_response import RcsAgentBusinessPaginationResponse
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
    api_instance = statflo_python_sdk.RcsAgentBusinessApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.rcs_agent_business_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of RcsAgentBusinessApi->rcs_agent_business_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentBusinessApi->rcs_agent_business_search: %s\n" % e)
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

[**RcsAgentBusinessPaginationResponse**](RcsAgentBusinessPaginationResponse.md)

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

# **rcs_agent_business_update**
> RcsAgentBusiness rcs_agent_business_update(id, rcs_agent_business_update=rcs_agent_business_update)

Update an rcs agent business.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_business import RcsAgentBusiness
from statflo_python_sdk.models.rcs_agent_business_update import RcsAgentBusinessUpdate
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
    api_instance = statflo_python_sdk.RcsAgentBusinessApi(api_client)
    id = 'id_example' # str | 
    rcs_agent_business_update = statflo_python_sdk.RcsAgentBusinessUpdate() # RcsAgentBusinessUpdate |  (optional)

    try:
        api_response = api_instance.rcs_agent_business_update(id, rcs_agent_business_update=rcs_agent_business_update)
        print("The response of RcsAgentBusinessApi->rcs_agent_business_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentBusinessApi->rcs_agent_business_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **rcs_agent_business_update** | [**RcsAgentBusinessUpdate**](RcsAgentBusinessUpdate.md)|  | [optional] 

### Return type

[**RcsAgentBusiness**](RcsAgentBusiness.md)

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

