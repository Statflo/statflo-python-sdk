# MessageMedia


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**message** | [**Message**](Message.md) |  | 
**url** | **str** |  | 
**content_type** | **str** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_media import MessageMedia

# TODO update the JSON string below
json = "{}"
# create an instance of MessageMedia from a JSON string
message_media_instance = MessageMedia.from_json(json)
# print the JSON string representation of the object
print(MessageMedia.to_json())

# convert the object into a dict
message_media_dict = message_media_instance.to_dict()
# create an instance of MessageMedia from a dict
message_media_from_dict = MessageMedia.from_dict(message_media_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


