# MessageDeliveryStatusPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[MessageDeliveryStatus]**](MessageDeliveryStatus.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_delivery_status_pagination_response import MessageDeliveryStatusPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MessageDeliveryStatusPaginationResponse from a JSON string
message_delivery_status_pagination_response_instance = MessageDeliveryStatusPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(MessageDeliveryStatusPaginationResponse.to_json())

# convert the object into a dict
message_delivery_status_pagination_response_dict = message_delivery_status_pagination_response_instance.to_dict()
# create an instance of MessageDeliveryStatusPaginationResponse from a dict
message_delivery_status_pagination_response_from_dict = MessageDeliveryStatusPaginationResponse.from_dict(message_delivery_status_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


