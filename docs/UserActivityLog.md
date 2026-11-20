# UserActivityLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user** | [**User**](User.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**date_added** | **datetime** |  | 
**module** | **str** |  | [optional] 
**code** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_activity_log import UserActivityLog

# TODO update the JSON string below
json = "{}"
# create an instance of UserActivityLog from a JSON string
user_activity_log_instance = UserActivityLog.from_json(json)
# print the JSON string representation of the object
print(UserActivityLog.to_json())

# convert the object into a dict
user_activity_log_dict = user_activity_log_instance.to_dict()
# create an instance of UserActivityLog from a dict
user_activity_log_from_dict = UserActivityLog.from_dict(user_activity_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


