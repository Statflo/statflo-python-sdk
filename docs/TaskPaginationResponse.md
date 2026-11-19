# TaskPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Task]**](Task.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.task_pagination_response import TaskPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TaskPaginationResponse from a JSON string
task_pagination_response_instance = TaskPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(TaskPaginationResponse.to_json())

# convert the object into a dict
task_pagination_response_dict = task_pagination_response_instance.to_dict()
# create an instance of TaskPaginationResponse from a dict
task_pagination_response_from_dict = TaskPaginationResponse.from_dict(task_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


