# MessageMediaUpdate


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
from statflo_python_sdk.models.message_media_update import MessageMediaUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageMediaUpdate from a JSON string
message_media_update_instance = MessageMediaUpdate.from_json(json)
# print the JSON string representation of the object
print(MessageMediaUpdate.to_json())

# convert the object into a dict
message_media_update_dict = message_media_update_instance.to_dict()
# create an instance of MessageMediaUpdate from a dict
message_media_update_from_dict = MessageMediaUpdate.from_dict(message_media_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


