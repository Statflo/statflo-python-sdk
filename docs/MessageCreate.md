# MessageCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user_id** | **int** |  | 
**conversation_id** | **int** |  | 
**content** | **str** |  | [optional] [default to '']
**action** | **str** |  | 
**provider** | **str** |  | [optional] [default to 'twilio']
**reference_id** | **str** |  | [optional] 
**delivery_status** | **str** |  | [optional] [default to 'new']
**ip_address** | **str** |  | [optional] 
**associated_app_phone_number** | **str** |  | [optional] 
**associated_app_phone_number_type** | **str** |  | [optional] 
**message_template_id** | **str** |  | [optional] 
**bulk_message_id** | **int** |  | [optional] 
**date_added** | **datetime** |  | 
**date_sent** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_create import MessageCreate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageCreate from a JSON string
message_create_instance = MessageCreate.from_json(json)
# print the JSON string representation of the object
print(MessageCreate.to_json())

# convert the object into a dict
message_create_dict = message_create_instance.to_dict()
# create an instance of MessageCreate from a dict
message_create_from_dict = MessageCreate.from_dict(message_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


