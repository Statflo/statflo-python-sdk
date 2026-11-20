# RoleCreate


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

## Example

```python
from statflo_python_sdk.models.role_create import RoleCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RoleCreate from a JSON string
role_create_instance = RoleCreate.from_json(json)
# print the JSON string representation of the object
print(RoleCreate.to_json())

# convert the object into a dict
role_create_dict = role_create_instance.to_dict()
# create an instance of RoleCreate from a dict
role_create_from_dict = RoleCreate.from_dict(role_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


