# MessageMediaPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[MessageMedia]**](MessageMedia.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_media_pagination_response import MessageMediaPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MessageMediaPaginationResponse from a JSON string
message_media_pagination_response_instance = MessageMediaPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(MessageMediaPaginationResponse.to_json())

# convert the object into a dict
message_media_pagination_response_dict = message_media_pagination_response_instance.to_dict()
# create an instance of MessageMediaPaginationResponse from a dict
message_media_pagination_response_from_dict = MessageMediaPaginationResponse.from_dict(message_media_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


