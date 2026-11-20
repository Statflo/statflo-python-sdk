# statflo_python_sdk.AppointmentLocationApi

All URIs are relative to *https://app.statflo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**appointment_location_create**](AppointmentLocationApi.md#appointment_location_create) | **POST** /v4/api/appointment-location | 
[**appointment_location_delete**](AppointmentLocationApi.md#appointment_location_delete) | **DELETE** /v4/api/appointment-location/{id} | 
[**appointment_location_get**](AppointmentLocationApi.md#appointment_location_get) | **GET** /v4/api/appointment-location/{id} | 
[**appointment_location_search**](AppointmentLocationApi.md#appointment_location_search) | **GET** /v4/api/appointment-location | 
[**appointment_location_update**](AppointmentLocationApi.md#appointment_location_update) | **PUT** /v4/api/appointment-location/{id} | 


# **appointment_location_create**
> AppointmentLocation appointment_location_create(appointment_location_create=appointment_location_create)

Create an appointment location.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.appointment_location import AppointmentLocation
from statflo_python_sdk.models.appointment_location_create import AppointmentLocationCreate
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
    api_instance = statflo_python_sdk.AppointmentLocationApi(api_client)
    appointment_location_create = statflo_python_sdk.AppointmentLocationCreate() # AppointmentLocationCreate |  (optional)

    try:
        api_response = api_instance.appointment_location_create(appointment_location_create=appointment_location_create)
        print("The response of AppointmentLocationApi->appointment_location_create:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppointmentLocationApi->appointment_location_create: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointment_location_create** | [**AppointmentLocationCreate**](AppointmentLocationCreate.md)|  | [optional] 

### Return type

[**AppointmentLocation**](AppointmentLocation.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **appointment_location_delete**
> appointment_location_delete(id)

Delete an appointment location.

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
    api_instance = statflo_python_sdk.AppointmentLocationApi(api_client)
    id = 'id_example' # str | 

    try:
        api_instance.appointment_location_delete(id)
    except Exception as e:
        print("Exception when calling AppointmentLocationApi->appointment_location_delete: %s\n" % e)
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
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **appointment_location_get**
> AppointmentLocation appointment_location_get(id)

Retrieve an appointment location.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.appointment_location import AppointmentLocation
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
    api_instance = statflo_python_sdk.AppointmentLocationApi(api_client)
    id = 'id_example' # str | 

    try:
        api_response = api_instance.appointment_location_get(id)
        print("The response of AppointmentLocationApi->appointment_location_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppointmentLocationApi->appointment_location_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**AppointmentLocation**](AppointmentLocation.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **appointment_location_search**
> AppointmentLocationPaginationResponse appointment_location_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)

Search appointment locations.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.appointment_location_pagination_response import AppointmentLocationPaginationResponse
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
    api_instance = statflo_python_sdk.AppointmentLocationApi(api_client)
    filter = None # Dict[str, object] |  (optional)
    query = 'query_example' # str |  (optional)
    page = 56 # int |  (optional)
    per_page = 56 # int |  (optional)
    sort = 'sort_example' # str |  (optional)

    try:
        api_response = api_instance.appointment_location_search(filter=filter, query=query, page=page, per_page=per_page, sort=sort)
        print("The response of AppointmentLocationApi->appointment_location_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppointmentLocationApi->appointment_location_search: %s\n" % e)
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

[**AppointmentLocationPaginationResponse**](AppointmentLocationPaginationResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **appointment_location_update**
> AppointmentLocation appointment_location_update(id, appointment_location_update=appointment_location_update)

Update an appointment location.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.appointment_location import AppointmentLocation
from statflo_python_sdk.models.appointment_location_update import AppointmentLocationUpdate
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
    api_instance = statflo_python_sdk.AppointmentLocationApi(api_client)
    id = 'id_example' # str | 
    appointment_location_update = statflo_python_sdk.AppointmentLocationUpdate() # AppointmentLocationUpdate |  (optional)

    try:
        api_response = api_instance.appointment_location_update(id, appointment_location_update=appointment_location_update)
        print("The response of AppointmentLocationApi->appointment_location_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppointmentLocationApi->appointment_location_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **appointment_location_update** | [**AppointmentLocationUpdate**](AppointmentLocationUpdate.md)|  | [optional] 

### Return type

[**AppointmentLocation**](AppointmentLocation.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

