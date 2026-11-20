# UserPermissionUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**blacklisted** | **bool** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_permission_update import UserPermissionUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of UserPermissionUpdate from a JSON string
user_permission_update_instance = UserPermissionUpdate.from_json(json)
# print the JSON string representation of the object
print(UserPermissionUpdate.to_json())

# convert the object into a dict
user_permission_update_dict = user_permission_update_instance.to_dict()
# create an instance of UserPermissionUpdate from a dict
user_permission_update_from_dict = UserPermissionUpdate.from_dict(user_permission_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


