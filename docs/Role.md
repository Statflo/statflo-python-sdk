# Role


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**display_in_app** | **bool** |  | [optional] [default to True]
**order** | **int** |  | 
**restrict_by_sales_rep_id** | **bool** |  | [optional] [default to True]
**restrict_by_outlet_id** | **bool** |  | [optional] [default to True]
**restrict_by_region_id** | **bool** |  | [optional] [default to True]
**restrict_by_district_id** | **bool** |  | [optional] [default to True]
**linked_feature_flag** | **int** |  | [optional] [default to 0]
**role_permissions** | [**List[RolePermission]**](RolePermission.md) |  | 
**role_permission_overrides** | [**List[RolePermissionOverride]**](RolePermissionOverride.md) |  | 

## Example

```python
from statflo_python_sdk.models.role import Role

# TODO update the JSON string below
json = "{}"
# create an instance of Role from a JSON string
role_instance = Role.from_json(json)
# print the JSON string representation of the object
print(Role.to_json())

# convert the object into a dict
role_dict = role_instance.to_dict()
# create an instance of Role from a dict
role_from_dict = Role.from_dict(role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


