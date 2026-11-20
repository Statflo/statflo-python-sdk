# MessageTemplateUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer_id** | **int** |  | [optional] 
**template_name** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 
**template** | **object** |  | 
**priority** | **int** |  | [optional] 
**category_ids** | **List[int]** |  | [optional] 
**date_created** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.message_template_update import MessageTemplateUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateUpdate from a JSON string
message_template_update_instance = MessageTemplateUpdate.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateUpdate.to_json())

# convert the object into a dict
message_template_update_dict = message_template_update_instance.to_dict()
# create an instance of MessageTemplateUpdate from a dict
message_template_update_from_dict = MessageTemplateUpdate.from_dict(message_template_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


