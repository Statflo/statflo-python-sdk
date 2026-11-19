# ConversationCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**contact_id** | **int** |  | [optional] 
**account_id** | **str** |  | 
**last_read_message_id** | **int** |  | [optional] 
**status** | **int** |  | [optional] 
**textkit_id** | **str** |  | [optional] 
**opportunity_score** | **int** |  | [optional] [default to 0]
**insights_widget_payload** | **object** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.conversation_create import ConversationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ConversationCreate from a JSON string
conversation_create_instance = ConversationCreate.from_json(json)
# print the JSON string representation of the object
print(ConversationCreate.to_json())

# convert the object into a dict
conversation_create_dict = conversation_create_instance.to_dict()
# create an instance of ConversationCreate from a dict
conversation_create_from_dict = ConversationCreate.from_dict(conversation_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


