# MessageTemplateCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer_id** | **int** |  | [optional] 
**template_name** | **str** |  | 
**language** | **str** |  | [optional] [default to 'en']
**metadata** | **object** |  | [optional] 
**template** | **object** |  | 
**priority** | **int** |  | [optional] [default to 100]
**category_ids** | **List[int]** |  | [optional] [default to []]
**date_created** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.message_template_create import MessageTemplateCreate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateCreate from a JSON string
message_template_create_instance = MessageTemplateCreate.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateCreate.to_json())

# convert the object into a dict
message_template_create_dict = message_template_create_instance.to_dict()
# create an instance of MessageTemplateCreate from a dict
message_template_create_from_dict = MessageTemplateCreate.from_dict(message_template_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


