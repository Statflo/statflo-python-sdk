# VendorMessagePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[VendorMessage]**](VendorMessage.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.vendor_message_pagination_response import VendorMessagePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of VendorMessagePaginationResponse from a JSON string
vendor_message_pagination_response_instance = VendorMessagePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(VendorMessagePaginationResponse.to_json())

# convert the object into a dict
vendor_message_pagination_response_dict = vendor_message_pagination_response_instance.to_dict()
# create an instance of VendorMessagePaginationResponse from a dict
vendor_message_pagination_response_from_dict = VendorMessagePaginationResponse.from_dict(vendor_message_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


