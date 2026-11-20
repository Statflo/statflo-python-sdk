# RolePermissionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dealer_blacklisted** | **bool** |  | [optional] [default to False]

## Example

```python
from statflo_python_sdk.models.role_permission_create import RolePermissionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RolePermissionCreate from a JSON string
role_permission_create_instance = RolePermissionCreate.from_json(json)
# print the JSON string representation of the object
print(RolePermissionCreate.to_json())

# convert the object into a dict
role_permission_create_dict = role_permission_create_instance.to_dict()
# create an instance of RolePermissionCreate from a dict
role_permission_create_from_dict = RolePermissionCreate.from_dict(role_permission_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


