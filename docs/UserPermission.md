# UserPermission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**User**](User.md) |  | 
**permission** | [**Permission**](Permission.md) |  | 
**blacklisted** | **bool** |  | [optional] [default to False]

## Example

```python
from statflo_python_sdk.models.user_permission import UserPermission

# TODO update the JSON string below
json = "{}"
# create an instance of UserPermission from a JSON string
user_permission_instance = UserPermission.from_json(json)
# print the JSON string representation of the object
print(UserPermission.to_json())

# convert the object into a dict
user_permission_dict = user_permission_instance.to_dict()
# create an instance of UserPermission from a dict
user_permission_from_dict = UserPermission.from_dict(user_permission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


