# statflo_python_sdk.RcsAgentApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**rcs_agent_create**](RcsAgentApi.md#rcs_agent_create) | **POST** /v4/api/rcs-agent | 
[**rcs_agent_delete**](RcsAgentApi.md#rcs_agent_delete) | **DELETE** /v4/api/rcs-agent/{id} | 
[**rcs_agent_get**](RcsAgentApi.md#rcs_agent_get) | **GET** /v4/api/rcs-agent/{id} | 
[**rcs_agent_search**](RcsAgentApi.md#rcs_agent_search) | **GET** /v4/api/rcs-agent | 
[**rcs_agent_update**](RcsAgentApi.md#rcs_agent_update) | **PUT** /v4/api/rcs-agent/{id} | 


# **rcs_agent_create**
> RcsAgent rcs_agent_create(rcs_agent_create=rcs_agent_create)

Create an rcs agent.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent import RcsAgent
from statflo_python_sdk.models.rcs_agent_create import RcsAgentCreate
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
    api_instance = statflo_python_sdk.RcsAgentApi(api_client)
    rcs_agent_create = statflo_python_sdk.RcsAgentCreate() # RcsAgentCreate |  (optional)

    try:
        api_response = api_instance.rcs_agent_create(rcs_agent_create=rcs_agent_create)
        print("The response of RcsAgentApi->rcs_agent_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentApi->rcs_agent_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rcs_agent_create** | [**RcsAgentCreate**](RcsAgentCreate.md)|  | [optional] 

### Return type

[**RcsAgent**](RcsAgent.md)

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

# **rcs_agent_delete**
> rcs_agent_delete(id)

Remove an rcs agent.

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
    api_instance = statflo_python_sdk.RcsAgentApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.rcs_agent_delete(id)
    except Exception as e:
        print("Exception when calling RcsAgentApi->rcs_agent_delete: %s\n" % e)
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

# **rcs_agent_get**
> RcsAgent rcs_agent_get(id)

Retrieve an rcs agent.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent import RcsAgent
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
    api_instance = statflo_python_sdk.RcsAgentApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.rcs_agent_get(id)
        print("The response of RcsAgentApi->rcs_agent_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentApi->rcs_agent_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**RcsAgent**](RcsAgent.md)

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

# **rcs_agent_search**
> RcsAgentPaginationResponse rcs_agent_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search rcs agents.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_pagination_response import RcsAgentPaginationResponse
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
    api_instance = statflo_python_sdk.RcsAgentApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.rcs_agent_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of RcsAgentApi->rcs_agent_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentApi->rcs_agent_search: %s\n" % e)
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

[**RcsAgentPaginationResponse**](RcsAgentPaginationResponse.md)

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

# **rcs_agent_update**
> RcsAgent rcs_agent_update(id, rcs_agent_update=rcs_agent_update)

Update an rcs agent.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent import RcsAgent
from statflo_python_sdk.models.rcs_agent_update import RcsAgentUpdate
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
    api_instance = statflo_python_sdk.RcsAgentApi(api_client)
    id = 'id_example' # str | 
    rcs_agent_update = statflo_python_sdk.RcsAgentUpdate() # RcsAgentUpdate |  (optional)

    try:
        api_response = api_instance.rcs_agent_update(id, rcs_agent_update=rcs_agent_update)
        print("The response of RcsAgentApi->rcs_agent_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentApi->rcs_agent_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **rcs_agent_update** | [**RcsAgentUpdate**](RcsAgentUpdate.md)|  | [optional] 

### Return type

[**RcsAgent**](RcsAgent.md)

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

