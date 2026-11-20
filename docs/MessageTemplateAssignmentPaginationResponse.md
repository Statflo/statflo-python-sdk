# MessageTemplateAssignmentPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[MessageTemplateAssignment]**](MessageTemplateAssignment.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.message_template_assignment_pagination_response import MessageTemplateAssignmentPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MessageTemplateAssignmentPaginationResponse from a JSON string
message_template_assignment_pagination_response_instance = MessageTemplateAssignmentPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(MessageTemplateAssignmentPaginationResponse.to_json())

# convert the object into a dict
message_template_assignment_pagination_response_dict = message_template_assignment_pagination_response_instance.to_dict()
# create an instance of MessageTemplateAssignmentPaginationResponse from a dict
message_template_assignment_pagination_response_from_dict = MessageTemplateAssignmentPaginationResponse.from_dict(message_template_assignment_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


