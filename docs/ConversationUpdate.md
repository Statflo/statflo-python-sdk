# ConversationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**contact_id** | **int** |  | [optional] 
**account_id** | **str** |  | 
**last_read_message_id** | **int** |  | [optional] 
**status** | **int** |  | [optional] 
**textkit_id** | **str** |  | [optional] 
**opportunity_score** | **int** |  | [optional] 
**insights_widget_payload** | **object** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.conversation_update import ConversationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ConversationUpdate from a JSON string
conversation_update_instance = ConversationUpdate.from_json(json)
# print the JSON string representation of the object
print(ConversationUpdate.to_json())

# convert the object into a dict
conversation_update_dict = conversation_update_instance.to_dict()
# create an instance of ConversationUpdate from a dict
conversation_update_from_dict = ConversationUpdate.from_dict(conversation_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


