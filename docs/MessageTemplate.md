# MessageTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**template_name** | **str** |  | [optional] 
**language** | **str** |  | [optional] [default to 'en']
**metadata** | **object** |  | [optional] 
**template** | **object** |  | [optional] 
**campaign** | [**Campaign**](Campaign.md) |  | 
**priority** | **int** |  | [optional] [default to 100]
**message_template_assignments** | [**List[MessageTemplateAssignment]**](MessageTemplateAssignment.md) |  | 
**categories** | [**List[MessageTemplateCategory]**](MessageTemplateCategory.md) |  | 
**date_created** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.message_template import MessageTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplate from a JSON string
message_template_instance = MessageTemplate.from_json(json)
# print the JSON string representation of the object
print(MessageTemplate.to_json())

# convert the object into a dict
message_template_dict = message_template_instance.to_dict()
# create an instance of MessageTemplate from a dict
message_template_from_dict = MessageTemplate.from_dict(message_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


