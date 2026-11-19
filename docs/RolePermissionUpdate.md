# RolePermissionUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dealer_blacklisted** | **bool** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.role_permission_update import RolePermissionUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RolePermissionUpdate from a JSON string
role_permission_update_instance = RolePermissionUpdate.from_json(json)
# print the JSON string representation of the object
print(RolePermissionUpdate.to_json())

# convert the object into a dict
role_permission_update_dict = role_permission_update_instance.to_dict()
# create an instance of RolePermissionUpdate from a dict
role_permission_update_from_dict = RolePermissionUpdate.from_dict(role_permission_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


