# statflo_python_sdk.ContentSharingCategoryApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**content_sharing_category_create**](ContentSharingCategoryApi.md#content_sharing_category_create) | **POST** /v4/api/content-sharing-category | 
[**content_sharing_category_delete**](ContentSharingCategoryApi.md#content_sharing_category_delete) | **DELETE** /v4/api/content-sharing-category/{id} | 
[**content_sharing_category_get**](ContentSharingCategoryApi.md#content_sharing_category_get) | **GET** /v4/api/content-sharing-category/{id} | 
[**content_sharing_category_search**](ContentSharingCategoryApi.md#content_sharing_category_search) | **GET** /v4/api/content-sharing-category | 
[**content_sharing_category_update**](ContentSharingCategoryApi.md#content_sharing_category_update) | **PUT** /v4/api/content-sharing-category/{id} | 


# **content_sharing_category_create**
> ContentSharingCategory content_sharing_category_create(content_sharing_category_create=content_sharing_category_create)

Create a content sharing category.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_category import ContentSharingCategory
from statflo_python_sdk.models.content_sharing_category_create import ContentSharingCategoryCreate
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
    api_instance = statflo_python_sdk.ContentSharingCategoryApi(api_client)
    content_sharing_category_create = statflo_python_sdk.ContentSharingCategoryCreate() # ContentSharingCategoryCreate |  (optional)

    try:
        api_response = api_instance.content_sharing_category_create(content_sharing_category_create=content_sharing_category_create)
        print("The response of ContentSharingCategoryApi->content_sharing_category_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingCategoryApi->content_sharing_category_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_sharing_category_create** | [**ContentSharingCategoryCreate**](ContentSharingCategoryCreate.md)|  | [optional] 

### Return type

[**ContentSharingCategory**](ContentSharingCategory.md)

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

# **content_sharing_category_delete**
> content_sharing_category_delete(id)

Remove a content sharing category.

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
    api_instance = statflo_python_sdk.ContentSharingCategoryApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.content_sharing_category_delete(id)
    except Exception as e:
        print("Exception when calling ContentSharingCategoryApi->content_sharing_category_delete: %s\n" % e)
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

# **content_sharing_category_get**
> ContentSharingCategory content_sharing_category_get(id)

Retrieve a content sharing category.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_category import ContentSharingCategory
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
    api_instance = statflo_python_sdk.ContentSharingCategoryApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.content_sharing_category_get(id)
        print("The response of ContentSharingCategoryApi->content_sharing_category_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingCategoryApi->content_sharing_category_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ContentSharingCategory**](ContentSharingCategory.md)

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

# **content_sharing_category_search**
> ContentSharingCategoryPaginationResponse content_sharing_category_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search content sharing categories

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_category_pagination_response import ContentSharingCategoryPaginationResponse
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
    api_instance = statflo_python_sdk.ContentSharingCategoryApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.content_sharing_category_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of ContentSharingCategoryApi->content_sharing_category_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingCategoryApi->content_sharing_category_search: %s\n" % e)
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

[**ContentSharingCategoryPaginationResponse**](ContentSharingCategoryPaginationResponse.md)

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

# **content_sharing_category_update**
> ContentSharingCategory content_sharing_category_update(id, content_sharing_category_update=content_sharing_category_update)

Update a content sharing category.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_category import ContentSharingCategory
from statflo_python_sdk.models.content_sharing_category_update import ContentSharingCategoryUpdate
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
    api_instance = statflo_python_sdk.ContentSharingCategoryApi(api_client)
    id = 'id_example' # str | 
    content_sharing_category_update = statflo_python_sdk.ContentSharingCategoryUpdate() # ContentSharingCategoryUpdate |  (optional)

    try:
        api_response = api_instance.content_sharing_category_update(id, content_sharing_category_update=content_sharing_category_update)
        print("The response of ContentSharingCategoryApi->content_sharing_category_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingCategoryApi->content_sharing_category_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **content_sharing_category_update** | [**ContentSharingCategoryUpdate**](ContentSharingCategoryUpdate.md)|  | [optional] 

### Return type

[**ContentSharingCategory**](ContentSharingCategory.md)

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

