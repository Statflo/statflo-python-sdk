# statflo_python_sdk.TaskApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**task_create**](TaskApi.md#task_create) | **POST** /v4/api/task | 
[**task_delete**](TaskApi.md#task_delete) | **DELETE** /v4/api/task/{id} | 
[**task_get**](TaskApi.md#task_get) | **GET** /v4/api/task/{id} | 
[**task_search**](TaskApi.md#task_search) | **GET** /v4/api/task | 
[**task_update**](TaskApi.md#task_update) | **PUT** /v4/api/task/{id} | 


# **task_create**
> Task task_create(task_create=task_create)

Create a task.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.task import Task
from statflo_python_sdk.models.task_create import TaskCreate
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
    api_instance = statflo_python_sdk.TaskApi(api_client)
    task_create = statflo_python_sdk.TaskCreate() # TaskCreate |  (optional)

    try:
        api_response = api_instance.task_create(task_create=task_create)
        print("The response of TaskApi->task_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaskApi->task_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **task_create** | [**TaskCreate**](TaskCreate.md)|  | [optional] 

### Return type

[**Task**](Task.md)

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

# **task_delete**
> task_delete(id)

Remove a task.

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
    api_instance = statflo_python_sdk.TaskApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.task_delete(id)
    except Exception as e:
        print("Exception when calling TaskApi->task_delete: %s\n" % e)
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

# **task_get**
> Task task_get(id)

Retrieve a task.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.task import Task
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
    api_instance = statflo_python_sdk.TaskApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.task_get(id)
        print("The response of TaskApi->task_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaskApi->task_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**Task**](Task.md)

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

# **task_search**
> TaskPaginationResponse task_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search tasks.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.task_pagination_response import TaskPaginationResponse
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
    api_instance = statflo_python_sdk.TaskApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.task_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of TaskApi->task_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaskApi->task_search: %s\n" % e)
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

[**TaskPaginationResponse**](TaskPaginationResponse.md)

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

# **task_update**
> Task task_update(id, task_update=task_update)

Update a task.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.task import Task
from statflo_python_sdk.models.task_update import TaskUpdate
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
    api_instance = statflo_python_sdk.TaskApi(api_client)
    id = 'id_example' # str | 
    task_update = statflo_python_sdk.TaskUpdate() # TaskUpdate |  (optional)

    try:
        api_response = api_instance.task_update(id, task_update=task_update)
        print("The response of TaskApi->task_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TaskApi->task_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **task_update** | [**TaskUpdate**](TaskUpdate.md)|  | [optional] 

### Return type

[**Task**](Task.md)

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

