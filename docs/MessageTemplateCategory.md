# MessageTemplateCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 

## Example

```python
from statflo_python_sdk.models.message_template_category import MessageTemplateCategory

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateCategory from a JSON string
message_template_category_instance = MessageTemplateCategory.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateCategory.to_json())

# convert the object into a dict
message_template_category_dict = message_template_category_instance.to_dict()
# create an instance of MessageTemplateCategory from a dict
message_template_category_from_dict = MessageTemplateCategory.from_dict(message_template_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


