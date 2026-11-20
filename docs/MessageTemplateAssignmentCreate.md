# MessageTemplateAssignmentCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**property_id** | **int** |  | [optional] 
**template_id** | **str** |  | [optional] 
**dealer_id** | **int** |  | [optional] 
**priority** | **int** |  | [optional] [default to 100]
**assign_date** | **datetime** |  | [optional] 
**date_update** | **datetime** |  | [optional] 
**unassign_date** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_template_assignment_create import MessageTemplateAssignmentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateAssignmentCreate from a JSON string
message_template_assignment_create_instance = MessageTemplateAssignmentCreate.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateAssignmentCreate.to_json())

# convert the object into a dict
message_template_assignment_create_dict = message_template_assignment_create_instance.to_dict()
# create an instance of MessageTemplateAssignmentCreate from a dict
message_template_assignment_create_from_dict = MessageTemplateAssignmentCreate.from_dict(message_template_assignment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


