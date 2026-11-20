# statflo_python_sdk.CampaignPropertyApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**campaign_property_create**](CampaignPropertyApi.md#campaign_property_create) | **POST** /v4/api/campaign-property | 
[**campaign_property_delete**](CampaignPropertyApi.md#campaign_property_delete) | **DELETE** /v4/api/campaign-property/{id} | 
[**campaign_property_get**](CampaignPropertyApi.md#campaign_property_get) | **GET** /v4/api/campaign-property/{id} | 
[**campaign_property_search**](CampaignPropertyApi.md#campaign_property_search) | **GET** /v4/api/campaign-property | 
[**campaign_property_update**](CampaignPropertyApi.md#campaign_property_update) | **PUT** /v4/api/campaign-property/{id} | 


# **campaign_property_create**
> CampaignProperty campaign_property_create(campaign_property_create=campaign_property_create)

Create a campaign property.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_property import CampaignProperty
from statflo_python_sdk.models.campaign_property_create import CampaignPropertyCreate
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
    api_instance = statflo_python_sdk.CampaignPropertyApi(api_client)
    campaign_property_create = statflo_python_sdk.CampaignPropertyCreate() # CampaignPropertyCreate |  (optional)

    try:
        api_response = api_instance.campaign_property_create(campaign_property_create=campaign_property_create)
        print("The response of CampaignPropertyApi->campaign_property_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignPropertyApi->campaign_property_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **campaign_property_create** | [**CampaignPropertyCreate**](CampaignPropertyCreate.md)|  | [optional] 

### Return type

[**CampaignProperty**](CampaignProperty.md)

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

# **campaign_property_delete**
> campaign_property_delete(id)

Remove a campaign property.

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
    api_instance = statflo_python_sdk.CampaignPropertyApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.campaign_property_delete(id)
    except Exception as e:
        print("Exception when calling CampaignPropertyApi->campaign_property_delete: %s\n" % e)
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

# **campaign_property_get**
> CampaignProperty campaign_property_get(id)

Retrieve a campaign property.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_property import CampaignProperty
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
    api_instance = statflo_python_sdk.CampaignPropertyApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.campaign_property_get(id)
        print("The response of CampaignPropertyApi->campaign_property_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignPropertyApi->campaign_property_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**CampaignProperty**](CampaignProperty.md)

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

# **campaign_property_search**
> CampaignPropertyPaginationResponse campaign_property_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search campaign properties.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_property_pagination_response import CampaignPropertyPaginationResponse
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
    api_instance = statflo_python_sdk.CampaignPropertyApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.campaign_property_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of CampaignPropertyApi->campaign_property_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignPropertyApi->campaign_property_search: %s\n" % e)
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

[**CampaignPropertyPaginationResponse**](CampaignPropertyPaginationResponse.md)

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

# **campaign_property_update**
> CampaignProperty campaign_property_update(id, campaign_property_update=campaign_property_update)

Update a campaign property.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_property import CampaignProperty
from statflo_python_sdk.models.campaign_property_update import CampaignPropertyUpdate
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
    api_instance = statflo_python_sdk.CampaignPropertyApi(api_client)
    id = 'id_example' # str | 
    campaign_property_update = statflo_python_sdk.CampaignPropertyUpdate() # CampaignPropertyUpdate |  (optional)

    try:
        api_response = api_instance.campaign_property_update(id, campaign_property_update=campaign_property_update)
        print("The response of CampaignPropertyApi->campaign_property_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignPropertyApi->campaign_property_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **campaign_property_update** | [**CampaignPropertyUpdate**](CampaignPropertyUpdate.md)|  | [optional] 

### Return type

[**CampaignProperty**](CampaignProperty.md)

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

