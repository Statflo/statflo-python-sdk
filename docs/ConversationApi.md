# statflo_python_sdk.ConversationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**conversation_create**](ConversationApi.md#conversation_create) | **POST** /v4/api/conversation | 
[**conversation_get**](ConversationApi.md#conversation_get) | **GET** /v4/api/conversation/{id} | 
[**conversation_search**](ConversationApi.md#conversation_search) | **GET** /v4/api/conversation | 
[**conversation_update**](ConversationApi.md#conversation_update) | **PUT** /v4/api/conversation/{id} | 


# **conversation_create**
> Conversation conversation_create(conversation_create=conversation_create)

Create a conversation.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.conversation import Conversation
from statflo_python_sdk.models.conversation_create import ConversationCreate
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
    api_instance = statflo_python_sdk.ConversationApi(api_client)
    conversation_create = statflo_python_sdk.ConversationCreate() # ConversationCreate |  (optional)

    try:
        api_response = api_instance.conversation_create(conversation_create=conversation_create)
        print("The response of ConversationApi->conversation_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConversationApi->conversation_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversation_create** | [**ConversationCreate**](ConversationCreate.md)|  | [optional] 

### Return type

[**Conversation**](Conversation.md)

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

# **conversation_get**
> Conversation conversation_get(id)

Retrieve a conversation.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.conversation import Conversation
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
    api_instance = statflo_python_sdk.ConversationApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.conversation_get(id)
        print("The response of ConversationApi->conversation_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConversationApi->conversation_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**Conversation**](Conversation.md)

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

# **conversation_search**
> ConversationPaginationResponse conversation_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search conversations.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.conversation_pagination_response import ConversationPaginationResponse
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
    api_instance = statflo_python_sdk.ConversationApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.conversation_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of ConversationApi->conversation_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConversationApi->conversation_search: %s\n" % e)
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

[**ConversationPaginationResponse**](ConversationPaginationResponse.md)

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

# **conversation_update**
> Conversation conversation_update(id, conversation_update=conversation_update)

Update a conversation.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.conversation import Conversation
from statflo_python_sdk.models.conversation_update import ConversationUpdate
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
    api_instance = statflo_python_sdk.ConversationApi(api_client)
    id = 'id_example' # str | 
    conversation_update = statflo_python_sdk.ConversationUpdate() # ConversationUpdate |  (optional)

    try:
        api_response = api_instance.conversation_update(id, conversation_update=conversation_update)
        print("The response of ConversationApi->conversation_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConversationApi->conversation_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **conversation_update** | [**ConversationUpdate**](ConversationUpdate.md)|  | [optional] 

### Return type

[**Conversation**](Conversation.md)

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

