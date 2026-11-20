# statflo_python_sdk.BulkRequestApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulk_request**](BulkRequestApi.md#bulk_request) | **POST** /v4/api/bulk | 


# **bulk_request**
> List[object] bulk_request(bulk_sub_request)

Submit multiple requests in bulk.

### Example

* Bearer (JWT) Authentication (Bearer):

```python
import statflo_python_sdk
from statflo_python_sdk.models.bulk_sub_request import BulkSubRequest
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
    api_instance = statflo_python_sdk.BulkRequestApi(api_client)
    bulk_sub_request = [statflo_python_sdk.BulkSubRequest()] # List[BulkSubRequest] | 

    try:
        api_response = api_instance.bulk_request(bulk_sub_request)
        print("The response of BulkRequestApi->bulk_request:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BulkRequestApi->bulk_request: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulk_sub_request** | [**List[BulkSubRequest]**](BulkSubRequest.md)|  | 

### Return type

**List[object]**

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

