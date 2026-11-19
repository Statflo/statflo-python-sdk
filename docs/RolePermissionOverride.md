# RolePermissionOverride


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | [**Role**](Role.md) |  | 
**permission** | [**Permission**](Permission.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 

## Example

```python
from statflo_python_sdk.models.role_permission_override import RolePermissionOverride

# TODO update the JSON string below
json = "{}"
# create an instance of RolePermissionOverride from a JSON string
role_permission_override_instance = RolePermissionOverride.from_json(json)
# print the JSON string representation of the object
print(RolePermissionOverride.to_json())

# convert the object into a dict
role_permission_override_dict = role_permission_override_instance.to_dict()
# create an instance of RolePermissionOverride from a dict
role_permission_override_from_dict = RolePermissionOverride.from_dict(role_permission_override_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


