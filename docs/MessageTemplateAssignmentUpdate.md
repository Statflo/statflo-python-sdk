# MessageTemplateAssignmentUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**property_id** | **int** |  | [optional] 
**template_id** | **str** |  | [optional] 
**dealer_id** | **int** |  | [optional] 
**priority** | **int** |  | [optional] 
**assign_date** | **datetime** |  | [optional] 
**date_update** | **datetime** |  | [optional] 
**unassign_date** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_template_assignment_update import MessageTemplateAssignmentUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateAssignmentUpdate from a JSON string
message_template_assignment_update_instance = MessageTemplateAssignmentUpdate.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateAssignmentUpdate.to_json())

# convert the object into a dict
message_template_assignment_update_dict = message_template_assignment_update_instance.to_dict()
# create an instance of MessageTemplateAssignmentUpdate from a dict
message_template_assignment_update_from_dict = MessageTemplateAssignmentUpdate.from_dict(message_template_assignment_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


