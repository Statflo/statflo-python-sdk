# statflo_python_sdk.CampaignActionApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**campaign_action_create**](CampaignActionApi.md#campaign_action_create) | **POST** /v4/api/campaign-action | 
[**campaign_action_delete**](CampaignActionApi.md#campaign_action_delete) | **DELETE** /v4/api/campaign-action/{id} | 
[**campaign_action_get**](CampaignActionApi.md#campaign_action_get) | **GET** /v4/api/campaign-action/{id} | 
[**campaign_action_search**](CampaignActionApi.md#campaign_action_search) | **GET** /v4/api/campaign-action | 
[**campaign_action_update**](CampaignActionApi.md#campaign_action_update) | **PUT** /v4/api/campaign-action/{id} | 


# **campaign_action_create**
> CampaignAction campaign_action_create(campaign_action_create=campaign_action_create)

Create a campaign action.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_action import CampaignAction
from statflo_python_sdk.models.campaign_action_create import CampaignActionCreate
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
    api_instance = statflo_python_sdk.CampaignActionApi(api_client)
    campaign_action_create = statflo_python_sdk.CampaignActionCreate() # CampaignActionCreate |  (optional)

    try:
        api_response = api_instance.campaign_action_create(campaign_action_create=campaign_action_create)
        print("The response of CampaignActionApi->campaign_action_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignActionApi->campaign_action_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **campaign_action_create** | [**CampaignActionCreate**](CampaignActionCreate.md)|  | [optional] 

### Return type

[**CampaignAction**](CampaignAction.md)

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

# **campaign_action_delete**
> campaign_action_delete(id)

Remove a campaign action.

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
    api_instance = statflo_python_sdk.CampaignActionApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.campaign_action_delete(id)
    except Exception as e:
        print("Exception when calling CampaignActionApi->campaign_action_delete: %s\n" % e)
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

# **campaign_action_get**
> CampaignAction campaign_action_get(id)

Retrieve a campaign action.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_action import CampaignAction
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
    api_instance = statflo_python_sdk.CampaignActionApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.campaign_action_get(id)
        print("The response of CampaignActionApi->campaign_action_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignActionApi->campaign_action_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**CampaignAction**](CampaignAction.md)

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

# **campaign_action_search**
> CampaignActionPaginationResponse campaign_action_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search campaign actions.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_action_pagination_response import CampaignActionPaginationResponse
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
    api_instance = statflo_python_sdk.CampaignActionApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.campaign_action_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of CampaignActionApi->campaign_action_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignActionApi->campaign_action_search: %s\n" % e)
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

[**CampaignActionPaginationResponse**](CampaignActionPaginationResponse.md)

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

# **campaign_action_update**
> CampaignAction campaign_action_update(id, campaign_action_update=campaign_action_update)

Update a campaign action.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_action import CampaignAction
from statflo_python_sdk.models.campaign_action_update import CampaignActionUpdate
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
    api_instance = statflo_python_sdk.CampaignActionApi(api_client)
    id = 'id_example' # str | 
    campaign_action_update = statflo_python_sdk.CampaignActionUpdate() # CampaignActionUpdate |  (optional)

    try:
        api_response = api_instance.campaign_action_update(id, campaign_action_update=campaign_action_update)
        print("The response of CampaignActionApi->campaign_action_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignActionApi->campaign_action_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **campaign_action_update** | [**CampaignActionUpdate**](CampaignActionUpdate.md)|  | [optional] 

### Return type

[**CampaignAction**](CampaignAction.md)

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

