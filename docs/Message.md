# Message


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user** | [**User**](User.md) |  | 
**conversation** | [**Conversation**](Conversation.md) |  | 
**content** | **str** |  | [optional] [default to '']
**action** | **str** |  | [optional] 
**provider** | **str** |  | [optional] [default to 'twilio']
**reference_id** | **str** |  | [optional] 
**delivery_status** | **str** |  | [optional] [default to 'new']
**ip_address** | **str** |  | [optional] 
**associated_app_phone_number** | **str** |  | [optional] 
**associated_app_phone_number_type** | **str** |  | [optional] 
**message_template** | [**MessageTemplate**](MessageTemplate.md) |  | 
**bulk_message** | [**BulkMessage**](BulkMessage.md) |  | 
**date_added** | **datetime** |  | 
**date_sent** | **datetime** |  | [optional] 
**media** | [**List[MessageMedia]**](MessageMedia.md) |  | 

## Example

```python
from statflo_python_sdk.models.message import Message

# TODO update the JSON string below
json = "{}"
# create an instance of Message from a JSON string
message_instance = Message.from_json(json)
# print the JSON string representation of the object
print(Message.to_json())

# convert the object into a dict
message_dict = message_instance.to_dict()
# create an instance of Message from a dict
message_from_dict = Message.from_dict(message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


