# MessageUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**conversation_id** | **int** |  | [optional] 
**content** | **str** |  | [optional] 
**action** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**reference_id** | **str** |  | [optional] 
**delivery_status** | **str** |  | [optional] 
**ip_address** | **str** |  | [optional] 
**associated_app_phone_number** | **str** |  | [optional] 
**associated_app_phone_number_type** | **str** |  | [optional] 
**message_template_id** | **str** |  | [optional] 
**bulk_message_id** | **int** |  | [optional] 
**date_added** | **datetime** |  | 
**date_sent** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_update import MessageUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageUpdate from a JSON string
message_update_instance = MessageUpdate.from_json(json)
# print the JSON string representation of the object
print(MessageUpdate.to_json())

# convert the object into a dict
message_update_dict = message_update_instance.to_dict()
# create an instance of MessageUpdate from a dict
message_update_from_dict = MessageUpdate.from_dict(message_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


