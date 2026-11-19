# TaskCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | 
**status** | **str** |  | [optional] [default to 'To Do']
**user_id_assigned** | **int** |  | [optional] 
**priority** | **int** |  | [optional] [default to 3]
**due_date** | **datetime** |  | 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.task_create import TaskCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TaskCreate from a JSON string
task_create_instance = TaskCreate.from_json(json)
# print the JSON string representation of the object
print(TaskCreate.to_json())

# convert the object into a dict
task_create_dict = task_create_instance.to_dict()
# create an instance of TaskCreate from a dict
task_create_from_dict = TaskCreate.from_dict(task_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


