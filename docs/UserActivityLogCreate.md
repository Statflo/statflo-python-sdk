# UserActivityLogCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**activity_performed** | **str** |  | [optional] 
**date_added** | **datetime** |  | 
**module** | **str** |  | [optional] 
**code** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_activity_log_create import UserActivityLogCreate

# TODO update the JSON string below
json = "{}"
# create an instance of UserActivityLogCreate from a JSON string
user_activity_log_create_instance = UserActivityLogCreate.from_json(json)
# print the JSON string representation of the object
print(UserActivityLogCreate.to_json())

# convert the object into a dict
user_activity_log_create_dict = user_activity_log_create_instance.to_dict()
# create an instance of UserActivityLogCreate from a dict
user_activity_log_create_from_dict = UserActivityLogCreate.from_dict(user_activity_log_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


