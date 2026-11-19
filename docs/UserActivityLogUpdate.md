# UserActivityLogUpdate


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
from statflo_python_sdk.models.user_activity_log_update import UserActivityLogUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of UserActivityLogUpdate from a JSON string
user_activity_log_update_instance = UserActivityLogUpdate.from_json(json)
# print the JSON string representation of the object
print(UserActivityLogUpdate.to_json())

# convert the object into a dict
user_activity_log_update_dict = user_activity_log_update_instance.to_dict()
# create an instance of UserActivityLogUpdate from a dict
user_activity_log_update_from_dict = UserActivityLogUpdate.from_dict(user_activity_log_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


