# MessageDeliveryStatusCreate


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
from statflo_python_sdk.models.message_delivery_status_create import MessageDeliveryStatusCreate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageDeliveryStatusCreate from a JSON string
message_delivery_status_create_instance = MessageDeliveryStatusCreate.from_json(json)
# print the JSON string representation of the object
print(MessageDeliveryStatusCreate.to_json())

# convert the object into a dict
message_delivery_status_create_dict = message_delivery_status_create_instance.to_dict()
# create an instance of MessageDeliveryStatusCreate from a dict
message_delivery_status_create_from_dict = MessageDeliveryStatusCreate.from_dict(message_delivery_status_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


