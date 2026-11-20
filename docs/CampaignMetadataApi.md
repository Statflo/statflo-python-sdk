# statflo_python_sdk.CampaignMetadataApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**campaign_metadata_create**](CampaignMetadataApi.md#campaign_metadata_create) | **POST** /v4/api/campaign-metadata | 
[**campaign_metadata_delete**](CampaignMetadataApi.md#campaign_metadata_delete) | **DELETE** /v4/api/campaign-metadata/{id} | 
[**campaign_metadata_get**](CampaignMetadataApi.md#campaign_metadata_get) | **GET** /v4/api/campaign-metadata/{id} | 
[**campaign_metadata_search**](CampaignMetadataApi.md#campaign_metadata_search) | **GET** /v4/api/campaign-metadata | 
[**campaign_metadata_update**](CampaignMetadataApi.md#campaign_metadata_update) | **PUT** /v4/api/campaign-metadata/{id} | 


# **campaign_metadata_create**
> CampaignMetadata campaign_metadata_create(campaign_metadata_create=campaign_metadata_create)

Create a campaign metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_metadata import CampaignMetadata
from statflo_python_sdk.models.campaign_metadata_create import CampaignMetadataCreate
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
    api_instance = statflo_python_sdk.CampaignMetadataApi(api_client)
    campaign_metadata_create = statflo_python_sdk.CampaignMetadataCreate() # CampaignMetadataCreate |  (optional)

    try:
        api_response = api_instance.campaign_metadata_create(campaign_metadata_create=campaign_metadata_create)
        print("The response of CampaignMetadataApi->campaign_metadata_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignMetadataApi->campaign_metadata_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **campaign_metadata_create** | [**CampaignMetadataCreate**](CampaignMetadataCreate.md)|  | [optional] 

### Return type

[**CampaignMetadata**](CampaignMetadata.md)

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

# **campaign_metadata_delete**
> campaign_metadata_delete(id)

Remove a campaign metadata.

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
    api_instance = statflo_python_sdk.CampaignMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.campaign_metadata_delete(id)
    except Exception as e:
        print("Exception when calling CampaignMetadataApi->campaign_metadata_delete: %s\n" % e)
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

# **campaign_metadata_get**
> CampaignMetadata campaign_metadata_get(id)

Retrieve a campaign metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_metadata import CampaignMetadata
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
    api_instance = statflo_python_sdk.CampaignMetadataApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.campaign_metadata_get(id)
        print("The response of CampaignMetadataApi->campaign_metadata_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignMetadataApi->campaign_metadata_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**CampaignMetadata**](CampaignMetadata.md)

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

# **campaign_metadata_search**
> CampaignMetadataPaginationResponse campaign_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search campaign metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_metadata_pagination_response import CampaignMetadataPaginationResponse
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
    api_instance = statflo_python_sdk.CampaignMetadataApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.campaign_metadata_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of CampaignMetadataApi->campaign_metadata_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignMetadataApi->campaign_metadata_search: %s\n" % e)
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

[**CampaignMetadataPaginationResponse**](CampaignMetadataPaginationResponse.md)

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

# **campaign_metadata_update**
> CampaignMetadata campaign_metadata_update(id, campaign_metadata_update=campaign_metadata_update)

Update a campaign metadata.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.campaign_metadata import CampaignMetadata
from statflo_python_sdk.models.campaign_metadata_update import CampaignMetadataUpdate
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
    api_instance = statflo_python_sdk.CampaignMetadataApi(api_client)
    id = 'id_example' # str | 
    campaign_metadata_update = statflo_python_sdk.CampaignMetadataUpdate() # CampaignMetadataUpdate |  (optional)

    try:
        api_response = api_instance.campaign_metadata_update(id, campaign_metadata_update=campaign_metadata_update)
        print("The response of CampaignMetadataApi->campaign_metadata_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CampaignMetadataApi->campaign_metadata_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **campaign_metadata_update** | [**CampaignMetadataUpdate**](CampaignMetadataUpdate.md)|  | [optional] 

### Return type

[**CampaignMetadata**](CampaignMetadata.md)

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

