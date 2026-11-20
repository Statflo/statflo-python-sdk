# MessageTemplateAssignment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**var_property** | [**CampaignProperty**](CampaignProperty.md) |  | 
**template** | [**MessageTemplate**](MessageTemplate.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**priority** | **int** |  | [optional] [default to 100]
**assign_date** | **datetime** |  | [optional] 
**date_update** | **datetime** |  | [optional] 
**unassign_date** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_template_assignment import MessageTemplateAssignment

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateAssignment from a JSON string
message_template_assignment_instance = MessageTemplateAssignment.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateAssignment.to_json())

# convert the object into a dict
message_template_assignment_dict = message_template_assignment_instance.to_dict()
# create an instance of MessageTemplateAssignment from a dict
message_template_assignment_from_dict = MessageTemplateAssignment.from_dict(message_template_assignment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


