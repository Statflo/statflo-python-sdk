# statflo_python_sdk.RcsAgentUseCaseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**rcs_agent_use_case_create**](RcsAgentUseCaseApi.md#rcs_agent_use_case_create) | **POST** /v4/api/rcs-agent-use-case | 
[**rcs_agent_use_case_delete**](RcsAgentUseCaseApi.md#rcs_agent_use_case_delete) | **DELETE** /v4/api/rcs-agent-use-case/{id} | 
[**rcs_agent_use_case_get**](RcsAgentUseCaseApi.md#rcs_agent_use_case_get) | **GET** /v4/api/rcs-agent-use-case/{id} | 
[**rcs_agent_use_case_search**](RcsAgentUseCaseApi.md#rcs_agent_use_case_search) | **GET** /v4/api/rcs-agent-use-case | 
[**rcs_agent_use_case_update**](RcsAgentUseCaseApi.md#rcs_agent_use_case_update) | **PUT** /v4/api/rcs-agent-use-case/{id} | 


# **rcs_agent_use_case_create**
> RcsAgentUseCase rcs_agent_use_case_create(rcs_agent_use_case_create=rcs_agent_use_case_create)

Create an rcs agent use case.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_use_case import RcsAgentUseCase
from statflo_python_sdk.models.rcs_agent_use_case_create import RcsAgentUseCaseCreate
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
    api_instance = statflo_python_sdk.RcsAgentUseCaseApi(api_client)
    rcs_agent_use_case_create = statflo_python_sdk.RcsAgentUseCaseCreate() # RcsAgentUseCaseCreate |  (optional)

    try:
        api_response = api_instance.rcs_agent_use_case_create(rcs_agent_use_case_create=rcs_agent_use_case_create)
        print("The response of RcsAgentUseCaseApi->rcs_agent_use_case_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentUseCaseApi->rcs_agent_use_case_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rcs_agent_use_case_create** | [**RcsAgentUseCaseCreate**](RcsAgentUseCaseCreate.md)|  | [optional] 

### Return type

[**RcsAgentUseCase**](RcsAgentUseCase.md)

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

# **rcs_agent_use_case_delete**
> rcs_agent_use_case_delete(id)

Remove an rcs agent use case.

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
    api_instance = statflo_python_sdk.RcsAgentUseCaseApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.rcs_agent_use_case_delete(id)
    except Exception as e:
        print("Exception when calling RcsAgentUseCaseApi->rcs_agent_use_case_delete: %s\n" % e)
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

# **rcs_agent_use_case_get**
> RcsAgentUseCase rcs_agent_use_case_get(id)

Retrieve an rcs agent use case.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_use_case import RcsAgentUseCase
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
    api_instance = statflo_python_sdk.RcsAgentUseCaseApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.rcs_agent_use_case_get(id)
        print("The response of RcsAgentUseCaseApi->rcs_agent_use_case_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentUseCaseApi->rcs_agent_use_case_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**RcsAgentUseCase**](RcsAgentUseCase.md)

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

# **rcs_agent_use_case_search**
> RcsAgentUseCasePaginationResponse rcs_agent_use_case_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search rcs agent use cases.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_use_case_pagination_response import RcsAgentUseCasePaginationResponse
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
    api_instance = statflo_python_sdk.RcsAgentUseCaseApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.rcs_agent_use_case_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of RcsAgentUseCaseApi->rcs_agent_use_case_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentUseCaseApi->rcs_agent_use_case_search: %s\n" % e)
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

[**RcsAgentUseCasePaginationResponse**](RcsAgentUseCasePaginationResponse.md)

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

# **rcs_agent_use_case_update**
> RcsAgentUseCase rcs_agent_use_case_update(id, rcs_agent_use_case_update=rcs_agent_use_case_update)

Update an rcs agent use case.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.rcs_agent_use_case import RcsAgentUseCase
from statflo_python_sdk.models.rcs_agent_use_case_update import RcsAgentUseCaseUpdate
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
    api_instance = statflo_python_sdk.RcsAgentUseCaseApi(api_client)
    id = 'id_example' # str | 
    rcs_agent_use_case_update = statflo_python_sdk.RcsAgentUseCaseUpdate() # RcsAgentUseCaseUpdate |  (optional)

    try:
        api_response = api_instance.rcs_agent_use_case_update(id, rcs_agent_use_case_update=rcs_agent_use_case_update)
        print("The response of RcsAgentUseCaseApi->rcs_agent_use_case_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RcsAgentUseCaseApi->rcs_agent_use_case_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **rcs_agent_use_case_update** | [**RcsAgentUseCaseUpdate**](RcsAgentUseCaseUpdate.md)|  | [optional] 

### Return type

[**RcsAgentUseCase**](RcsAgentUseCase.md)

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

