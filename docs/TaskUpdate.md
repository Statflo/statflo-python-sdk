# TaskUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | 
**status** | **str** |  | [optional] 
**user_id_assigned** | **int** |  | [optional] 
**priority** | **int** |  | [optional] 
**due_date** | **datetime** |  | 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.task_update import TaskUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of TaskUpdate from a JSON string
task_update_instance = TaskUpdate.from_json(json)
# print the JSON string representation of the object
print(TaskUpdate.to_json())

# convert the object into a dict
task_update_dict = task_update_instance.to_dict()
# create an instance of TaskUpdate from a dict
task_update_from_dict = TaskUpdate.from_dict(task_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


