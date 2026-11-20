# ConversationPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Conversation]**](Conversation.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.conversation_pagination_response import ConversationPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ConversationPaginationResponse from a JSON string
conversation_pagination_response_instance = ConversationPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ConversationPaginationResponse.to_json())

# convert the object into a dict
conversation_pagination_response_dict = conversation_pagination_response_instance.to_dict()
# create an instance of ConversationPaginationResponse from a dict
conversation_pagination_response_from_dict = ConversationPaginationResponse.from_dict(conversation_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


