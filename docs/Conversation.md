# Conversation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**contact** | [**Contact**](Contact.md) |  | 
**account_id** | **str** |  | 
**last_read_message_id** | **int** |  | [optional] 
**status** | **int** |  | [optional] 
**textkit_id** | **str** |  | [optional] 
**opportunity_score** | **int** |  | [optional] [default to 0]
**insights_widget_payload** | **object** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.conversation import Conversation

# TODO update the JSON string below
json = "{}"
# create an instance of Conversation from a JSON string
conversation_instance = Conversation.from_json(json)
# print the JSON string representation of the object
print(Conversation.to_json())

# convert the object into a dict
conversation_dict = conversation_instance.to_dict()
# create an instance of Conversation from a dict
conversation_from_dict = Conversation.from_dict(conversation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


