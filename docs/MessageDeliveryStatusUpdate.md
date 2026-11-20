# MessageDeliveryStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**message_id** | **int** |  | 
**postback** | **object** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_delivery_status_update import MessageDeliveryStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageDeliveryStatusUpdate from a JSON string
message_delivery_status_update_instance = MessageDeliveryStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(MessageDeliveryStatusUpdate.to_json())

# convert the object into a dict
message_delivery_status_update_dict = message_delivery_status_update_instance.to_dict()
# create an instance of MessageDeliveryStatusUpdate from a dict
message_delivery_status_update_from_dict = MessageDeliveryStatusUpdate.from_dict(message_delivery_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


