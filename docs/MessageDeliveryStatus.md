# MessageDeliveryStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**message** | [**Message**](Message.md) |  | 
**postback** | **object** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_delivery_status import MessageDeliveryStatus

# TODO update the JSON string below
json = "{}"
# create an instance of MessageDeliveryStatus from a JSON string
message_delivery_status_instance = MessageDeliveryStatus.from_json(json)
# print the JSON string representation of the object
print(MessageDeliveryStatus.to_json())

# convert the object into a dict
message_delivery_status_dict = message_delivery_status_instance.to_dict()
# create an instance of MessageDeliveryStatus from a dict
message_delivery_status_from_dict = MessageDeliveryStatus.from_dict(message_delivery_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


