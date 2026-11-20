# UserPermissionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**blacklisted** | **bool** |  | [optional] [default to False]

## Example

```python
from statflo_python_sdk.models.user_permission_create import UserPermissionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of UserPermissionCreate from a JSON string
user_permission_create_instance = UserPermissionCreate.from_json(json)
# print the JSON string representation of the object
print(UserPermissionCreate.to_json())

# convert the object into a dict
user_permission_create_dict = user_permission_create_instance.to_dict()
# create an instance of UserPermissionCreate from a dict
user_permission_create_from_dict = UserPermissionCreate.from_dict(user_permission_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


