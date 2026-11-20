# statflo_python_sdk.ContentSharingLinkApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**content_sharing_link_create**](ContentSharingLinkApi.md#content_sharing_link_create) | **POST** /v4/api/content-sharing-link | 
[**content_sharing_link_delete**](ContentSharingLinkApi.md#content_sharing_link_delete) | **DELETE** /v4/api/content-sharing-link/{id} | 
[**content_sharing_link_get**](ContentSharingLinkApi.md#content_sharing_link_get) | **GET** /v4/api/content-sharing-link/{id} | 
[**content_sharing_link_search**](ContentSharingLinkApi.md#content_sharing_link_search) | **GET** /v4/api/content-sharing-link | 
[**content_sharing_link_update**](ContentSharingLinkApi.md#content_sharing_link_update) | **PUT** /v4/api/content-sharing-link/{id} | 


# **content_sharing_link_create**
> ContentSharingLink content_sharing_link_create(content_sharing_link_create=content_sharing_link_create)

Create a content sharing link.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_link import ContentSharingLink
from statflo_python_sdk.models.content_sharing_link_create import ContentSharingLinkCreate
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
    api_instance = statflo_python_sdk.ContentSharingLinkApi(api_client)
    content_sharing_link_create = statflo_python_sdk.ContentSharingLinkCreate() # ContentSharingLinkCreate |  (optional)

    try:
        api_response = api_instance.content_sharing_link_create(content_sharing_link_create=content_sharing_link_create)
        print("The response of ContentSharingLinkApi->content_sharing_link_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingLinkApi->content_sharing_link_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_sharing_link_create** | [**ContentSharingLinkCreate**](ContentSharingLinkCreate.md)|  | [optional] 

### Return type

[**ContentSharingLink**](ContentSharingLink.md)

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

# **content_sharing_link_delete**
> content_sharing_link_delete(id)

Remove a content sharing link.

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
    api_instance = statflo_python_sdk.ContentSharingLinkApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.content_sharing_link_delete(id)
    except Exception as e:
        print("Exception when calling ContentSharingLinkApi->content_sharing_link_delete: %s\n" % e)
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

# **content_sharing_link_get**
> ContentSharingLink content_sharing_link_get(id)

Retrieve a content sharing category.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_link import ContentSharingLink
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
    api_instance = statflo_python_sdk.ContentSharingLinkApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.content_sharing_link_get(id)
        print("The response of ContentSharingLinkApi->content_sharing_link_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingLinkApi->content_sharing_link_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**ContentSharingLink**](ContentSharingLink.md)

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

# **content_sharing_link_search**
> ContentSharingLinkPaginationResponse content_sharing_link_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Get a list of all links

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_link_pagination_response import ContentSharingLinkPaginationResponse
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
    api_instance = statflo_python_sdk.ContentSharingLinkApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.content_sharing_link_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of ContentSharingLinkApi->content_sharing_link_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingLinkApi->content_sharing_link_search: %s\n" % e)
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

[**ContentSharingLinkPaginationResponse**](ContentSharingLinkPaginationResponse.md)

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

# **content_sharing_link_update**
> ContentSharingLink content_sharing_link_update(id, content_sharing_link_update=content_sharing_link_update)

Update a content sharing link.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.content_sharing_link import ContentSharingLink
from statflo_python_sdk.models.content_sharing_link_update import ContentSharingLinkUpdate
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
    api_instance = statflo_python_sdk.ContentSharingLinkApi(api_client)
    id = 'id_example' # str | 
    content_sharing_link_update = statflo_python_sdk.ContentSharingLinkUpdate() # ContentSharingLinkUpdate |  (optional)

    try:
        api_response = api_instance.content_sharing_link_update(id, content_sharing_link_update=content_sharing_link_update)
        print("The response of ContentSharingLinkApi->content_sharing_link_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContentSharingLinkApi->content_sharing_link_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **content_sharing_link_update** | [**ContentSharingLinkUpdate**](ContentSharingLinkUpdate.md)|  | [optional] 

### Return type

[**ContentSharingLink**](ContentSharingLink.md)

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

