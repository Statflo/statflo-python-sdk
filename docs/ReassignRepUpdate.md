# ReassignRepUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**new_external_user_id** | **str** |  | [optional] 
**old_external_user_id** | **str** |  | [optional] 
**new_external_location_id** | **str** |  | [optional] 
**old_external_location_id** | **str** |  | [optional] 
**account_name** | **str** |  | 
**account_id** | **str** |  | 
**date_changed** | **datetime** |  | 
**reason** | **str** |  | [optional] 
**old_ban** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.reassign_rep_update import ReassignRepUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ReassignRepUpdate from a JSON string
reassign_rep_update_instance = ReassignRepUpdate.from_json(json)
# print the JSON string representation of the object
print(ReassignRepUpdate.to_json())

# convert the object into a dict
reassign_rep_update_dict = reassign_rep_update_instance.to_dict()
# create an instance of ReassignRepUpdate from a dict
reassign_rep_update_from_dict = ReassignRepUpdate.from_dict(reassign_rep_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


