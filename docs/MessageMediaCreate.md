# MessageMediaCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**message_id** | **int** |  | 
**url** | **str** |  | 
**content_type** | **str** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_media_create import MessageMediaCreate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageMediaCreate from a JSON string
message_media_create_instance = MessageMediaCreate.from_json(json)
# print the JSON string representation of the object
print(MessageMediaCreate.to_json())

# convert the object into a dict
message_media_create_dict = message_media_create_instance.to_dict()
# create an instance of MessageMediaCreate from a dict
message_media_create_from_dict = MessageMediaCreate.from_dict(message_media_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


