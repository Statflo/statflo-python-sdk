# statflo_python_sdk.ContentSharingRecommendApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**content_sharing_recommended_create**](ContentSharingRecommendApi.md#content_sharing_recommended_create) | **POST** /v4/api/content-sharing-recommend | 
[**content_sharing_recommended_delete**](ContentSharingRecommendApi.md#content_sharing_recommended_delete) | **DELETE** /v4/api/content-sharing-recommend/{id} | 
[**content_sharing_recommended_get**](ContentSharingRecommendApi.md#content_sharing_recommended_get) | **GET** /v4/api/content-sharing-recommend/{id} | 
[**content_sharing_recommended_search**](ContentSharingRecommendApi.md#content_sharing_recommended_search) | **GET** /v4/api/content-sharing-recommend | 
[**content_sharing_recommended_update**](ContentSharingRecommendApi.md#content_sharing_recommended_update) | **PUT** /v4/api/content-sharing-recommend/{id} | 


# **content_sharing_recommended_create**
> ContentSharingRecommended content_sharing_recommended_create(content_sharing_recommended_create=content_sharing_recommended_create)

Create a content sharing recommendation.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_recommended import ContentSharingRecommended
from statflo_python_sdk.models.content_sharing_recommended_create import ContentSharingRecommendedCreate
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
    api_instance = statflo_python_sdk.ContentSharingRecommendApi(api_client)
    content_sharing_recommended_create = statflo_python_sdk.ContentSharingRecommendedCreate() # ContentSharingRecommendedCreate |  (optional)

    try:
        api_response = api_instance.content_sharing_recommended_create(content_sharing_recommended_create=content_sharing_recommended_create)
        print("The response of ContentSharingRecommendApi->content_sharing_recommended_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingRecommendApi->content_sharing_recommended_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_sharing_recommended_create** | [**ContentSharingRecommendedCreate**](ContentSharingRecommendedCreate.md)|  | [optional] 

### Return type

[**ContentSharingRecommended**](ContentSharingRecommended.md)

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

# **content_sharing_recommended_delete**
> content_sharing_recommended_delete(id)

Remove a content sharing recommendation.

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
    api_instance = statflo_python_sdk.ContentSharingRecommendApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.content_sharing_recommended_delete(id)
    except Exception as e:
        print("Exception when calling ContentSharingRecommendApi->content_sharing_recommended_delete: %s\n" % e)
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

# **content_sharing_recommended_get**
> ContentSharingRecommended content_sharing_recommended_get(id)

Retrieve a content sharing recommendation.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_recommended import ContentSharingRecommended
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
    api_instance = statflo_python_sdk.ContentSharingRecommendApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.content_sharing_recommended_get(id)
        print("The response of ContentSharingRecommendApi->content_sharing_recommended_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingRecommendApi->content_sharing_recommended_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ContentSharingRecommended**](ContentSharingRecommended.md)

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

# **content_sharing_recommended_search**
> ContentSharingRecommendPaginationResponse content_sharing_recommended_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Get a list of all recommendations

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_recommend_pagination_response import ContentSharingRecommendPaginationResponse
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
    api_instance = statflo_python_sdk.ContentSharingRecommendApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.content_sharing_recommended_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of ContentSharingRecommendApi->content_sharing_recommended_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingRecommendApi->content_sharing_recommended_search: %s\n" % e)
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

[**ContentSharingRecommendPaginationResponse**](ContentSharingRecommendPaginationResponse.md)

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

# **content_sharing_recommended_update**
> ContentSharingRecommended content_sharing_recommended_update(id, content_sharing_recommended_update=content_sharing_recommended_update)

Update a content sharing recommendation.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_recommended import ContentSharingRecommended
from statflo_python_sdk.models.content_sharing_recommended_update import ContentSharingRecommendedUpdate
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
    api_instance = statflo_python_sdk.ContentSharingRecommendApi(api_client)
    id = 'id_example' # str | 
    content_sharing_recommended_update = statflo_python_sdk.ContentSharingRecommendedUpdate() # ContentSharingRecommendedUpdate |  (optional)

    try:
        api_response = api_instance.content_sharing_recommended_update(id, content_sharing_recommended_update=content_sharing_recommended_update)
        print("The response of ContentSharingRecommendApi->content_sharing_recommended_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingRecommendApi->content_sharing_recommended_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **content_sharing_recommended_update** | [**ContentSharingRecommendedUpdate**](ContentSharingRecommendedUpdate.md)|  | [optional] 

### Return type

[**ContentSharingRecommended**](ContentSharingRecommended.md)

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

