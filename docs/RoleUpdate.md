# RoleUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**display_in_app** | **bool** |  | [optional] 
**order** | **int** |  | 
**restrict_by_sales_rep_id** | **bool** |  | [optional] 
**restrict_by_outlet_id** | **bool** |  | [optional] 
**restrict_by_region_id** | **bool** |  | [optional] 
**restrict_by_district_id** | **bool** |  | [optional] 
**linked_feature_flag** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.role_update import RoleUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RoleUpdate from a JSON string
role_update_instance = RoleUpdate.from_json(json)
# print the JSON string representation of the object
print(RoleUpdate.to_json())

# convert the object into a dict
role_update_dict = role_update_instance.to_dict()
# create an instance of RoleUpdate from a dict
role_update_from_dict = RoleUpdate.from_dict(role_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


